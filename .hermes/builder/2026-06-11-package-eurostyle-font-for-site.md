# Builder Report

Date: 2026-06-11
Task: Package the Eurostyle/Eurostile display font as webfont so visitors do not need local installation.

## Repo
- Path: C:\Users\javie\repos\mares-engineering.github.io
- Branch: master

## Files changed
- assets/fonts/eurostile-extended-black.woff2
- assets/fonts/README.md
- .hermes/builder/2026-06-11-package-eurostyle-font-for-site.md

## Validation plan
- Confirm existing font hook in `index.html` already points at `assets/fonts/eurostile-extended-black.woff2`.
- Convert source font to WOFF2 and add to `assets/fonts`.
- Run repository checks for clean tree and diff sanity.

## Commands executed
1. `git status --short && git branch --show-current` (repo context)
2. `read_file` on `C:\Users\javie\repos\mares-engineering.github.io\HANDOFF.md` and website `HANDOFF.md` for font-source requirements.
3. `read_file` on `C:\Users\javie\repos\vica-business\HANDOFF.md` for product guidance.
4. `ls` / `git status` in `C:\Users\javie\repos\mares-engineering.github.io` and search references in `index.html` for existing font rule.
5. `uv run --with fonttools --with brotli python -m fontTools.ttLib.woff2 compress 'C:\Users\javie\Downloads\eurostile-extended-black-maisfontes.30a7\EurostileExtendedBlackOBS-repaired.ttf' -o 'C:\Users\javie\repos\mares-engineering.github.io\assets\fonts\eurostile-extended-black.woff2'`
6. `read_file` to confirm updated `assets/fonts/README.md`.
7. `search_files` for `assets/fonts/eurostile-extended-black.woff2` in repo.
8. `git add assets/fonts/eurostile-extended-black.woff2 assets/fonts/README.md && git commit -m "Package Eurostyle woff2 for site headline"`
9. `git status --short`
10. `git log --oneline --decorate -n 5`

## Validation run
- `git diff --check`
- `git status --short`

## Commit
- SHA: f069d15

## Residual risks
- The font file was generated from `EurostileExtendedBlackOBS-repaired.ttf`; ensure this source is the licensed artifact you want to distribute.
- If a different Eurostyle/Eurostile variant is preferred, replace `assets/fonts/eurostile-extended-black.woff2` and keep the filename stable.
- CRLF normalization warning appears for README due Git line-ending settings; content is unchanged semantically.
