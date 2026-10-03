# Useful AI Stuff

Practical AI skills, templates, workflows, and small tools I use and share.

This is not a prompt dump. Each artifact encodes a repeatable method, solves a real problem, and works without private project context.

## Structure

```text
useful-ai-stuff/
├── skills/
│   ├── zinsser-editor/
│   ├── no-slop/
│   └── execution-discipline/
├── templates/
│   └── agent-project/
├── workflows/
│   ├── claude-codex-collaboration/
│   └── human-in-the-loop-agent/
├── tools/
├── prompts/
└── experiments/
```

## Maturity

Each artifact has one maturity level:

- **stable** — used repeatedly; behavior is well understood.
- **tested** — useful in real work but still evolving.
- **prototype** — functional enough to test and explore.
- **discovery** — an idea or experiment, not a production recommendation.

## Current collection

### Skills

- **Zinsser Editor** — edits nonfiction for clarity, structure, precision, voice, and restraint.
- **No Slop** — removes generic, synthetic, and over-engineered AI writing without flattening the author's voice.
- **Execution Discipline** — keeps agents focused on concrete deliverables, verification, recovery, and explicit completion.

### Templates

- **Agent Project** — maintains durable project memory for architecture, decisions, current state, and roadmap.

### Workflows

- **Claude + Codex Collaboration** — separates implementation from adversarial review, with explicit gates between phases.
- **Human-in-the-Loop Agent** — defines approval boundaries for agents that read, recommend, draft, or take external actions.

## Principles

1. **Useful beats clever.**
2. **Canonical instructions live once.**
3. **Separate analysis from execution.**
4. **Verification is part of completion.**
5. **Require human approval before consequential external actions unless authority has been explicitly delegated.**
6. **Preserve context, uncertainty, and voice instead of normalizing everything.**
7. **A skill should know when not to act.**

## Contributing

Keep contributions small and testable.

Before publishing, remove private data, credentials, account identifiers, client-specific material, and proprietary information.
