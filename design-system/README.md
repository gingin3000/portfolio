# Aurora Design System

A framework-agnostic CSS design system with a distinctive glass-and-aurora aesthetic:
a blue-forward semantic palette, Wix Madefor type, a 4px spacing grid, and full
light/dark theming with a signature staggered cross-fade.

No build step, no dependencies. Just CSS custom properties and a handful of component
classes. Works in any framework or in plain HTML.

## Quick start

```html
<link rel="stylesheet" href="design-system.css">

<button class="ds-button">Send message</button>
<span class="ds-chip">Design tokens</span>
```

Toggle themes by setting an attribute on the root element:

```js
document.documentElement.setAttribute('data-theme', 'dark'); // or 'light'
```

**Living style guide:** open [`docs/index.html`](docs/index.html) in a browser to browse
every token and component, and to see the theme cross-fade in action.

## Architecture

Tokens are layered so you theme by remapping, never by editing components.

```
Primitives   raw tonal ramps (the only hex values)   tokens/primitives.css
    │
Semantic     role aliases → primitives (theme here)   tokens/semantic.css
    │
Foundations  spacing, radius, elevation, type scale   tokens/foundations.css
    │
Components   consume semantic tokens only             components/*.css
```

```
design-system/
├── design-system.css        ← single entrypoint (@imports everything, in order)
├── tokens/
│   ├── fonts.css            external font @imports (swap for self-hosted here)
│   ├── primitives.css       blue/red/orange/green/grey ramps + alpha
│   ├── semantic.css         primary/secondary/status/surface/text roles (light + dark)
│   └── foundations.css      spacing · radius · elevation · type scale · icon axes
├── components/
│   ├── effects.css          glass/glow/aurora helper tokens + keyframes
│   ├── base.css             element defaults, focus ring, type utilities, cross-fade
│   ├── icon.css             .ds-icon (Material Symbols Rounded)
│   ├── button.css           .ds-button (primary/secondary/ghost/sm) + .ds-cta
│   ├── card.css             .ds-surface · .ds-card · .ds-media
│   ├── field.css            .ds-field (input/textarea, error state)
│   ├── chip.css             .ds-chip · .ds-badge--{role}
│   └── nav.css              .ds-nav floating pill
└── docs/
    └── index.html           living style guide
```

## Tokens at a glance

### Semantic colour roles
Each role comes in `main`, and where relevant `container` / `on-container` /
`contrast-text` pairs, for: **primary, secondary, error, warning, info, success,
neutral, promotional**. Plus surface (`--surface-default`, `--surface-inverse`,
`--background-default`, `--background-highlight`), text (`--text-display / primary /
secondary / disabled / on-inverse`), and line roles (`--divider-*`, `--outline-*`).

All roles have dark-mode overrides under `[data-theme="dark"]`.

### Foundations
| Scale | Values |
| --- | --- |
| Spacing (4px grid) | `--space-4` → `--space-96` (4, 8, 12, 16, 20, 24, 28, 32, 48, 64, 96) |
| Radius | `--radius-8`, `--radius-12`, `--radius-24`, `--radius-full` |
| Elevation | `--elevation-1` → `--elevation-5`, `--inset-shadow-field` |
| Type | `--type-display-lg` … `--type-body-sm`, `--type-eyebrow` (use with `font:` shorthand) |
| Weights | `--fw-regular` 400 · `--fw-medium` 500 · `--fw-semibold` 600 · `--fw-bold` 700 |

### Typography
- **Headings** — Wix Madefor Display
- **Body** — Wix Madefor Text
- **Icons** — Material Symbols Rounded (variable: fill, weight, grade, optical size)

## Components

| Class | What it is |
| --- | --- |
| `.ds-button` `--secondary` `--ghost` `--sm` | Pill actions; `.ds-cta` for inline arrow links |
| `.ds-card` / `.ds-surface` / `.ds-media` | Glass card / solid surface / dashed image frame |
| `.ds-field` (`--error`) | Labelled input + textarea |
| `.ds-chip`, `.ds-badge--{role}` | Neutral pill / status-tinted badge |
| `.ds-nav`, `.ds-nav__item.is-active`, `.ds-nav__toggle` | Floating glass nav pill |
| `.ds-icon` (`--sm/lg/xl`, `--filled`) | Material Symbols icon |
| `.ds-display-lg` … `.ds-body-sm`, `.ds-eyebrow` | Typography utilities |

## Theming

The only file you edit to reskin the system is `tokens/semantic.css` — remap roles to
different primitives (or add new primitives). Components never reference hex directly.

The staggered light/dark cross-fade is opt-in per toggle: add `class="theming"` to
`<html>` on click, remove it ~2.25s later (see `base.css` and the docs page's script).
It respects `prefers-reduced-motion`.

## Provenance

Derived by analysing `tokens.css` and `index.html` from the source portfolio. The token
values are faithful to the original; this repo reorganises them into a primitive→semantic
architecture, generalises the inline styles into named components, and adds a documented
type scale, utility classes, and a living style guide.
