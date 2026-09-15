---
version: alpha
name: AHKFlow
description: >-
  Design system for AHKFlow — an open-source AutoHotkey V2 hotstring manager &
  CLI for Windows (Blazor WebAssembly + ahkflow CLI on a shared API). A dense,
  spreadsheet-first productivity tool built as a tweaked MudBlazor 9.x theme.
  Tokens below are the LIGHT theme (canonical); dark-theme counterparts carry a
  `-dark` suffix and are documented in prose.
colors:
  # Brand anchors (nature-derived: spring-river green / blue / copper)
  primary: "#6AA84F"
  primary-surface: "#EEF7E9"
  on-primary-surface: "#2D5720"
  # AA-safe pair for filled buttons (white text) and outlined/text buttons
  # (brand text on a light surface). Dark-theme counterparts are darker/
  # lighter respectively, because dark theme lifts the whole brand ramp.
  primary-action-bg: "#4C7939"
  primary-action-bg-dark: "#467034"
  primary-outline-text: "#4C7939"
  primary-outline-text-dark: "#74B85C"
  secondary: "#3B8FC2"
  secondary-action-bg: "#2A678C"
  secondary-action-bg-dark: "#235674"
  secondary-outline-text: "#2A678C"
  secondary-outline-text-dark: "#56A6D6"
  tertiary: "#8C3A3A"
  tertiary-darken: "#652A2A"
  # Copper's base is already AA-safe as text-on-white / white-on-fill in light
  # theme; dark theme still needs its own darker/lighter pair (see -dark).
  tertiary-action-bg: "#8C3A3A"
  tertiary-action-bg-dark: "#834040"
  tertiary-outline-text: "#8C3A3A"
  tertiary-outline-text-dark: "#D58A8A"
  slate: "#5B6470"
  # On-fill inks. Action fills are deep in BOTH themes, so on-accent is white
  # in light and the off-white ink in dark (never #15201A on a deep fill).
  # Status-hue fills (info/warning/slate chips) LIFT in dark, so their text
  # flips to near-black via the separate on-status slot.
  on-accent: "#FFFFFF"
  on-status: "#FFFFFF"
  # Status hues as AA-safe small text: -darken stop in light, lifted base in dark.
  success-text: "#235C18"
  warning-text: "#8F6007"
  # Semantic status (own slots — error is a dedicated bright red, distinct from tertiary copper)
  info: "#2B6CB0"
  success: "#3D8B2E"
  warning: "#C98B0D"
  error: "#C1423A"
  error-action-bg: "#882B25"
  error-action-bg-dark: "#9E332C"
  # Surfaces & inks (light)
  canvas: "#F6F8F5"
  surface: "#FFFFFF"
  surface-2: "#EEF1EC"
  surface-sunken: "#E9EFE7"
  code-surface: "#EEF1EC"
  on-surface: "#0F1410"
  on-surface-muted: "#4D544A"
  on-surface-faint: "#676F64"
  on-surface-disabled: "rgba(15, 20, 16, 0.38)"
  # Borders & lines (light)
  divider: "#EEF1EC"
  border: "#DDE4D9"
  border-strong: "#C6CEC2"
  border-green: "#DEEAD6"
  # Interaction tints
  hover-tint: "color-mix(in srgb, #6AA84F 10%, transparent)"
  row-draft: "color-mix(in srgb, #6AA84F 10%, transparent)"
  row-edit: "color-mix(in srgb, #3B8FC2 9%, transparent)"
  focus-ring: "#3B8FC2"
  overlay: "rgba(33, 33, 33, 0.498)"
  # Dark theme counterparts (apply when [data-theme="dark"])
  canvas-dark: "#32333D"
  surface-dark: "#37373F"
  surface-2-dark: "#2B2C34"
  on-surface-dark: "#E6E9E4"
  on-surface-muted-dark: "#C0C3BE"
  border-dark: "#474B44"
  primary-dark: "#74B85C"
  secondary-dark: "#56A6D6"
  tertiary-dark: "#C26B6B"
  error-dark: "#D9706A"
  on-accent-dark: "#E6E9E4"
  on-status-dark: "#15201A"
  success-text-dark: "#5FB84A"
  warning-text-dark: "#DDA02E"
