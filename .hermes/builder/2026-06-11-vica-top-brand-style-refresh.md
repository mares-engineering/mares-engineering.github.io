# VICA top-brand style alignment to homepage tokens

- Timestamp (UTC): 2026-06-11T23:04:38Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `vica/index.html`

## What changed
- Updated the top `MARES ENGINEERING` header element in `vica/index.html` to use the homepage-style typographic system while preserving the current compact size/position:
  - Added homepage display stack (`Mares Display`, `Eurostile`, `Eurostyle` family fallback) and `@font-face` source.
  - Applied homepage-style gradient text fill, stroke, and glow/sheen effects.
  - Kept the existing scale/placement behavior (`0.72rem` size and current top-of-page alignment in `.page`).
  - Kept text without underlining (`text-decoration: none` on the new top link).
- Preserved existing page structure and content positions otherwise.

## Validation run
- `date -u +"%Y-%m-%dT%H:%M:%SZ"`
- `git diff --check -- vica/index.html`
- `search_files ... "Mares Display|eurostile-extended-black.woff2|MARES ENGINEERING"` to confirm resources/classes present

## Residual notes
- Global style changes also refresh page background treatment and body typography tokens to align with homepage visual system.
