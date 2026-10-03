# Useful AI Stuff

Practical AI skills, templates, workflows, and small tools I use and share freely.

This repository is intentionally selective. It is not a prompt dump. Each artifact should encode a repeatable method, solve a real problem, and be usable without private project context.

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

Artifacts should identify themselves as one of:

- **stable** — used repeatedly and behavior is understood;
- **tested** — useful in real work but still evolving;
- **prototype** — functional enough to explore;
- **discovery** — documented idea or experiment, not a production recommendation.

## Current collection

### Skills

- **Zinsser Editor** — nonfiction editing for clarity, structure, precision, voice, and restraint.
- **No Slop** — detects and removes synthetic, generic, over-engineered AI writing without flattening the author's voice.
- **Execution Discipline** — keeps agents focused on concrete deliverables, verification, recovery, and explicit completion.

### Templates

- **Agent Project** — durable project memory for architecture, decisions, current state, and roadmap.

### Workflows

- **Claude + Codex Collaboration** — separates implementation from adversarial review and uses explicit gates between phases.
- **Human-in-the-Loop Agent** — approval boundaries for agents that read, recommend, draft, and take external actions.

## Principles

1. **Useful beats clever.**
2. **Canonical instructions live once.**
3. **Agents should distinguish analysis from execution.**
4. **Verification is part of completion.**
5. **Human approval is required before consequential external actions unless authority was explicitly delegated.**
6. **Good skills preserve context, uncertainty, and voice instead of normalizing everything.**
7. **A skill should know when not to act.**

## Contributing

Keep contributions small and testable. Remove private data, credentials, account identifiers, client-specific material, and proprietary information before publishing.
