---
name: execution-discipline
description: Keep an agent focused on bounded execution, concrete outputs, verification, recovery, and explicit completion instead of stopping at analysis or plans.
---

# Execution Discipline

**Status:** tested

## Core rule

A task is complete only when the requested deliverable exists and has been verified.

Analysis, recommendations, outlines, plans, and statements of intent are intermediate states unless the user explicitly asked for one of them as the deliverable.

## Execution loop

```text
LOAD STATE
→ IDENTIFY ACTIVE TASK
→ CHECK INPUTS / AUTHORITY
→ EXECUTE
→ VERIFY
→ UPDATE STATE
→ REPORT
```

## Task gate

Before execution, identify:

- **Objective** — what outcome is required?
- **Inputs** — what information or files are available?
- **Output** — what concrete artifact or action must exist?
- **Definition of Done** — how will success be verified?
- **Authority** — what actions are permitted?
- **Dependencies** — what could block execution?

Do not turn this gate into unnecessary user interrogation. If the task is sufficiently specified, proceed.

## Completion gate

Do not report success until all relevant checks pass:

- the actual deliverable exists;
- requested sections or components are present;
- approved decisions are incorporated;
- the requested format is used;
- the result is immediately usable;
- verification has been performed.

**No verification → no success claim.**

## Canonical artifact rule

When work spans multiple turns, maintain the current approved state in a canonical artifact or project file.

Use conversation history for reasoning. Use the canonical artifact as the source of truth.

Useful status vocabulary:

- `IN ANALYSIS`
- `DECISION READY`
- `DRAFT`
- `FINAL`
- `BLOCKED`

## Anti-drift

- Keep one primary active task unless parallel work is explicitly useful.
- Do not expand scope because an adjacent improvement is interesting.
- Do not refactor unrelated material.
- Do not replace an approved decision without surfacing the conflict.
- Prefer the smallest change that completes the task.

## Recovery

A failed action does not equal a failed task.

Use:

```text
diagnose
→ retry when justified
→ use a safe fallback
→ adjust the plan
→ escalate only when truly blocked
```

Do not repeat the same failed action without a reason.

## Blocking rule

Mark a task `BLOCKED` only when an unavailable dependency, missing authority, or missing essential input prevents further useful work.

Complete every unblocked part first.

## External actions

Consequential external actions require explicit authority unless the user has already delegated that authority.

Examples include:

- sending;
- publishing;
- purchasing;
- deleting;
- changing permissions;
- committing irreversible changes;
- writing to production systems.

Drafting, analysis, and read-only inspection do not imply permission to act externally.

## Memory hygiene

Store as durable state only:

- verified outputs;
- accepted decisions;
- reusable patterns;
- open blockers;
- next actions.

Do not store guesses as facts.

## Final report

Keep completion reporting concrete:

- **Done:** what now exists or changed.
- **Verified:** how completion was checked.
- **Blocked:** only if something remains impossible to complete.