typography:
  display:
    fontFamily: Roboto
    fontSize: 39px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.02em
  page-title:
    fontFamily: Roboto
    fontSize: 31px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.015em
  section-title:
    fontFamily: Roboto
    fontSize: 25px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.005em
  panel-title:
    fontFamily: Roboto
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.3
  group-label:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0.01em
  micro-heading:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.45
    letterSpacing: 0.02em
  lead:
    fontFamily: Roboto
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-small:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4286
    letterSpacing: 0.01em
    fontFeature: "'tnum' 1"
  body-small-medium:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.01em
    fontFeature: "'tnum' 1"
  caption:
    fontFamily: Roboto
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: 0.02em
    fontFeature: "'tnum' 1"
  label:
    fontFamily: Roboto
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0.07em
  # A type role, not a license for a stat-card dashboard. Use it for a count
  # that is live, traceable to a real record set, and secondary to the page's
  # real content. Never for invented values. See Do's and Don'ts.
  metric:
    fontFamily: Roboto
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1
    letterSpacing: -0.02em
    fontFeature: "'tnum' 1"
  button:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.01em
  code-inline:
    fontFamily: Consolas
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    fontFeature: "'zero' 1"
  code-block:
    fontFamily: Consolas
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.7
    fontFeature: "'zero' 1"
rounded:
  sm: 3px
  md: 4px
  lg: 8px
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  panel-padding: 16px
  cell-pad-x: 16px
  cell-pad-y: 6px
  row-dense: 36px
  row: 44px
  # Grid density tiers (Settings-level global preference; see Layout)
  row-comfortable: 44px
  row-cozy: 38px
  row-compact: 32px
  appbar-height: 56px
  drawer-width: 240px
  content-max-width: 1600px
  reading-max-width: 760px
  form-max-width: 560px
  toolbar-search-max: 360px
components:
  button-primary:
    backgroundColor: "{colors.primary-action-bg}"
    textColor: "{colors.on-accent}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 36px
  button-primary-hover:
    backgroundColor: "#3C5F2E"
  button-outlined:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary-outline-text}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 36px
  button-outlined-hover:
    backgroundColor: "{colors.hover-tint}"
  button-destructive:
    backgroundColor: "{colors.tertiary-action-bg}"
    textColor: "{colors.on-accent}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 36px
  button-destructive-hover:
    backgroundColor: "{colors.tertiary-darken}"
  icon-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface-muted}"
    rounded: "{rounded.full}"
    size: 36px
  input-field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-small}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 40px
  chip-soft:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-primary-surface}"
    typography: "{typography.caption}"
    rounded: "{rounded.full}"
    padding: 2px 10px
    height: 24px
  chip-selected:
    backgroundColor: "{colors.primary-action-bg}"
    textColor: "{colors.on-accent}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.panel-padding}"
  dialog:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  table-header:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface-faint}"
    typography: "{typography.label}"
    height: 40px
  table-row:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-small}"
    height: "{spacing.row-dense}"
  table-row-hover:
    backgroundColor: "{colors.hover-tint}"
  app-bar:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-primary-surface}"
    height: "{spacing.appbar-height}"
  nav-item-active:
    backgroundColor: "{colors.primary-surface}"
    textColor: "{colors.on-primary-surface}"
    typography: "{typography.body-small-medium}"
    rounded: "{rounded.md}"
  code-block:
    backgroundColor: "{colors.code-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.code-block}"
    rounded: "{rounded.md}"
    padding: 16px 18px
  keycap:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.code-inline}"
    rounded: "{rounded.md}"
    padding: 1px 7px
---

# AHKFlow Design System

## Overview

AHKFlow is an open-source **AutoHotkey V2 hotstring manager & CLI** for Windows: users define hotstrings and hotkeys once, organize them by profile and category, and download valid `.ahk` scripts through a Blazor WebAssembly web app or the `ahkflow` CLI.

It is a **dense, spreadsheet-first productivity tool** — not a marketing site. Users are Windows automation enthusiasts working in long daily sessions on large datasets. Design priorities, in order: **(1)** efficient reading and inline management of many rows, **(2)** readability and accessibility (high contrast), **(3)** aesthetics. Desktop-primary, mobile-friendly.

