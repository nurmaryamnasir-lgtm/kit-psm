---
name: Kit PD
description: PEMBINA Shah Alam mad'u tracking and development workspace
colors:
  blue-ink: "#072a63"
  blue: "#0a3b8c"
  blue-2: "#1657c4"
  blueb: "#3f74d6"
  yellow: "#ffce33"
  ink: "#0e1726"
  muted: "#5b6b86"
  line: "#e3e9f4"
  paper: "#eef2fa"
  card: "#ffffff"
  green: "#1f9d55"
  green-soft: "#e4f6ec"
  amber: "#dd9021"
  amber-soft: "#fcf1dc"
  blue-soft: "#e4ecfb"
  grey-soft: "#eef1f7"
  red: "#d3453f"
  red-soft: "#fbe6e5"
  purple: "#6b3fa0"
  teal: "#1f8f80"
  teal-soft: "#e3f5f1"
  pink: "#c2367a"
  pink-soft: "#fde8f1"
  on-blue-label: "#bcd0f5"
  on-blue-sub: "#cfe0ff"
  on-blue-body: "#dbe6ff"
  yellow-soft: "#fff3c9"
  yellow-tint: "#fff7e0"
  yellow-deep: "#ffeab4"
  yellow-line: "#f2dda6"
  cream: "#fffdf5"
  blue-faint: "#7f95c4"
  red-line: "#f5c6c2"
  purple-soft: "#efe8f8"
  kd-red: "#c0201f"
  surface-raised: "#fcfdff"
  ipt-1: "#147FB3"
  ipt-2: "#2a9d8f"
  ipt-3: "#7048b6"
  ipt-4: "#d98324"
  ipt-5: "#e07b39"
  ipt-none: "#b8c2d6"
  shadow: "0 1px 2px rgba(9, 30, 66, .06), 0 6px 18px rgba(9, 30, 66, .07)"
typography:
  display:
    fontFamily: "ui-sans-serif, system-ui, 'Segoe UI', -apple-system, 'Helvetica Neue', Arial, sans-serif"
    fontSize: "clamp(2rem, 5vw, 2.8rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "ui-sans-serif, system-ui, 'Segoe UI', -apple-system, 'Helvetica Neue', Arial, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 800
    lineHeight: 1.25
    letterSpacing: "-0.02em"
  body:
    fontFamily: "ui-sans-serif, system-ui, 'Segoe UI', -apple-system, 'Helvetica Neue', Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "normal"
  label:
    fontFamily: "ui-sans-serif, system-ui, 'Segoe UI', -apple-system, 'Helvetica Neue', Arial, sans-serif"
    fontSize: "10.5px"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "0.04em"
  scale:
    micro: "9px"
    eyebrow: "10px"
    label: "10.5px"
    caps: "11px"
    helper: "11.5px"
    meta: "12px"
    secondary: "12.5px"
    compact: "13px"
    prose: "13.5px"
    control: "14px"
    card-title: "14.5px"
    body: "15px"
    panel-title: "16px"
    numeral: "18px"
    brand: "19px"
    heading: "20px"
    metric: "30px"
    empty-glyph: "32px"
rounded:
  rule: "2px"
  dot: "3px"
  spine: "4px"
  event: "5px"
  tag: "7px"
  xs: "8px"
  sm: "9px"
  control: "10px"
  md: "11px"
  panel: "12px"
  lg: "13px"
  surface: "14px"
  sheet: "18px"
  badge: "20px"
  xl: "22px"
  circle: "50%"
spacing:
  xs: "4px"
  sm: "8px"
  md: "10px"
  lg: "12px"
  xl: "16px"
  xxl: "24px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.card}"
    rounded: "{rounded.md}"
    padding: "10px 16px"
    typography: "{typography.label}"
  button-secondary:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "10px 14px"
    typography: "{typography.body}"
  button-destructive:
    backgroundColor: "{colors.card}"
    textColor: "{colors.red}"
    rounded: "{rounded.md}"
    padding: "12px 15px"
    typography: "{typography.body}"
  field:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "10px 11px"
    typography: "{typography.body}"
  card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.lg}"
    padding: "12px"
    shadow: "{colors.shadow}"
---

# Design System: Kit PD

## Overview

**Creative North Star: "Operational clarity with institutional authority"**

Kit PD is a disciplined operational dashboard for PEMBINA organizers: its design language prioritizes trust, speed, and legibility over decoration. The system is grounded in a strong blue institutional palette, quiet surfaces, and a consistent application of cards, pills, toggles, and tables that support high-volume admin work. It feels serious and usable, with enough structure to stay calm even as records, follow-ups, and developmental stages pile up.

