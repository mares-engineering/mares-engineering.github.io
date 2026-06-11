# Undo beveling-alignment adjustment after center-shift regression on VICA brand header

- Timestamp (UTC): 2026-06-11T23:25:39Z
- Repo: `C:/Users/javie/repos/mares-engineering.github.io`
- Branch: `master`
- Commit applied: `926fd98`

## What changed
- Reverted the previous tweak (`ce8835f`) that introduced `.brand-link` `inline-grid`/`place-items:center` behavior and altered `MARES ENGINEERING` positioning.
- Restored the prior VICA header header state where the link is:
  - `display: inline-block`
  - left-aligned in page flow
  - no centered/expanded link container behavior
- Left beveling/font-size semantics in place from the previous accepted version (`fd0c581`), while removing the problematic alignment regression.

## Validation
- `sed`/`read` inspection of `vica/index.html` brand block
- `git diff --check -- vica/index.html`
- `git revert --no-edit ce8835f`
- `git push origin master`
