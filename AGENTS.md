# tinytype — agent guide

Single-file HTML game (index.html). No build, no dependencies, no tests.

## Key facts

- **`index.html`** is the only source file. All CSS and JS is inline.
- Uses Web Audio API for synth sounds — no audio files.
- Timer: default 3 min, customizable via `?time=2m` / `?time=30s` / `?time=120` query param.
- Case selector (A / a / Aa) at top-right, default is uppercase.
- Deployed via GitHub Pages from `main` branch root. No build step.
- All keyboard shortcuts suppressed except Escape (fullscreen exit).

## Edit

Open `index.html` and make changes directly. No server or build needed — just refresh the browser.

## Dev preview

```bash
open index.html          # macOS
```

## Deploy

Push `main` to GitHub. Pages auto-deploys from `/` root. URL: `https://<user>.github.io/tinytype`

## Convention notes


- File is formatted with 4-space indentation (not tabs).
- No external resources — everything must be self-contained in `index.html`.
- Colors use muted, desaturated palette for toddler eye safety. Keep it soft.
