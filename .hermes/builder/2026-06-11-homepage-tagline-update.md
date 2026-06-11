# Homepage tagline update

- Timestamp (UTC): 2026-06-11T19:51:39Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Files changed: `index.html`

## What I changed
- Updated the homepage tagline text in `index.html` from:
  - `We build restrained interfaces for` + `race-critical information.`
  - to `Reduce noise, focus on what matters.`

## Commands run
- `git status --short`
- `git rev-parse --abbrev-ref HEAD`
- `git remote -v`
- `git diff --check -- index.html`
- `git diff -- index.html`
- `git add index.html`
- `git commit -m "Update homepage tagline copy"`
- `git rev-parse --short HEAD`
- `git push`

## Validation
- `git diff --check` passed with no issues.
- Working tree clean after commit: `git status --short` returned no changes.
- Commit recorded: `39e2cc4`

## Push
- Pushed to `origin` successfully: `master -> master`.

## Residual risks
- No functional runtime risk; this is copy-only text change.
- Homepage tagline now matches requested wording on the main site only.
