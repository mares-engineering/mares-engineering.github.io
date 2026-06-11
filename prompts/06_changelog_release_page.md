# Prompt: P1 changelog / news / release page skeleton

Create a static changelog/news page suitable for public updates.

## Read first

- `AGENTS.md`
- `CONTENT_PRINCIPLES.md`
- `WEBSITE_ROADMAP.md`

## Objective

Build a public changelog with date-ordered release/news entries.

## Scope

- Static content only.
- No references to internal issues, unreleased internal roadmap, or private metrics.
- Keep entries concise and evidence-light.

## Required structure

- Heading/title with VICA updates.
- Chronological sections (newest first).
- Each entry includes date and short summary.
- Optional compatibility and installation notes.

## Validation and completion criteria

- Run `git status --short`.
- Run `git diff --check`.
- Commit locally; do not push.
