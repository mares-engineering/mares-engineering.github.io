# VICA brand beveling refined to homepage style

- Timestamp (UTC): 2026-06-11T23:20:10Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `vica/index.html`

## What changed
- The top `MARES ENGINEERING` logo link in `vica/index.html` was updated to restore the homepage-like bevel/glow behavior while preserving the small compact size and top-aligned placement.
- Added homepage-style glow layers to the brand link via:
  - `::before` + `::after` on `.brand-link`
  - same radial-gradient blur profile as `index.html` for the halo stack
- Kept size/position intent:
  - `font-size: 0.72rem` on `.brand`
  - top-of-page compact alignment in `.page`
  - no underline (`text-decoration: none`) on the linked logo.

## Commands run
- `git diff --check -- vica/index.html`
- `git diff -- vica/index.html`
- `date -u +"%Y-%m-%dT%H:%M:%SZ"`

## Notes
- `git status --short` confirmed only `vica/index.html` changed before commit.