The visual language is nature-inspired — green, blue, and copper retinted from a spring-river photo. **"Flow"** evokes a calm typing flow-state and river-like rhythm, expressed subtly through spacing, hairline dividers, and quiet motion — never literal illustration. Target feel: *"Airtable meets Notion tables meets Anthropic minimalism, with enterprise productivity density."*

The system is a **tweaked MudBlazor 9.x theme**: every token compiles back into a `MudTheme` (`PaletteLight`/`PaletteDark`, `Typography`, `Shadows`, `LayoutProperties`, `ZIndex`) plus a thin CSS layer for the code role MudBlazor has no slot for. The MudBlazor Default Baseline (v9.4) is authoritative for every foundation value AHKFlow does not override.

Voice is **calm, utilitarian, concise**: sentence case everywhere (buttons included — "Add", "Reload", "Delete 3 selected"), UPPERCASE only for column headers, field labels, and eyebrows. No hype, no emoji in product chrome.

## Colors

The palette is nature-derived, low-saturation, and calm. Light theme is canonical; the tokens above carry `-dark` suffixed counterparts for the dark theme (applied via `[data-theme="dark"]`).

- **Primary — brand green (#6AA84F):** main CTAs, links, success accents, the "AHK" wordmark. Hover/pressed darken to #4C7939. A pale green wash (`primary-surface`, #EEF7E9) is the one canonical brand tint — used identically for the app-bar chrome and the active nav pill.
- **Secondary — flow blue (#3B8FC2):** secondary actions, the "flow" wordmark, row-edit tint, and the **focus ring** color.
- **Tertiary — copper red (#8C3A3A):** destructive *component* actions the user chooses — Delete buttons, delete icon buttons, error-state chips, validation borders. Warm and intentional, not alarming.
- **Error — bright red (#C1423A):** reserved for real *error messages* the system reports — error alerts, error toasts, RFC 9457 ProblemDetails banners. Never used for user-chosen destructive buttons.
- **Semantic status:** info #2B6CB0, success #3D8B2E, warning #C98B0D — each its own slot, never remapped from brand hues.
- **Filled-button-safe tones:** the raw brand anchors (#6AA84F, #3B8FC2) don't clear WCAG AA against white text at button sizes, and dark theme's lifted ramp makes it worse. Filled buttons and outlined/text-button labels use dedicated darker "action" tones instead (#4C7939 primary / #2A678C secondary in light; #467034 / #235674 for filled backgrounds in dark, where outlined text instead keeps the lifted base since that already reads fine on a dark canvas). The same rule covers every green-filled element — count badges, checkmark fills, FABs, power toggles — never raw #6AA84F under light text.
- **On-fill inks:** text on filled *action* fills is `on-accent` — white in light, off-white ink #E6E9E4 in dark (the dark action fills stay deep, so light text is what clears AA). Filled *status-hue* chips (info/warning/slate) lift to mid tones in dark and flip to near-black `on-status` #15201A instead. Status hues used as small text on surfaces take the dedicated text-safe pair `success-text`/`warning-text`: the -darken stop in light, the lifted base in dark.
- **Neutrals:** a green-grey neutral ramp underpins everything. Light canvas is river-pale #F6F8F5 with pure-white surfaces; ink is near-black #0F1410 (≈17.3:1 on canvas). Dark theme uses MudBlazor's neutral dark grays (#32333D canvas / #37373F surface) with **off-white ink #E6E9E4 — never pure white** (it haloes). Brand accents lift slightly in dark (green → #74B85C, blue → #56A6D6, copper → #C26B6B).
- **Slate (#5B6470):** the sixth swatch hue for profile/entity color coding, alongside green, blue, copper, info-blue, and warning-amber.

**Copper vs. red rule of thumb:** if the *user chooses* the action (delete, remove, clear) → copper. If the *system reports* a failure → red.

## Typography

Two families only: **Roboto** for all reading text and headings, **Consolas** for code (inline, CLI blocks, keycaps). The brand wordmark is a fixed vector asset — never re-typeset from a font.

- **Scale:** Major Third (1.25) above body; hand-tuned 16/14/12 core below. Headings read as clear level changes without stealing viewport from data rows.
- **body-small (14px) is the workhorse** — grid cells, tables, and most of the app are set there, not 16px. Body prose never drops below 16px; 12px caption is the content floor.
- **Numerals:** tabular figures (`tnum`) in grids, counts, and timestamps so columns align; proportional in running prose. **Slashed zero** (`zero`) in all code so `0` never reads as `O`.
- **Labels/overlines** (12px, 600, +0.07em) are strictly UPPERCASE — column headers, field labels, eyebrows.
- **Buttons** are 14px medium with `text-transform: none` (sentence case).
- Headings step down below 600px viewports (display 39→30, page-title 31→26, section-title 25→21); body sizes hold. Editable inputs lift to 16px on mobile to prevent iOS zoom.

## Layout

Desktop-first app shell: a **56px app bar** (z-index 1300) with the brand corner, and a **collapsible drawer** (z 1100; ~240px expanded, measured to its widest item; 200px overlay drawer on mobile) holding sectioned nav (**Editor / Scripts / System**). Content scrolls under the sticky shell, max width 1600px.

The app bar accepts five light-theme **plate treatments** — mist · sage · fern · green · white. The pale green wash (`primary-surface`) remains the canonical brand treatment; the UI kit currently defaults to the white plate. Dark theme always uses the dark chrome.

- **Rhythm:** a strict **4px base unit** governs padding, gaps, and row heights.
- **Density:** grids ship three user-selectable tiers, set once in Settings and applied to every grid — **Comfortable 44px** (default), **Cozy 38px**, **Compact 32px** rows. Header text never drops below the 12px floor at any tier. Minimum mobile hit target is 44px; sub-44px icon controls expand their touch area to 44px on coarse pointers without changing visual size. Cell padding is 16px horizontal, 6px vertical at the default tier. (The generic Table primitive keeps a single 36px `dense` mode.)
- **Canonical page:** a single 16px-padded paper wrapping toolbar + grid. Toolbar pattern: primary action (Add) + secondary (Reload) on the left, spacer, search on the right (max 360px).
- **Page header:** every page opens with one baseline row — the page title plus its live count or status chips — then a 14px gap to the content. Home uses the same row with the slogan ("AutoHotkey V2 hotstring manager & CLI", 18px, brand action tone) as its subtitle. No page invents its own header.
- **Width tiers:** every page uses exactly one of three left-anchored widths — `content-max` 1600px (data grids, Home, Downloads, Profiles), `reading-max` 760px (Health, Changelog), `form-max` 560px (Settings). All tiers share the same left origin; narrow pages are never centered.
- **Z-index ladder** (MudBlazor): drawer 1100 · popover 1200 · appbar 1300 · dialog 1400 · snackbar 1500 · tooltip 1600.

## Elevation & Depth

Backgrounds are **flat**: tinted canvas + flat white surfaces. No gradients, no photographic backgrounds, no textures, no glassmorphism.

Surface depth maps to the **MudBlazor elevation ramp (0/1/2/4/8)** — never arbitrary box-shadows. Shadows are soft, neutral, low-contrast in light; deeper in dark:

- Elevation 1: `0 1px 2px rgba(15,20,16,0.10), 0 1px 3px rgba(15,20,16,0.06)`
- Elevation 2: `0 2px 4px rgba(15,20,16,0.10), 0 3px 6px rgba(15,20,16,0.07)`
- Elevation 4: `0 4px 10px rgba(15,20,16,0.11), 0 8px 18px rgba(15,20,16,0.08)`
- Elevation 8: `0 8px 22px rgba(15,20,16,0.14), 0 16px 38px rgba(15,20,16,0.10)`

Flat/outlined cards use a 1px green-grey border (#DDE4D9) instead of a shadow. Two border tiers share one hue: `divider` for faint in-card hairlines, `border` for structural edges. Dialog overlays use a ~50% dark scrim; that and low-alpha hover tints are the only transparency.

## Shapes

MudBlazor default **4px radius** everywhere: buttons, inputs, paper, chips, code blocks. **3px** for inline code, **8px** for dialogs and popovers, **pill (9999px)** for filter chips and badges. Never mix arbitrary radii; icon buttons are circular.

Iconography is **Material Symbols (Outlined)** — `FILL 0, wght 400`, tracking the Roboto body weight. No custom icon font. Canonical names: Home `home`, Hotstrings `abc`, Hotkeys `keyboard`, Downloads `download`, Profiles `group`, Categories `label`, Health `monitor_heart`, Recycle Bin `restore_from_trash`, Settings `settings`, Changelog `history`; actions Add `add`, Reload `refresh`, Edit `edit`, Delete `delete`, Bulk delete `delete_sweep`, Commit `check`, Cancel `close`, Save `save`, Search `search`.

## Components

### Buttons

Filled primary (green, white text, darkens on hover/press), outlined (neutral border via `currentColor`, green-dark text, brand-soft hover tint), and text variants. Filled and outlined labels use the AA-safe action tone (#4C7939), not the raw brand swatch (#6AA84F) — see Colors. Four color slots: primary, secondary, **tertiary (copper) — the destructive color for user-chosen actions** (Delete, Remove), and error (bright red, reserved for system-reported failures — never a plain delete button). Sizes: small 30px, medium 36px (default), large 42px. Sentence case, 14px medium.

### Chips & tags

System-wide convention: **deselected = soft tone, selected = filled solid with on-fill text** — the selected fill uses the hue's AA-safe action tone (green fills with #4C7939, never the raw #6AA84F swatch, whose white-text contrast is only 2.9:1), and the text is `on-accent` for the brand hues and `on-status` for the status hues (which flip to near-black in dark — see Colors). Chips accept semantic aliases and six raw swatch hues (green/blue/copper/info/warning/slate). Outlined chips are quiet bordered tags used for profile tags. Filter chips may carry a trailing match-count badge and a clear (×).

**Table chip overflow (`ChipOverflow`).** In grid cells that carry a *set* of chips (Profiles, Categories), a row must stay **one line tall and scannable** no matter how many values it holds. `ChipOverflow` renders the first value (`max` defaults to 1) as a normal chip and collapses the remainder into a dashed neutral **"+N" pill**; hovering the pill (or tapping, on touch — the tap pins it open until an outside click) reveals the hidden chips in a small popover above the cell. The visible chip is the row's **first-assigned** value, not alphabetical, so it doesn't jump around while editing. Zero values render a muted em-dash (`—`), never an empty cell; the Profiles column's all-profiles state keeps its dedicated "Any" chip instead. The full uncapped set still shows inside the editor and mobile detail. Never wrap chips to a second line inside a data row.

**Multi-select trigger label.** The shared `ProfileSelect` / `CategorySelect` dropdowns summarise their selection in the closed trigger as: **none →** the muted placeholder (`Any profile` / `No category`), **exactly one →** that value's name, **more than one → "N selected"**. This is structural — the label can never truncate to `App Lau…` in a narrow column. Selecting an option keeps the dropdown **open** (it's a multi-select); it closes only on an outside click or the trigger.

### Hotstring kinds & Type chip

Every hotstring has a **kind** (repo enum `HotstringKind`) — one of four, shown in the grid's **Type** column via `HotstringKindChip`:

- **Text** — a literal replacement (the default). The dominant kind, so it renders **quiet**: a neutral surface-2 / ink-muted chip with no hue, keeping the grid calm so only the special kinds draw the eye.
- **Date & time** — inserts the current date/time from a chosen format, optionally offset. Teal tint.
- **Macro** — a scripted sequence with `{{cursor}}` / `{{key:Enter}}` / `{{key:Tab}}` tokens. Magenta tint.
- **Raw** — a verbatim AutoHotkey V2 definition, parsed for its trigger and options. Amber tint, **always with a warning glyph** and the accessible warning *"Verbatim AutoHotkey definition — review before running."* — a syntax error in a Raw definition can break the whole profile script.

The special-kind hues are a deliberate data wheel kept **clear of the brand triad**: teal (oklch H 200), magenta (H 350), amber (H 70) for Date & time, Macro, and Raw (Text carries no hue). Each renders as a soft tint (`color-mix(in oklch, surface 84%, hue)` background, `mix 35% ink` text) so light/dark track without a dark-mode selector. These are *data* chips — never selectable, never filled solid like the category filter chips. **Text always renders quiet** (neutral, no hue); Date & time, Macro, and Raw carry their soft tint. Raw always keeps its warning glyph.

**Option-glyph legend.** Trigger options ride as faint monospace glyphs after the Type chip, decoded in the Type column header's help tooltip: `* = expands immediately · ? = triggers inside words · C = case sensitive · O = omits ending character · window icon = only in a specific app · clipboard icon = pasted via clipboard`.

**Type filter.** A `Type` select (All / Text / Date & time / Macro / Raw) sits in the toolbar beside the category filter chips, narrowing the grid by kind independently of the category chips.

### Version history

Every hotstring keeps a **version history**. The grid row's **History** action (a `history` icon between Edit and Delete) opens the **history dialog**: a left column of version buttons — `v3 Edit`, `v2 Restore`, `v1 Delete` — each tagged with its **change type** (`Edit` / `Delete` / `Restore`, the repo `HistoryChangeType` enum, colored blue / copper / green with a matching glyph), and a right pane previewing the selected version's snapshot (Trigger, Replacement or Format, Description, profile + category counts) with a **Revert** button. Reverting replaces the current record with that snapshot and toasts confirmation. Newest version first; the newest is selected on open.

### The hotstring editor

Non-Text kinds and any **change-type** action route to the full-page **kind-aware editor** (`HotstringEditorSurface`) rather than the inline row — Text stays inline for quick trigger/replacement edits. When an inline edit's Type select routes to the editor, the jump is announced with an info toast and is **reversible**: cancelling the editor restores the inline row edit with its in-progress values intact. The editor opens as a full-screen overlay from the grid and as a standalone page in the `hotstring-editor` template. It leads with a **kind toggle** (segmented Text · Date & time · Macro · Raw), then swaps the middle of the form per kind: Text shows a Delivery select (Auto / Hotstring / Clipboard); Date & time shows format presets + optional offset and a live preview (no replacement); Macro shows an insert-token toolbar (`{{cursor}}` / `{{key:Enter}}` / `{{key:Tab}}`); Raw shows a verbatim-definition textarea with a warning banner, an Examples panel, and a parsed trigger/options summary. Shared across kinds: a **Generated AutoHotkey code** panel, Description, Apply-to-all / Profiles, Trigger options (Omit ending disabled under Expand immediately), Window context, and Categories.

### Recycle Bin

Deleting a hotstring or hotkey moves it to the **Recycle Bin** (a System-section nav page), not oblivion. The bin lists **both types together** in one table — **Type** (a Hotstring/Hotkey chip), **Name** (the trigger, or the key combo as keycaps), **Details** (replacement or description), and **Deleted** (when) — with two per-row actions: **Restore** (green, returns the item to its live list) and **Delete forever** (red, confirmed — it does *not* return to the bin). A single **Reload** sits in the toolbar; the empty state reads "The recycle bin is empty." On mobile the table collapses to cards. Backed by the repo `DeletedHotstringDto` / `DeletedHotkeyDto`.

### Inputs

White surface, 1px #C6CEC2 rest border, 4px radius, 40px height, 14px text. Focus swaps the border to flow blue plus a blue focus ring (`0 0 0 2px canvas, 0 0 0 4px #3B8FC2`). Validation errors use copper borders/labels inline after a commit attempt.

### Data grids & tables

The heart of the product. 40px UPPERCASE label header row, 36px dense body rows, hairline row lines (`rgba(15,20,16,0.09)`), a 7% green hover tint, near-invisible stripe. Row states: draft rows tint green 10%, rows being edited tint blue 9%. Tabular figures throughout. Each row carries an **Enabled** toggle whose rendering is a global preference (`enabledStyle`): `switch` (default) or `power` — a round power-button that reads filled-green when on, hairline when off.

### Feedback

Toasts are short past-tense confirmations ("Hotstring created.") queued in a stack of up to 3, positioned to never overlap the mobile FAB; toasts and snackbars use a plain 1px border with the severity icon — never a colored side-stripe. Alerts render RFC 9457 `title` + `detail` cleanly, and can carry an inline remedy at the right edge (`action` — e.g. a Log in button beside "You are not signed in."). Empty states distinguish truly-empty from filtered-empty: "No hotstrings yet. Add one to get started." when the dataset is empty, "No hotstrings match your search." when a search hides everything, "No hotstrings match the active filters." when facet filters do.

### Signed-out states

Being signed out is a **fact, not a failure** — it is always **info** severity. Warning is reserved for session expiry ("Your session expired. Log in again to continue."), error for a failed sign-in attempt only. The canonical string is "You are not signed in." — sentence case, period, never "Please log in".

- **Chrome stays.** The nav rail, app bar, and page titles always render; a signed-out user can explore the full product layout.
- **Data pages gate.** Hotstrings, Hotkeys, Downloads, Profiles, Categories, and Settings replace their page body with the **SignInGate**: icon ring + "You are not signed in." + one sentence of what signing in unlocks + a filled Log in button. Never render disabled toolbars or fake-empty grids — "No hotstrings yet." is a lie when the truth is "we don't know". Match the gate's `minHeight` roughly to the body it replaces to limit layout shift on login. Settings gates because its preferences are account-scoped (theme is persisted server-side); a signed-out user has no preferences to show or save.
- **Home never gates.** The hero and CLI quickstart are the product pitch; signed-out adds an info alert with an inline Log in action, and stat values render the "—" data placeholder — never a false 0.
- **App bar auth chrome:** signed out shows an outlined Log in button; signed in shows the greeting plus an initials avatar opening the account menu (name/email header, Settings, Sign out).
- **Feedback moments:** signing in shows a full-canvas centered indeterminate progress with "Signing you in…"; sign-in and sign-out each confirm with a success toast ("Signed in as …." / "Signed out.").

### Code & keycaps

Inline code and CLI blocks are Consolas on the code surface with a load-bearing 1px border (the fill can match a panel background, so the border provides the contrast — never fake it by swapping the background). Key combos render as bordered keycaps with a 1px drop edge.

### Motion

Calm and river-like: 120–300ms, `cubic-bezier(0.4,0,0.2,1)`, fades and gentle slides. Hover = subtle tint or darker fill; press = darker fill; disabled = reduced opacity, no pointer events. **No bounce, no infinite decorative loops.** Animate `transform`/`opacity`, not layout properties. `prefers-reduced-motion: reduce` collapses every duration to effectively instant (a global guard in the tokens covers components that set literal durations).

## Voice & tone

Calm, utilitarian, concise — a tool for experienced daily users, never marketing.

- **Voice:** plain, direct, operational. No hype, no exclamation, no hand-holding for obvious controls — e.g. "Define them once, organize them by profile, and download a valid `.ahk` script."
- **Person:** addresses the user as **"you"** ("Manage your AutoHotkey hotstrings…"); the product refers to itself as **AHKFlow** (product) / `AHKFlowApp` (solution).
- **Casing:** sentence case for body, labels, and buttons (`text-transform: none` — "Add", "Reload", "Delete 3 selected"). Column headers, field labels, and eyebrows are UPPERCASE — the label/overline role, see Typography.
- **Microcopy patterns (verbatim from the app):**
  - Toasts: short past-tense confirmations — "Hotstring created." · "Hotstring updated." · "Settings saved."
  - Search placeholder: "Search For Hotstrings".
  - Destructive confirm: title "Delete hotstring?", body `Delete "{trigger}"? This cannot be undone.`, confirm button "Delete".
  - Empty states, truly empty: "No hotstrings yet. Add one to get started." · "No categories yet. Add one to get started." · "No profiles yet. Add one to get started."
  - Empty states, filtered: "No hotstrings match your search." · "No hotstrings match the active filters." · `No profiles match "{search}".` · "No categories in this scope."
  - Bulk delete: button "Delete {n} selected"; confirm body "Delete {n} hotstrings? This cannot be undone." (properly pluralized, never "(s)").
  - Blocked action: name the rule, then the remedy: "Can't delete the default profile. Set another as default first." Warning severity, raised on activation (see Do's and Don'ts).
  - Validation: "Trigger is required" · "Replacement is required" · "Name is required".
  - Not-signed-in: "You are not signed in."
- **Punctuation:** no em dashes in UI copy — use commas, colons, semicolons, or periods. The "—" glyph may appear only as an empty-cell data placeholder.
- **Slogan (final):** **"AutoHotkey V2 hotstring manager & CLI."**
- **Errors:** backend returns RFC 9457 ProblemDetails → render `title` + `detail` cleanly. Field-level validation is inline on the input after a commit attempt; request-level errors go to a Snackbar or an inline alert.
- **Destructive color:** follows the same user-chose vs. system-reported split as Colors — copper for buttons the user picks, bright red only for errors the system reports. See the copper-vs-red rule above.
- **Emoji:** not used in product chrome. Unicode glyphs appear only as content (e.g. the `→` in a hotstring replacement, the `>`/`_` prompt in the logo).
- **Sample data:** mockups use neutral, clearly-fake placeholders ("Sam Rivers", `sam@example.com`) — never real user data.

## Accessibility contract

WCAG 2.2 AA is the committed floor (PRODUCT.md). The React design-system kit is a **visual specification**: it demonstrates look, layout, and copy, while full keyboard and assistive-technology support ships in the MudBlazor Blazor app before release — MudBlazor components provide native keyboard operability, roles, and focus management out of the box. This section is the contract the app implementation must satisfy (and the kit follows where cheap):

- **Contrast:** ≥4.5:1 body/small text, ≥3:1 large text and UI components, in **both** themes. Use the action tones and on-fill inks from Colors; never raw brand hues under light text.
- **Focus:** every interactive element shows the flow-blue focus ring on `:focus-visible` (`0 0 0 2px canvas, 0 0 0 4px #3B8FC2`; that hex is light theme — the ring uses the theme blue token, so it lifts to `#56A6D6` in dark). Never suppress `outline` without applying the ring. One shared rule in the tokens applies it globally.
- **Names:** icon-only buttons always carry an `aria-label` (and a tooltip); a decorative tooltip never substitutes for an accessible name.
- **Controls:** interactive elements are native `<button>`/`<input>`/`<select>` or carry the full ARIA pattern (role, state, `tabindex`, keyboard handlers). Checkboxes, switches, radios, selects, sortable headers (`aria-sort`), and facet rows must be keyboard-operable.
- **Overlays:** dialogs trap focus, close on Escape, and return focus to the trigger; popovers and menus close on Escape; triggers expose `aria-expanded`.
- **Structure:** real headings (`<h1>`–`<h3>`) behind the title roles; nav landmarks with `aria-label` and `aria-current`; toast live-region mounted persistently so announcements aren't missed; progress elements carry `progressbar` semantics.
- **Motion:** `prefers-reduced-motion` collapses all durations (implemented in tokens).
- **Touch:** ≥44px hit targets on coarse pointers (the `.ahk-hit` helper expands smaller icon controls).
- **Text:** never below the 12px floor; editable inputs ≥16px on mobile (iOS zoom).

## Do's and Don'ts

- Do use copper for user-chosen destructive actions and bright red only for system-reported errors — never swap them.
- Do set grids, counts, and timestamps in tabular figures, and all code with slashed zeros.
- Do keep body-small (14px) as the data workhorse; never drop content below 12px, and never set prose below 16px.
- Do use the elevation ramp (0/1/2/4/8) or a 1px border for depth — never arbitrary box-shadows.
- Do use the darker "action" tone (not the raw brand swatch) for filled-button text/backgrounds — the raw swatch fails WCAG AA at button sizes.
- Do use the brand asset files for the logo/wordmark — never re-typeset it from a font.
- Do write sentence case everywhere, UPPERCASE only for the label/overline role.
- Do give every interactive element the flow-blue `:focus-visible` ring — never suppress outline without it.
- Don't build a stat-card dashboard. The `metric` type role sets a large number; it does not sanction a grid of identical metric cards, which PRODUCT.md anti-references as the SaaS-dashboard cliché. A count may appear only when it is live, traceable to a record set the user can open, and secondary to the page's real content. Never invent a number, a timestamp, or an activity feed to fill a landing page.
- Don't disable a control whose only explanation is a tooltip. `disabled` carries `pointer-events: none` (see Motion), so the tooltip never reaches a pointer user — screen readers still read the `aria-label`, leaving the sighted mouse user the one stranded. When a rule blocks an action, keep the control enabled and explain on activation with a warning toast naming the rule and the remedy. Model: the Categories orphan-guard.
- Don't use pure white text on dark surfaces — ink is off-white #E6E9E4 (this includes text on filled buttons: dark `on-accent` is #E6E9E4).
- Don't use gradients, photographic backgrounds, textures, glassmorphism, or backdrop blur.
- Don't use emoji in product chrome; Unicode glyphs appear only as user content.
- Don't add bounce or infinite decorative animation; motion stays 120–300ms and eased.
- Don't invent new green tints — layer `primary-surface`, `on-primary-surface`, and `border-green` instead.
- Don't let the primary green appear as more than one filled CTA per toolbar; secondary actions are outlined or text.
