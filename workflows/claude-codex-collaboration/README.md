# Claude + Codex Collaboration

**Status:** tested

A lightweight workflow for using two capable coding agents without making them duplicate each other's work.

The principle is separation of roles: one agent drives implementation; the other provides adversarial review or targeted rescue.

## Default loop

```text
REQUEST
→ PLAN
→ IMPLEMENT
→ TEST
→ ADVERSARIAL REVIEW
→ REVISE
→ VERIFY
→ ACCEPT
```

## Roles

### Primary agent

Owns:

- understanding the task;
- proposing the implementation plan;
- editing the code;
- running relevant tests;
- producing a reviewable diff.

### Reviewer agent

Owns:

- challenging assumptions;
- finding regressions, omissions, and unnecessary changes;
- checking the diff against the requirement;
- identifying untested behavior;
- proposing the smallest corrective action.

The reviewer should not rewrite the entire solution merely to express a different preference.

## Gates

### Plan gate

Before coding, define:

- objective;
- scope;
- files/components likely to change;
- main technical choice;
- verification method.

For consequential architecture changes, obtain owner approval before implementation.

### Implementation gate

Do not expand scope while coding without surfacing the reason.

### Review gate

The reviewer evaluates:

1. requirement coverage;
2. correctness;
3. regressions;
4. unnecessary complexity;
5. test adequacy;
6. architecture violations;
7. security / privacy concerns where relevant.

### Acceptance gate

Accept only when:

- requested behavior exists;
- relevant tests pass;
- review findings are resolved or explicitly accepted;
- no unrelated changes remain.

## Rescue mode

Use the second agent before abandoning a blocked implementation.

Provide:

- task;
- current approach;
- exact failure;
- relevant diff/error;
- constraints;
- what has already been tried.

Ask for diagnosis first, not a complete replacement.

## Anti-patterns

Avoid:

- both agents independently implementing the entire task;
- endless model debate with no executable test;
- reviewer preference presented as correctness;
- large rewrites when a local fix works;
- passing huge chat histories instead of current state and diffs.

## Useful metric

Track **human interventions per completed change**.

The workflow is improving when agents complete more correct, reviewable tasks without increasing regressions or hidden scope changes.
