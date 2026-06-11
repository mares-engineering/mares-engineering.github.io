# Prompt: P1 install / disable / troubleshooting docs skeleton

Create or refine public documentation for install, disable, and troubleshooting.

## Read first

- `AGENTS.md`
- `CONTENT_PRINCIPLES.md`
- `WEBSITE_ROADMAP.md`
- Prompt/notes in `prompts/` as needed

## Scope

- Static documentation pages only.
- No backend, tracking, or form submission logic.
- No code changes outside docs and static assets.

## Content requirements

- Install checklist with minimal steps.
- **Disable/uninstall** path appears prominently at the top.
- Troubleshooting section with practical, conservative first-response steps.
- Safety and escalation guidance (e.g., when to pause use).

## Non-goals

- No production support portal wiring.
- No customer PII collection.
- No hidden scripts for telemetry.

## Validation and completion criteria

- Run `git status --short`.
- Run `git diff --check`.
- Commit locally; do not push.
