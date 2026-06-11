# Prompt: Continue Website Work In Codex

Use this prompt to start a new Codex project/thread for the website repo.

```text
This Codex project/thread is for the Mares Engineering GitHub Pages website.

Workspace:
C:\Users\javie\repos\mares-engineering.github.io

Business/productization reference repo:
C:\Users\javie\repos\vica-business

Core Vica app repo, read-only by default:
C:\Users\javie\repos\vica

Read first:
- C:\Users\javie\repos\mares-engineering.github.io\HANDOFF.md
- C:\Users\javie\repos\mares-engineering.github.io\AGENTS.md
- C:\Users\javie\repos\mares-engineering.github.io\WEBSITE_ROADMAP.md
- C:\Users\javie\repos\mares-engineering.github.io\CONTENT_PRINCIPLES.md
- C:\Users\javie\repos\vica-business\HANDOFF.md

Operating model:
Hermes profile vica-biz-spark is the default implementer for website work.
Codex should scope tasks, run Spark, review diffs, and request revisions.
Codex should not normally implement website work itself.

Use Spark with:
hermes -p vica-biz-spark -z "<self-contained task prompt>"

Important current state:
- Root / is the Mares Engineering home page.
- /vica/ is the Vica landing page.
- /minimai/ is preserved.
- Only the root Mares Engineering heading should use the Eurostyle/Eurostile
  display face.
- Other root text should remain Baskerville-style.
- Actual Eurostyle rendering requires a licensed webfont at
  assets/fonts/eurostile-extended-black.woff2.

Do not add production payments/accounts/licensing systems.
Do not add secrets, private strategy, customer data, or unsupported public
claims.
Do not edit core Vica runtime code.
Do not push unless Javier asks.

First check:
git status --short
git branch -vv

Recommended next task:
Run prompts/02_trust_and_safety_page.md through vica-biz-spark, then review the
result carefully for public-safety wording and builder-report accuracy.
```
