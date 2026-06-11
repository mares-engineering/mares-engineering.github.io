# VICA Website Roadmap (Public-safe)

This roadmap is for website work only and keeps the site static-first, conservative, and reviewable.

## P0 - Landing page and VICA positioning

- **Purpose:** Publish a restrained, truthful, static landing entry that introduces VICA clearly.
- **Likely files:**
  - `index.html` (if repurposed), `vica/index.html`, `vica.css` (if needed), `assets/` (optional).
- **Acceptance criteria:**
  - Static page with concise hero, one-sentence value proposition, and clear next step.
  - No backend calls, no account/payment/login flows.
  - Tone is serious and race-aware, avoiding generic HUD/overlay claims.
- **Spark autonomy:** High.
  - Spark can draft structure, copy, and light layout.
  - Required human review for regulatory or safety wording before publish.

## P0 - Waitlist / alpha-interest CTA placeholder

- **Purpose:** Add explicit, friction-minimal path for private-alpha interest without data collection promises.
- **Likely files:**
  - `vica/waitlist.html` (or landing variant), `vica/index.html`.
- **Acceptance criteria:**
  - CTA present and clearly framed as placeholder/intake notice.
  - No account creation, no sales funnel, no claim of guaranteed onboarding.
  - Static link/placeholder form pattern only.
- **Spark autonomy:** High.
  - Spark can create page and links.
  - Must avoid collecting sensitive/PII in static examples.

## P0 - Trust / privacy / install-safety page

- **Purpose:** Explain safety posture, install behavior, disable options, and data boundaries.
- **Likely files:**
  - `vica/trust.html`, `vica/safety.html` (or shared location).
- **Acceptance criteria:**
  - Explicit mention that VICA is race-critical assistance tooling and failure modes should remain safe.
  - Clear disable/uninstall guidance.
  - Data handling described conservatively, no overbroad telemetry commitments.
  - No legal overpromises.
- **Spark autonomy:** Medium.
  - Write conservative, conservative language with review gate on any trust wording.

## P0 - Compatibility page

- **Purpose:** Publish validated/supported target matrix with careful unknown handling.
- **Likely files:**
  - `vica/compatibility.html`, simple CSV/JSON snippet if needed.
- **Acceptance criteria:**
  - Categories explicitly separated: **validated**, **currently supported**, **unknown**.
  - No false certainty where evidence is missing.
  - Updates trackable via plain text source of truth.
- **Spark autonomy:** Medium.
  - Spark can scaffold the matrix; claims must be factual and labeled.

## P1 - Install / disable / troubleshooting docs

- **Purpose:** Provide public first-aid docs for install steps and emergency disable/stop paths.
- **Likely files:**
  - `vica/install-disable.html`, `vica/troubleshooting.html`.
- **Acceptance criteria:**
  - Install path is explicit and short.
  - Disable/uninstall actions are prominent and top-of-page.
  - Troubleshooting entries are practical, low-verbosity, and safe.
- **Spark autonomy:** Medium.
  - Write docs directly from static templates; review wording for safety-critical items.

## P1 - Changelog / news / release page

- **Purpose:** Publish public-safe progress updates without internal status details.
- **Likely files:**
  - `vica/changelog.html`, `vica/news.html`, or `vica/releases.md`.
- **Acceptance criteria:**
  - Chronological entries with date + short title + concise change.
  - No internal roadmap leakage.
  - Plain static list or markdown rendered pages only.
- **Spark autonomy:** Medium-high.
  - Spark can draft entry format; maintainers verify accuracy and disclosure wording.

## P1 - Support intake entry page

- **Purpose:** Offer a public-safe starting point for support without backend.
- **Likely files:**
  - `vica/support.html`, `vica/support/templates.md`.
- **Acceptance criteria:**
  - Includes clear triage questions and contact placeholder.
  - Template links or placeholders only, no real support data storage.
  - Links to troubleshooting and install-safety docs.
- **Spark autonomy:** High.
  - Static page and template assets can be scaffolded by Spark.

## P2 - Pricing / shop mock pages only

- **Purpose:** Add non-production pricing and shop visuals for evaluation only.
- **Likely files:**
  - `vica/pricing.html`, `vica/shop-mock.html`, `vica/assets/pricing.json`.
- **Acceptance criteria:**
  - No live payment, invoicing, licensing, or account system wiring.
  - Clearly marked as mock/scaffold.
  - No conversion pressure messaging.
- **Spark autonomy:** High with guardrails.
  - Spark can build mock UI and placeholder flows only.
  - Must stop if production-sales functionality is accidentally introduced.

## Scope rule

Treat this roadmap as public-safe and static-first. Any phase that introduces operational behavior beyond static content must be explicitly approved before implementation.
