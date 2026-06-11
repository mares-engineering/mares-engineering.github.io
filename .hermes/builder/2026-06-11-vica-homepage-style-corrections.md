# VICA homepage-style alignment correction

- Timestamp (UTC): 2026-06-11T21:23:47Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `vica/index.html`

## What changed
- Reworked `vica/index.html` to match the homepage visual system more completely:
  - Reused homepage palette/effects (`--bg`, `--fg`, glow, radial gradient background treatment, text effects).
  - Kept spacing, shell, and responsive behavior aligned to the homepage structure.
  - Kept the Mares Engineering masthead treatment and glow behavior while removing dependency on the Eurostyle font.
- Explicitly set display/body fonts to Baskerville for VICA (no Eurostyle/font-face import).
- Replaced static bottom footer links with a cleaner layout; top brand header now links to the homepage (`../index.html`) so users can navigate back via that or browser back.

## Commands run
- `git add vica/index.html`
- `git commit -m "Align VICA page to homepage styling and link top brand"`
- `git rev-parse --short HEAD`
- `git show --stat --oneline --name-only --no-patch`
- `date -u +"%Y-%m-%dT%H:%M:%SZ"`
- `git status --short`
- `git diff --check -- vica/index.html`

## Commit
- `83e94f3`

## Validation
- `git diff --check -- vica/index.html` returned clean (no whitespace errors).
- Manual verification confirms the bottom footer links were removed and the masthead is linked to homepage.

## Residual risks
- The VICA page no longer uses `Mares Display`/Eurostyle assets.
- Brand header still uses homepage-like gradient glow behavior, but with Baskerville typography per request.
