# Gina — Portfolio

A single-page portfolio implemented from the Claude Design file `Gina Portfolio.dc.html`, using the
Trusted Shops `trstd-core` design system (Wix Madefor type, Material Symbols icons, semantic color tokens).

## Run it

No build step. Either:

- **Open directly:** double-click `index.html`, or
- **Serve locally** (recommended, avoids any file:// quirks):
  ```sh
  cd gina-portfolio
  python3 -m http.server 8000
  # then open http://localhost:8000
  ```

An internet connection is needed the first time so the fonts load from Google Fonts.

## What's here

| File | Purpose |
| --- | --- |
| `index.html` | The whole app — markup, styles, and a small vanilla-JS state machine (no framework). |
| `tokens.css` | Design-system tokens copied from `trstd-core` (`colors_and_type.css`), with fonts pointed at the Google Fonts CDN so the site is self-contained. |
| `README.md` | This file. |

## Features (faithful to the design)

- Five views — **Home, Work, Case study, About, Contact** — swapped client-side (no page reloads).
- **Light / dark theme** toggle in the nav pill, persisted to `localStorage` under `gina-theme`.
- Animated **aurora background** with per-view blob geometry.
- Glassmorphism nav pill and work cards, glow-on-hover accents.
- Contact form with a **"Message sent"** confirmation and reset.

## Editing the content

All copy is placeholder text ready to be replaced. Everything lives in the constants near the top of the
`<script>` block in `index.html`:

- `PROJECTS` — the four Work cards (`title`, `line`, `cover`).
- `TITLES` — case-study headlines (indexed by the card that was clicked).
- `CASE_FACTS` — the Role / Timeline / Team / Platform row.
- `SKILLS` — the "Practice" chips on the About page.
- Home headline, About paragraphs, and section copy are inline in the `homeHTML()`, `aboutHTML()`,
  `caseHTML()`, and `contactHTML()` functions.

The dashed placeholder boxes (`.work-cover`, `.case-hero`, `.media`, `.portrait`) mark where images go —
swap each for an `<img>` when the real assets are ready.

## Notes

- `tokens.css` is a trimmed copy of the design system's `colors_and_type.css` — only the tokens this page
  uses were kept. If you pull in more `trstd-core` components later, replace it with the full token file.
- The original design system self-hosts the Wix Madefor TTFs; here they're loaded from Google Fonts to keep
  the project dependency-free. To fully self-host, drop the `.ttf` files into a `fonts/` folder and restore
  the `@font-face` blocks.
