# Revert VICA page to prior visual version with Eurostyle logo font

- Timestamp (UTC): 2026-06-11T21:52:33Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `vica/index.html`

## What changed
- Reverted `vica/index.html` content to the previous page layout/style state (before the most recent "masthead small/top-aligned" adjustment):
  - Restored centered masthead layout and larger hero-style spacing.
  - Kept the page structure/content consistent with the prior VICA page version.
- Applied the homepage display font stack to VICA branding text:
  - `--display-font` now uses the homepage stack (`'Mares Display', 'Eurostile Extended Black', 'Eurostyle Extended Black', ...`).
  - Added matching `@font-face` loading for `Mares Display` from `../assets/fonts/eurostile-extended-black.woff2`.
- Left `MARES ENGINEERING` as the top link back to homepage and kept the requested bottom-navigation links removed.

## Commands run
- `git checkout 83e94f3 -- vica/index.html`
- `git diff --check -- vica/index.html`
- `date -u +"%Y-%m-%dT%H:%M:%SZ"`
- `git log --oneline --decorate -n 3`

## Validation
- `git diff --check -- vica/index.html` passed clean (no whitespace/syntax diff issues).
- Confirmed top link text remains in page and no footer "back to" navigation remains.

## Residual risks
- `Mares Display` custom font is loaded via a relative path from `/vica/index.html` and expects `../assets/fonts/eurostile-extended-black.woff2` to be available in that location.