The visual world is intentionally practical: the eye is guided through stacked panels, tertiary metadata, and clear status color cues rather than dramatic art direction. The UI favors readable density, task completion, and operational confidence. The system uses soft layering, calibrated contrast, and controlled rhythm to make repetitive data entry feel manageable.

**Key Characteristics:**
- Strong blue institutional identity
- High clarity for data-heavy workflow screens
- Calm, low-noise surfaces with subtle elevation
- Clear status signaling via green, amber, red, and blue variants
- Compact but spacious card grids tuned for admin use

## Colors

The palette is anchored in a deep blue brand presence with supporting neutral, green, amber, red, and purple accents. The main principle is simple: blue carries the product identity, while the status colors are used carefully as indicators rather than decoration.

### Primary
- **Blue Ink** (#072a63): primary header treatment and the accent foundation for the product shell.
- **Blue** (#0a3b8c): main action color for primary buttons, active pills, and high-priority UI states.
- **Blue 2** (#1657c4): hover/secondary-blue state for active interactivity when the primary blue is already in use.
- **Blue B** (#3f74d6): secondary interaction/information accent; used for neutral active states and supportive highlight areas.

### Secondary
- **Yellow** (#ffce33): brand signal and supportive emphasis; used as a subtle badge or high-contrast signal on blue surfaces.
- **Green** (#1f9d55): success status and positive progression, especially in completion states and approval cues.
- **Amber** (#dd9021): caution and watch status, ideal for pending or attention-needed states.
- **Red** (#d3453f): warning or blocking states; used for removals, errors, or negative conditions.
- **Purple** (#6b3fa0): alternate roadmap or special marker color for non-core status distinctions.
- **Teal** (#1f8f80) / **Teal Soft** (#e3f5f1): mixed-participant programmes and DF sessions, distinguished from the blue used for women-only activity.
- **Pink** (#c2367a) / **Pink Soft** (#fde8f1): birthdays — the one calendar entry that is personal rather than operational, so it sits outside the status colors on purpose.

### Neutral
- **Ink** (#0e1726): default foreground color for text and critical labels.
- **Muted** (#5b6b86): secondary text, helper labels, and less dominant metadata.
- **Line** (#e3e9f4): borders, dividers, and form outlines.
- **Paper** (#eef2fa): page background and low-contrast surfaces.
- **Card** (#ffffff): base surface for content cards, drawers, panels, and forms.
- **Grey Soft** (#eef1f7): low-emphasis state backgrounds and calm neutral panels.

### On-Blue Text Tints

Deep blue surfaces — the product header, the BPMy summary panel, the active journey stage — need their own text ramp, because Ink and Muted are unreadable on them. Three steps cover every case, low to high contrast:

- **On Blue Label** (#bcd0f5): uppercase micro-labels and eyebrow text on a blue surface.
- **On Blue Sub** (#cfe0ff): supporting subtitles beneath a heading on blue.
- **On Blue Body** (#dbe6ff): body rows and table cells on blue, with pure white reserved for the value being emphasized.

### Soft Tints and Surfaces

Every status color needs a soft counterpart to sit behind it, and the yellow brand signal needs a wider family than the others because it carries the Muayyid stage, the "now" marker on the phase timeline, and the reference callout:

- **Yellow Soft** (#fff3c9): Muayyid avatar, programme tag, and the glow around the current phase node.
- **Yellow Tint** (#fff7e0) / **Yellow Deep** (#ffeab4): the two stops of the Muayyid journey-stage gradient.
- **Yellow Line** (#f2dda6): the border that pairs with those cream fills.
- **Cream** (#fffdf5): the reference callout surface, warmer than Paper so a definition reads as an aside.
- **Purple Soft** (#efe8f8): PD tag and the semester-break calendar chip.
- **Red Line** (#f5c6c2): the border on an absence cell, where Red Soft alone is not legible enough.
- **Blue Faint** (#7f95c4): Mutabaah avatar text — the quietest stage marker, since Mutabaah is the default state.
- **Surface Raised** (#fcfdff): the body of an expanded row, a hair lighter than Card so the open panel reads as nested.
- **KD Red** (#c0201f): reserved for Kalam Dakwah slide headers, which reproduce that deck's own brand red and are deliberately not the system's Red.

### Categorical Palette

Institutions get a stable identity color so a row can be scanned by its colour spine alone. This is a *data* palette, not a UI palette: the values carry no status meaning and must never be reused for state. The three local institutions are pinned (MSU → Purple, UiTM Shah Alam → #e07b39, UiTM Puncak Perdana → Green) and anything else hashes into the rotation — **IPT 1** (#147fb3), **IPT 2** (#2a9d8f), **IPT 3** (#7048b6), **IPT 4** (#d98324), Blue B, and Pink. **IPT None** (#b8c2d6) marks a record with no institution recorded. See `iptColor` in `lib/model.ts`.

### Named Rules
**The Blue-First Rule.** The product's dominant accent is blue; the system only introduces green, amber, red, and purple to communicate status and category distinctions, never as a competing interface identity.

**The Data-Palette Rule.** The categorical IPT colors are addressed only through `iptColor()`. They never appear as a hand-picked accent in a component, and no status is ever encoded with them.

## Typography

**Display Font:** ui-sans-serif, system-ui, "Segoe UI", -apple-system, "Helvetica Neue", Arial, sans-serif
**Body Font:** ui-sans-serif, system-ui, "Segoe UI", -apple-system, "Helvetica Neue", Arial, sans-serif
**Label Font:** ui-sans-serif, system-ui, "Segoe UI", -apple-system, "Helvetica Neue", Arial, sans-serif

The interface uses a practical sans-serif stack tuned for dense operational reading. It prioritizes clarity, clean rhythm, and immediate recognizability across tables, drawers, toggles, and forms.

### Hierarchy
- **Display** (800, clamp(2rem, 5vw, 2.8rem), 1.1): used for the most prominent product and section headings.
- **Headline** (800, 1.25rem, 1.25): used for panel titles, row names, and section labels.
- **Body** (400, 15px, 1.4): default reading size for application content, forms, and metadata.
- **Label** (800, 10.5px, 1.2, tracking 0.04em): small uppercase labels for fields and UI metadata.

### Size Ramp

The four roles above name the *intent*. Because this is a dense operational tool, the implemented ramp is finer than four steps — a records table, a calendar cell, a form label and a drawer heading genuinely need different sizes, and half-pixel steps in the 11–15px band are doing real work separating metadata from content. The full enumerated ramp:

| Step | Size | Where it is used |
| --- | --- | --- |
| micro | 9px | calendar attendance tag inside a day cell |
| eyebrow | 10px | product eyebrow, calendar month abbreviation, journey annotations |
| label | 10.5px | field labels (the Label role) |
| caps | 11px | badges, pill counts, group headers, section headings |
| helper | 11.5px | hints, helper text, legends, secondary counts |
| meta | 12px | avatar initials, panel headings, tertiary metadata |
| secondary | 12.5px | name chips, descriptive body inside reference panels |
| compact | 13px | filter selects, editor tabs, stage pills, dense body |
| prose | 13.5px | reading body in reference panels, secondary buttons, toasts |
| control | 14px | navigation tabs, primary and destructive buttons, menu rows |
| card-title | 14.5px | accordion and criteria card titles |
| body | 15px | default reading size, inputs, row names (the Body role) |
| panel-title | 16px | drawer name, phase titles, journey stage names, calendar header |
| numeral | 18px | large day numeral in a date block |
| brand | 19px | the Kit PD wordmark in the header |
| heading | 20px | sign-in heading (the Headline role) |
| metric | 30px | the BPMy percentage in the summary panel |
| empty-glyph | 32px | empty-state glyph |

The Display role (`clamp(2rem, 5vw, 2.8rem)`) is reserved: nothing in the current product is large enough to need it.

### Named Rules
**The Label-First Rule.** Small labels are treated as functional orientation aids, not decorative copy; they are uppercase, bold, and high-contrast for quick scanning.

**The Dense-Band Rule.** Sizes between 11px and 15px carry almost the whole interface. Pick within that band by role — helper, metadata, body, control — rather than reaching for a new size; a step outside the ramp should be a deliberate addition to this table, not a one-off.

## Layout

The interface is built on a clear content rhythm: stacked cards, dense but breathable forms, and a modular grid. The layout is flexible but grounded in consistent spacing and narrow read widths for editor panels and task lists.

The product relies on a 2-column form pattern for many inline editors and a generous stack for detail drawers. Content blocks are separated by moderate padding, while rows and metadata groups use tight internal spacing to avoid visual drift.

Core rhythm values are defined by the design system tokens:
- 8px base spacing for tight grouping
- 10px–16px for standard row spacing and field rhythm
- 12px card padding for compact panels
- 24px larger separation when a section needs stronger chunking

The app uses a core background of paper blue, white cards on top, and border lines to preserve legibility without introducing heavy visual noise.

## Elevation & Depth

Depth is subtle and low-noise. Instead of dramatic shadows, the interface uses soft ambient layering to separate cards, drawers, and controls from the page surface. The system is intentionally restrained: depth signals the material relationship, not the drama of the content.

### Shadow Vocabulary
- **Ambient** (`0 1px 2px rgba(9, 30, 66, .06), 0 6px 18px rgba(9, 30, 66, .07)`): default card and surface shadow; used for layered panels, rows, and controls that should sit just above the page.

### Named Rules
**The Quiet Elevation Rule.** Shadows are present only to help structure and separation; they do not dominate a panel or serve as a purely decorative halo.

## Shapes

The visual language prefers soft, practical geometry. Corners are gently rounded, enough to humanize the interface without looking playful or decorative. The product avoids extreme radius values and instead uses modest radii that support tablet-style UIs and operational forms.

The four radii that carry the product's character:

- Small input corners: 9px (`sm`)
- Standard control radius: 11px (`md`)
- Card surface radius: 13px (`lg`)
- Larger emphasis pills and badges: 22px (`xl`)

### Radius Ramp

Rounding scales with the size of the thing being rounded, so the implemented ramp runs from 2px marks up to fully circular avatars. The full enumerated scale:

| Token | Radius | Where it is used |
| --- | --- | --- |
| rule | 2px | the yellow accent bar that prefixes a section heading |
| dot | 3px | status dots, legend swatches, IPT colour dots |
| spine | 4px | the IPT colour spine on a row, and the focus ring |
| event | 5px | calendar event chips inside a day cell |
| tag | 7px | the stage tag (MUT / MUH / MAY) in a table row |
| xs | 8px | calendar day cells, menu rows, small inline chips |
| sm | 9px | form fields, inputs, textareas, avatar squares |
| control | 10px | header buttons, filter selects, editor tabs, sub-rows |
| md | 11px | primary, secondary and destructive buttons |
| panel | 12px | grouped panels, popover menus, criteria cards, PD rows |
| lg | 13px | content cards and rows — the primary information plane |
| surface | 14px | larger surfaces: reference boxes, day detail, member cards |
| sheet | 18px | the sign-in sheet, the largest single surface |
| badge | 20px | tags, badges, name chips, duration pills |
| xl | 22px | filter pills and toggle pills |
| circle | 50% | avatars, numbered circles, timeline nodes |

Borders are light and present only where they matter, usually around form fields, rows, and small groups. The app keeps its overall silhouette professional and administrative.

### Named Rules
**The Radius-Follows-Size Rule.** A radius is chosen from the size of the element, not for emphasis: marks take 2–5px, controls 8–11px, panels and cards 12–14px, and only pills and avatars round fully. Rounding is never used to make something look more important.

## Components

### Buttons
- **Shape:** rounded 11px, with action padding tuned to compact data-entry use.
- **Primary:** deep blue background, white text, strong weight, used for focus-driving actions and primary workflow completion.
- **Secondary:** white background, dark text, soft border, suited to supporting actions and non-critical interactions.
- **Destructive:** white background, red text, red border accents, reserved for delete or removal actions.
- **Hover / Focus:** the system uses a strong blue focus ring and simple state shifts; hover is purposeful, not flashy.

### Form Fields
- **Shape:** 9px radius, white background, thin border, restrained padding.
- **State:** clean and readable, with emphasis placed on labels and consistent spacing instead of highly decorated inputs.
- **Focus:** a blue focus ring preserves keyboard accessibility without visual excess.

### Chips / Pills / Tags
- **Shape:** rounded 22px, supportive label styling, often used for status clusters and filter toggles.
- **Pattern:** active pills carry blue backgrounds with white text; neutral pills remain low-contrast and calm.
- **Use:** common in filters, counts, and mood/status groupings.

### Cards / Panels
- **Shape:** 13px radius with low-contrast borders and soft shadow.
- **Role:** create contained action areas for sections, drawers, records, and metadata groups.
- **Pattern:** the page's neutral paper background keeps cards readable, while the card itself remains the primary information plane.

### Toggle Chips
- **Shape:** small pill-like segmented buttons inside a bordered container.
- **State:** active toggles switch to blue or green depending on context; inactive toggles stay in white with muted text.
- **Role:** used heavily for binary decisions and lightweight filtering in the workflow.

## Do's and Don'ts

### Do
- **Do** use the blue theme as the default product voice; make blue the visual anchor of ongoing operational workflows.
- **Do** keep metadata small, uppercase, and highly scannable.
- **Do** preserve calm surfaces and subtle shadows so data remains readable and the interface feels trustworthy.
- **Do** use green, amber, and red only to clarify status, not to create visual noise.
- **Do** keep forms compact and consistent, with labels above fields for fast data-entry scanning.

### Don't
- **Don't** introduce highly decorative gradients, glass effects, or absurd shadow treatments; this system is practical first.
- **Don't** use decorative emojis or fake “illustrative” icons where a clear action label or SVG will do better.
- **Don't** distort the product into a playful aesthetic; the system is built for admin clarity and trust.
- **Don't** overuse colors for emphasis; status colors are intentionally controlled and rarely compete with the blue brand base.
- **Don't** collapse the interface into dense unlabeled blocks; the product relies on clear structure, spacing, and labels for orientation.
