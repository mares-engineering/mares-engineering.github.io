# Builder Report

Date: 2026-06-11
Task: Fix homepage font fallback to a self-hosted Eurostyle-like display family.

## Repo
- Path: C:\Users\javie\repos\mares-engineering.github.io
- Branch: master

## Files changed
- index.html
- assets/fonts/README.md
- .hermes/builder/2026-06-11-prepare-self-hosted-eurostyle-font-hook.md

## Validation plan
- `git status --short`
- `git diff --check`
- Verify `index.html` now defines `@font-face` for `assets/fonts/eurostile-extended-black.woff2`
- Verify heading and links use a dedicated display font variable with geometry-oriented fallbacks

## Commands executed
1. `git branch --show-current`
2. `read_file` inspected `index.html` and `AGENTS.md`
3. `patch` updated `index.html` with `@font-face` and fallback-safe display variables
4. `write_file` added `assets/fonts/README.md`
5. `write_file` added `.hermes/builder/2026-06-11-prepare-self-hosted-eurostyle-font-hook.md`
6. `git status --short`
7. `git diff --check`

## Validation run
- `git status --short`
- `git diff --check`

## Commit
- SHA: 1e4b67b

## Residual risks
- Actual Eurostyle/Eurostile Extended Black rendering depends on adding a legally licensed `assets/fonts/eurostile-extended-black.woff2` file; fallback stack uses widely available geometric sans-heavy faces.
- The `@font-face` rule does not prevent layout shift until fallback swap occurs; `font-display: swap` helps reduce blocking.
