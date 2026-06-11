# Prompt: P0 Compatibility page skeleton

Use this prompt to create a compatibility matrix page for the VICA website.

## Read first

- `AGENTS.md`
- `CONTENT_PRINCIPLES.md`
- `WEBSITE_ROADMAP.md`

## Objective

Create a conservative compatibility page showing what is known and what is not.

## Scope

- Static page only.
- No data fetchers or runtime checks.
- No unverified claims.

## Required structure

- Section: **Validated**
- Section: **Current support**
- Section: **Unknown / planned**

Each section must use explicit labels to avoid implying certainty where evidence is missing.

## Acceptance points

- Unknown items are clearly marked as unknown.
- If versions/hardware change, updates are easy by editing a simple list/table.
- No broad promises of wide compatibility.

## Validation and completion criteria

- Run `git status --short`.
- Run `git diff --check`.
- Commit locally.
- After Codex review, push accepted changes to `origin`.
