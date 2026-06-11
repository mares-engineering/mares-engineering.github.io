# Prompt: P0 Landing page first pass (static)

Run this as a static website implementation pass for VICA. Before editing, read:

- `AGENTS.md`
- `WEBSITE_ROADMAP.md`
- `CONTENT_PRINCIPLES.md`
- If needed, the public business planning docs in `C:\\Users\\javie\\repos\\vica-business`

## Objective

Implement a first, restrained landing page for VICA in this website repo.

## Scope

- Static page only.
- No backend integration.
- No accounts, authentication, analytics scripts requiring PII collection, or payment/checkout flows.
- Keep the page public-safe and conservative.

## Constraints

- Preserve existing visible behavior unless this update is necessary for the landing work.
- Do not add private strategy, internal pricing assumptions, secrets, or customer data.
- Do not claim unapproved performance, official race approvals, or broad simulator support.

## Deliverables

1. Create/update a landing page file under `vica/` or site root that includes:
   - clear title and short value proposition
   - one-line positioning statement
   - primary CTA (waitlist/interest only)
   - short trust-oriented install safety note
2. Use plain HTML and minimal CSS as needed.
3. Add concise copy aligned with `CONTENT_PRINCIPLES.md`.

## Validation and completion criteria

- Run: `git status --short`.
- Run: `git diff --check`.
- Commit locally with a clear message.
- Do not push.

This task is done when the diff is clean (no whitespace errors), static, and review-ready.
