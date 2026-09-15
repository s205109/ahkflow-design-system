# AHKFlow Design System

Design system and component library for **AHKFlow**, an AutoHotkey V2 hotstring manager for
Windows: 362 tokens, 45 React components, 13 page templates, light + dark, WCAG 2.2 AA floor.

**[View it live →](https://s205109.github.io/ahkflow-design-system/)**

| | |
| --- | --- |
| [Interactive web app](https://s205109.github.io/ahkflow-design-system/web-app.html) | The system in use — grids, editors, profiles, settings, light/dark |
| [Design system reference](https://s205109.github.io/ahkflow-design-system/design-system.html) | One scrollable page: color, type, spacing, every component and state |
| [DESIGN.md](DESIGN.md) | The canonical written specification |

Both HTML files are fully self-contained (fonts, CSS, and JS inlined) and open offline.
The React kit is a *visual specification*: it demonstrates look, layout, and copy, while full
keyboard and assistive-technology support ships in the production Blazor app.

## Publishing with GitHub Pages

1. Create a repo named `ahkflow-design-system` and push the contents of this folder to its root.
2. Repo → **Settings** → **Pages** → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Wait ~1 minute. The site appears at `https://s205109.github.io/ahkflow-design-system/`.
4. Replace `s205109` in the links above with your GitHub username.

GitHub cannot render HTML inline in the repo file view — it strips scripts and styles. Pages is
what makes these pages viewable.

## Rebuilding

Regenerate with the `super_inline_html` bundler from the live design-system project:

| Output | Source |
| --- | --- |
| `index.html` | `_export-cover-src.html` (edit this, not the bundle) |
| `design-system.html` | `DESIGN.html` |
| `web-app.html` | `ui_kits/web_app/index.html` |
| `DESIGN.md` | straight copy |

Re-export `web-app.html` whenever `AppShell.jsx`, a surface, or a token file changes — the bundle
embeds a compiled `_ds_bundle.js` snapshot and goes stale otherwise.
