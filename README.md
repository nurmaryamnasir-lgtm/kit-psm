# Kit PD

Mad'u tracking and development workspace for PEMBINA Shah Alam.

Kit PD follows individuals through the Mutabaah → Muhib → Muayyid stages, records
usrah and follow-up activity, plans wasilah programmes, handles Bajet Muayyasyah
claims, and carries the reference material a Penggerak Dakwah needs while
planning.

## Running it

Plain HTML, CSS and JavaScript — no build step, no framework, no dependencies to
install. Either open `index.html` directly in a browser, or serve the folder so
that relative paths and `localStorage` behave like production:

```bash
python3 -m http.server 8000    # then open http://localhost:8000
```

Serving is preferable: opening over `file://` gives the page an opaque origin in
some browsers, which breaks `localStorage` and therefore the offline cache.

## Files

```
index.html                     the whole application
  ├─ <head>                    meta, theme colour, SheetJS from cdnjs
  ├─ <link> design-system.css  shared tokens and primitives
  ├─ <style>                   application CSS
  ├─ <body>                    header, tab bar, #app mount, login gate, toast
  └─ <script>                  state, views, event delegation, sync, import/export
components/design-system.css   design tokens and shared primitives
public/logo-pembina-shah-alam.png
DESIGN.md                      the design system, in full
PRODUCT.md                     product purpose and constraints
```

`design-system.css` is linked **before** the inline `<style>` block, so
page-specific rules in `index.html` still win any conflict.

The logo is embedded in `index.html` as a base64 data URI (header and login
gate), so the page renders standalone; `public/logo-pembina-shah-alam.png` is
the same image as a separate file.

## How the app is put together

There is no framework and no virtual DOM. The pattern throughout is:

- **One state object**, `S`, holding `people`, `meetings`, `wasilah`, `claims`,
  `holidays`, `pdList` and the managed option lists.
- **`render()`** switches on the current `view` and assigns a template string to
  `#app.innerHTML` — one `viewXxx()` function per tab.
- **Event delegation.** Single `click`, `input` and `change` listeners on
  `document` read `data-*` attributes to find their target: `data-sel` opens a
  member, `data-ed` edits a person field, `data-tgl` flips a toggle,
  `data-score` sets a BPMy score, `data-wed` / `data-ced` / `data-hed` edit a
  programme, claim or important date. Adding UI means emitting the right
  `data-*` attribute, not wiring a listener.
- **`save()`** debounces a write to the local cache and a push to the backend.

Keeping to that pattern matters: because markup is regenerated wholesale on
render, per-element listeners would be lost on every update.

## Sign-in and data

The app talks to a Google Apps Script backend that holds the shared document and
brokers Drive uploads. The `/exec` endpoint is set once, near the top of the sync
section in `index.html`:

```js
const APPS_SCRIPT_URL = "https://script.google.com/macros/s/…/exec";
```

Sign-in takes your name plus the team access code that the Apps Script checks.
The name is recorded as the approver on any tarsyih (stage promotion) you make.

**Contact details are deliberately server-only.** Email, phone, birth date,
address, postcode and residential college are listed in `SENSITIVE` and stripped
before anything is written to the device cache, so they are readable only while
signed in. The local cache is a redacted convenience copy and expires after
seven days.

Edits save locally at once and push to the backend on a short debounce; the app
polls for other people's changes every 25 seconds, skips adopting a remote copy
while you are mid-edit, and beacons any pending edit on page unload.

Because the endpoint sits in client-side source, it is visible to anyone who
loads the page. The security boundary is the access code and the Apps Script's
own authorization settings — not the secrecy of that URL. Keep the script's
access restricted accordingly, and keep this repository private.

## Scoring

Borang Pencalonan Muayyid scores each item 0–5 against a per-item weight, out of
a fixed 720-point maximum; a muhib qualifies for muayyid at 50%. Percentages
shown against a category are percentages of that 720 total, not of the category
— this matches the paper form. See `BPMY` in `index.html`.

## Notes

- The Gagasan header link points at `gagasan.html`; drop that document beside
  `index.html` to make it resolve.
- Spreadsheet import accepts `.xlsx`, `.xls` and `.csv`, matches a range of
  Malay and English column headings, and skips rows whose name already exists.
  SheetJS is loaded from cdnjs; without it, import and BPMy export fall back to
  CSV.
