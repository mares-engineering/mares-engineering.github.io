# Spark prompts for this repo

These prompts are for running `vica-biz-spark` against this repository.

Use the canonical launch form:

- `hermes -p vica-biz-spark -z "<prompt>"`

Each prompt is scoped to static, public-safe website tasks.

## Review flow

After Spark completes a prompt:

1. Review the diff for wording, claims, and safety posture.
2. If needed, run a follow-up review pass.
3. A `Codex`-lane agent is used primarily for review/escalation, not implementation.
4. No push is required for normal tasks in this repo.
