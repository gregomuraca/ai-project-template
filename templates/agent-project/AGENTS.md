# Agent Instructions

## Objective

Use this repository's written state before relying on chat history.

## Required reading order

Before substantial work, read:

1. `PROJECT_STATE.md`
2. `ARCHITECTURE.md` when the task can affect system structure
3. `DECISIONS.md` when the task may reopen an existing decision
4. `ROADMAP.md` when choosing or sequencing work

## Operating rules

- Keep scope bounded to the active task.
- Do not change architecture or UI outside the approved scope.
- Distinguish facts, assumptions, and open questions.
- Prefer small, reviewable changes.
- Run relevant tests or validators before claiming completion.
- If a consequential external action is required, verify authority first.
- Update project state when verified work materially changes what is true.

## Completion

A task is complete when the requested output exists and the relevant verification passes.

Do not report completion based only on an implementation attempt.
