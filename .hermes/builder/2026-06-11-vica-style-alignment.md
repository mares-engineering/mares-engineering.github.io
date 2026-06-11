# VICA page style alignment update

- Timestamp (UTC): 2026-06-11T19:58:00Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `vica/index.html`

## What changed
- Refreshed `vica/index.html` styles to match the homepage visual system:
  - Shared color tokens and typography direction (`--bg`, `--fg`, `--muted`, display/body fonts).
  - Reused `Mares Display` font-face usage with the same source path and local fallback stack.
  - Applied the same atmospheric background treatment, border/typography tone, and link styling approach.
  - Updated responsive spacing and heading scaling for consistent behavior with the homepage at small widths.

## Commands run
- `git add vica/index.html`
- `git commit -m "Align VICA page visual style with homepage"`
- `git rev-parse --short HEAD`
- `git status --short`
- `git diff --check -- vica/index.html`

## Validation
- `git diff --check` passed (no whitespace errors).
- Commit recorded for the task.

## Residual risks
- The VICA page now relies on `../assets/fonts/eurostile-extended-black.woff2` (same font strategy as homepage).
- If the font is unavailable in a deployment environment, fallback fonts will be used automatically.
