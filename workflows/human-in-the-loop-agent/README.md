# Human-in-the-Loop Agent

**Status:** tested

A practical authority model for agents that can read data, make recommendations, draft outputs, and potentially take external actions.

## Principle

Start with the least authority needed.

A useful default progression is:

```text
READ
→ ANALYZE
→ RECOMMEND
→ DRAFT
→ APPROVE
→ ACT
→ VERIFY
→ LOG
```

Do not confuse access with authority.

## Authority levels

### 1. Read

The agent may inspect approved sources.

No mutation.

### 2. Analyze

The agent may derive findings, rankings, or diagnoses.

No mutation.

### 3. Recommend

The agent may propose actions and explain rationale, expected benefit, uncertainty, and risks.

No mutation.

### 4. Draft

The agent may prepare a message, configuration, change set, campaign, PR, or other action artifact.

Still no external execution unless separately authorized.

### 5. Act

The agent may perform an external write only within explicitly granted boundaries.

Examples:

- send a specific approved message;
- apply an approved code change;
- create an approved record;
- update an approved configuration.

## Approval gate

Require human approval when an action is:

- irreversible or difficult to undo;
- externally visible;
- financial;
- permission-changing;
- destructive;
- legally or reputationally consequential;
- outside previously delegated scope.

The approval request should summarize:

- proposed action;
- target;
- expected effect;
- important risk;
- reversibility;
- evidence supporting the action.

## Draft-then-approve

For agents writing as a person or organization:

1. gather context;
2. draft;
3. show the exact draft;
4. obtain approval;
5. send;
6. verify delivery/status.

## Bounded autonomy

Delegation should specify:

- allowed tools/actions;
- allowed targets;
- spend or quantity limits when relevant;
- time window;
- stop conditions;
- escalation conditions.

## Logging

For material actions, record:

- timestamp;
- action;
- target;
- authority basis;
- result;
- error if any;
- verification;
- human correction when applicable.

Never log passwords, API keys, or secrets.

## Failure handling

If an action fails:

```text
stop
→ identify the first upstream error
→ determine whether retry is safe
→ retry within bounds or request approval
```

Do not compound uncertainty by continuing downstream after a critical failure.

## Learning loop

Sample completed traces periodically.

For failures or human corrections, ask:

- Was the authority boundary wrong?
- Was necessary context missing?
- Was the recommendation unsupported?
- Did the agent misunderstand a business rule?
- Can a deterministic validator prevent recurrence?

Update the workflow only from verified failures and accepted corrections.
