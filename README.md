# Kit Penggerak Dakwah — PEMBINA Shah Alam

Dua laman statik yang saling berpaut, untuk kegunaan **Penggerak Dakwah (PD)** — jejak kemenjadian ahli, rekod mesyuarat, dan rujukan gagasan. Berfungsi pada telefon **dan** web. Tiada pemasangan.

| Fail | Fungsi |
|---|---|
| `index.html` | **Penjejak PSM** — pipeline Takungan → Mutabaah → Muhib → Muayyid (auto-status), serta **Minit & Tindakan** untuk mesyuarat progres/feedback. |
| `gagasan.html` | **Kad Gagasan PEMBINA** — Visi & Misi, Objektif, kad produk (rujukan Hard Pitch). |

Kedua-dua berpaut: butang **Gagasan** pada penjejak, dan **Penjejak PSM** pada kad gagasan.

## Terbit di GitHub Pages
1. Buat repository baru (cth: `kit-pd`).
2. **Add file → Upload files** → seret masuk **index.html**, **gagasan.html**, **README.md** → **Commit**.
3. **Settings → Pages** → *Deploy from a branch* → **main** / **root** → **Save**.
4. Pautan: `https://<username>.github.io/kit-pd/` (penjejak) dan `.../gagasan.html` (kad).

## Guna semasa mesyuarat
- Tab **Penjejak Ahli**: kemas kini kehadiran & syarat setiap ahli; status "Layak Tarsyih / Kenaikan" terkira sendiri.
- Tab **Minit & Tindakan**: cipta rekod LMM/LMH, tulis minit, tambah **tindakan** (tugasan · PIC · tarikh akhir · status). Kotak **Tindakan Terbuka** mengumpul semua tindakan belum selesai merentas mesyuarat — senarai semak untuk mesyuarat berikutnya.

## Data
- Disimpan automatik dalam **pelayar** peranti (localStorage) — tidak dikongsi antara peranti.
- **Simpan JSON** = backup penuh & pindah peranti. **Muat JSON** = pulih.
- **Export Ahli (CSV)** & **Export Tindakan (CSV)** = buka dalam Excel / Google Sheets.
- Tip telefon: buka sekali, kemudian **Add to Home Screen**.

> Privasi: jika repo *public*, elak taip nombor telefon penuh; guna repo *private* untuk lebih selamat.
