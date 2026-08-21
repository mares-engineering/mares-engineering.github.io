# Website Handoff

Date: 2026-07-31

This repository is the public Mares Engineering GitHub Pages site.

## Current site shape

Root:

```text
/
```

- The opening viewport preserves the centered Mares Engineering wordmark on the
  original near-black field.
- A minimal product directory appears below the first viewport.
- Shared site styling lives in `assets/site.css`.

Products:

```text
/vica/
/faber/
/minimai/
```

- VICA is a restrained private-alpha product and documentation surface with
  English and Spanish pages.
- Faber leads with the implemented Faber Proof entry point and its bounded,
  evidence-first trust model.
- Minimai remains an intentionally sparse coming-soon concept page.

Application profile:

```text
/nous/
```

- The Nous page is an unlisted, `noindex` technical application profile for Javier
  Mares.
- It is an open application to pursue Faber at Nous, beginning with an
  evidence-bound promotion layer for Hermes and treating outcome-linked learning
  trajectories as a conditional second stage.
- It links only public-safe work samples and presents Nous's existing tests,
  sandboxing, benchmarks, and human review as the baseline Faber must beat.
- Keep it off the root product directory; the exact URL is intended to be shared
  directly with application reviewers.

## Visual-source decisions

VICA must use genuine output from the VICA display renderer, shown on a neutral
black field. The current web assets are offline renderer previews generated from
representative canonical state:

```text
vica/assets/display/wind.png
vica/assets/display/incidents.png
vica/assets/display/minimum_corner_speed.png
vica/assets/display/relative_vertical.png
```

They are not live-session screenshots and do not prove VR placement or performance.
Keep that distinction visible in the page caption. Do not reintroduce fabricated
cockpit, circuit, simulator, or imagined HUD-placement imagery.

The Faber comparison graphic is a tracked product asset and carries the exact
`REPLAY — FAKE-DEVELOPMENT` provenance label. Minimai has no approved imagery and
should remain typography-only until real product material exists.

The Faber page links the dedicated `portfolio/faber-proof` source branch rather than
the repository's broader default branch. Keep the local checkpoint, audit status, and
policy-lifecycle limitation synchronized with that curated branch.

## Typography decision

Only the Mares Engineering company mark uses the bundled Eurostile-style display
face. Product names and body copy remain serif-led.

The licensed webfont is expected at:

```text
assets/fonts/eurostile-extended-black.woff2
```

Visitors do not need the font installed locally. Do not replace or redistribute the
font unless Mares Engineering has the required webfont rights.

## Public-safety rules

Do not publish:

- private strategy or internal pricing assumptions;
- secrets, customer data, or private support material;
- official approval, certification, sanction, or broad compatibility claims;
- production payment, account, licensing, or availability claims;
- Faber customer, revenue, universal-correctness, or production-sandbox claims;
- Minimai implementation, privacy, platform, or launch-date claims without a source.

## Maintenance rules

- Preserve the root page's first viewport when changing product discovery below it.
- Keep the site static and JavaScript-free unless a real requirement changes that.
- Update English and Spanish VICA pages together.
- Regenerate VICA screenshots from the renderer; do not redraw display elements by
  hand.
- Keep the VICA disable path and product limits prominent.

## Review checklist

Before publishing:

```powershell
git status --short
git diff --check
```

Also verify every local link and image, confirm that the fabricated VICA composite is
absent, and review new claims against the relevant product source repository.

Accepted website commits should be pushed to `origin` after review. This permission
applies only to this website repository.
