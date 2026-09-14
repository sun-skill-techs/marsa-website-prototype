# agents.md — MARSA Gifting
_Static responsive coming-soon landing page._

## File Map
- `index.html` — semantic page structure: header, hero copy/logo, gift art, footer.
- `styles.css` — all typography, layout, responsive breakpoints, and CSS gift illustration.
- `assets/Logo Design 1.svg` — displayed MARSA Gifting logo.

## Typography and Palette
- Sans: `DM Sans`; display: `Playfair Display`.
- `h1` is the serif hero display; `.header__label`, `.hero__note`, `.art__caption`, and `.footer` share uppercase tracking.
- Colors are direct values in `styles.css`; no token layer exists.

## Layout
- Desktop `.hero` is a two-column grid; `.hero__copy` owns its horizontal padding.
- At `max-width: 850px`, `.hero__copy` becomes `display: contents` and the logo/content use grid rows.
- Smaller width and height media queries refine the mobile layout.

## Change Guide
| Task | File(s) to edit |
|---|---|
| Change page markup/copy | `index.html` |
| Change desktop layout or visual styling | `styles.css` base rules |
| Change mobile layout | `styles.css` media queries |
| Replace branding artwork | `assets/Logo Design 1.svg` |

## Gotchas
- Preserve mobile rules when making desktop-only changes: they rely on `.logo-wrap` overrides at `max-width: 850px` and below.
- The SVG viewBox includes whitespace, so its visible artwork may not coincide with the `.logo-wrap` edge.
- Preview with `python3 -m http.server 8000`.

## Maintaining this file

Keep this file for knowledge useful to almost every future agent session in this project.
Do not repeat what the codebase already shows; point to the authoritative file or command instead.
Prefer rewriting or pruning existing entries over appending new ones.
When updating this file, preserve this bar for all agents and keep entries concise.
