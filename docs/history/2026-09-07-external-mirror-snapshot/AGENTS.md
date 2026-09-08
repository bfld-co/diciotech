# AGENTS.md

## Anchora AI-Ready Baseline

This repository follows the non-invasive Anchora AI-Ready Baseline for work by Codex, Claude Code, Cursor, and other AI assistants.

## Read Order

1. repo.manifest.yaml for provenance and repository routing context.
2. README.md for product or project-specific instructions, if present.
3. AI_CONTEXT.md for AI operating context.
4. docs/ai/handoff.md for current handoff status.
5. Local docs, scripts, tests, and source files before changing behavior.

## Operating Rules

- Treat the repository as the source of truth. Do not rely only on chat history.
- Keep changes scoped to the user's request and the repo's existing architecture.
- Do not change runtime behavior, deploy flow, CI, credentials, webhooks, or Linear/GitHub integrations unless explicitly requested.
- Preserve existing conventions, file layout, naming, and validation commands.
- If commands are unknown, inspect the repo and document what was or was not validated.
- Prefer small, reviewable changes with clear handoff notes.

## Validation

Before finishing any future code change, identify and run the relevant validation path for this repo. If validation cannot run, report the reason and the residual risk.

## Handoff

After meaningful work, update docs/ai/handoff.md with: what changed, validation performed, open risks, and recommended next step.