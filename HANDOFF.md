# Website Handoff

Date: 2026-06-11

This repo is the public Mares Engineering GitHub Pages site.

## Current Site Shape

Root:

```text
/
```

Purpose:

- Mares Engineering home page
- links to Vica and Minimai
- not a dedicated Vica-only page

Vica:

```text
/vica/
```

Purpose:

- static public Vica landing page
- serious, restrained, safety-first positioning
- no backend
- no accounts
- no payments
- no analytics

Minimai:

```text
/minimai/
```

Purpose:

- existing Minimai placeholder/page, preserved

## Typography Decision

Only the root `Mares Engineering` heading should use the Eurostyle/Eurostile
display face.

Everything else on the root page should remain Baskerville-style unless Javier
explicitly changes direction.

Current implementation:

- CSS defines `@font-face` for `Mares Display`.
- It expects a licensed webfont at:

```text
assets/fonts/eurostile-extended-black.woff2
```

Important:

- Visitors do not need Eurostyle installed if this `.woff2` file is shipped.
- If the file is missing, browsers use fallback fonts.
- Do not add a commercial font file unless Javier has license rights to use it
  as a webfont.

## Public-Safety Rules

Do not publish:

- private strategy
- internal pricing assumptions
- secrets
- customer/support data
- official approval or certification claims
- broad simulator/platform support claims
- production payment/account/licensing claims

## Roadmap Source Of Truth

Read first:

- `AGENTS.md`
- `WEBSITE_ROADMAP.md`
- `CONTENT_PRINCIPLES.md`
- `prompts/README.md`

Prompt sequence:

1. `prompts/02_trust_and_safety_page.md`
2. `prompts/03_compatibility_page.md`
3. `prompts/04_install_disable_docs.md`
4. `prompts/05_support_intake_entry.md`
5. `prompts/06_changelog_release_page.md`
6. `prompts/07_pricing_mock_only.md`

The first landing-page pass has already been done and revised so `/vica/` is
separate from the root company page.

## Spark Operating Model

Default worker:

```text
Hermes profile: vica-biz-spark
```

Codex should normally:

- scope a focused task
- run Spark
- review the diff and generated claims
- ask Spark for revisions if needed

Example:

```powershell
cd C:\Users\javie\repos\mares-engineering.github.io
hermes -p vica-biz-spark -z (Get-Content -Raw .\prompts\02_trust_and_safety_page.md)
```

## Review Checklist

Before accepting Spark output:

```powershell
git status --short
git diff --check
git log --oneline --decorate -n 5
git show --stat --oneline HEAD
```

Also inspect builder reports. Spark has previously written incorrect commit
hashes in builder reports, so do not trust those blindly.

## Next Recommended Task

If continuing website work, create the trust/privacy/install-safety page next.

Goal:

- explain user control
- explain static/no-account/no-payment posture
- explain disable/uninstall safety
- avoid legal promises
- avoid official approval/certification claims

Then move to compatibility and install/disable docs.
