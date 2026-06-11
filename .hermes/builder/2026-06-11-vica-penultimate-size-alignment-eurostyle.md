# VICA page: restore penultimate size/alignment and keep Eurostyle logo

- Timestamp (UTC): 2026-06-11T22:05:00Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `vica/index.html`

## What changed
- Rebased `vica/index.html` to the penultimate layout/version while keeping the requested font behavior:
  - Restored the existing small, top-aligned logo link sizing/alignment (from the one-before-last revision of this page).
  - Kept `MARES ENGINEERING` as the top navigation link to `../index.html` with no bottom “back to ...” links.
- Applied the homepage display font stack to the VICA logo text:
  - `--display-font: 'Mares Display', 'Eurostile Extended Black', 'Eurostyle Extended Black', 'Arial Black', 'Trebuchet MS', 'Franklin Gothic Demi Cond', sans-serif;`
  - Added matching `@font-face` for `Mares Display` at `../assets/fonts/eurostile-extended-black.woff2`.

## Commands run
- `git checkout 5538933 -- vica/index.html`
- `git diff 5538933 -- vica/index.html` (then applied a focused font change)
- `git add vica/index.html`
- `git diff --check --cached -- vica/index.html`

## Validation
- Verified top brand link remains and bottom back links are absent via content search.
- `git diff --check --cached -- vica/index.html` returned no whitespace issues.
