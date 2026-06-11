# VICA Website Repo Agent Instructions

This repository is the public **Mares Engineering** GitHub Pages site at `mares-engineering.github.io`.

It hosts website-facing documentation and marketing context for VICA and related Mares Engineering pages. Treat all content here as public-facing. Do not add private strategy notes, internal pricing assumptions, secrets, unpublished claims, or customer data.

## Operating model

- This repo should remain simple, static, fast, and conservative by default.
- VICA website work should be serious, restrained, and trust-oriented.
- Prefer lightweight Markdown, static HTML, and plain configuration over complex application behavior.
- Prefer clear wording over hype and broad feature claims.
- Keep install and safety posture explicit.

## Implementation responsibility

- Normal implementation work in this repo is done by **Hermes profile `vica-biz-spark`**.
- `Codex` / larger model agents should normally be used for scoping, review, or escalation, not primary implementation.

## Hard constraints

- Do not edit core VICA runtime code.
- Do not edit production payment, account, or licensing systems.
- Do not add secrets, private keys, or internal support/customer data.
- Do not publish unapproved performance/coverage claims, official certification claims, or official race/organizer approvals.
- Do not change visible website behavior unless needed for docs/workflow changes.

## Reference context

- Use `C:\Users\javie\repos\vica-business` as the primary reference for business/productization plans.
- Treat `C:\Users\javie\repos\vica` as read-only unless explicitly instructed otherwise.

## Validation expectations

For changed files in this repo, include at minimum:
- `git status --short`
- `git diff --check`
- local commit when ready
- push accepted commits to `origin`

## Push policy

For this repository only, pushing is allowed and expected.

- Do not consider completed website work finished while it is local-only.
- After validation and review, push the accepted commit(s) to `origin`.
- If implementation was delegated to Hermes/Spark, Codex should review the
  result before pushing the final accepted state.
- This push policy applies only to `C:\Users\javie\repos\mares-engineering.github.io`.
  Do not infer push permission for `C:\Users\javie\repos\vica-business`,
  `C:\Users\javie\repos\vica`, or any other repo.
