# Zinsser Editor

A usable nonfiction editing skill based on operational principles from William Zinsser's *On Writing Well*.

It is designed for LLM agents. The goal is **not** to imitate Zinsser's prose. The skill uses his editorial principles to improve clarity, simplicity, structure, precision, voice, rhythm, and restraint.

## Structure

```text
zinsser-editor/
├── SKILL.md
├── README.md
├── references/
│   ├── principles.md
│   └── diagnostics.md
└── tests/
    └── cases.md
```

## How it works

`SKILL.md` is the executable core. It defines four modes:

- **analyze** — diagnose without rewriting;
- **edit** — make the smallest useful changes;
- **rewrite** — permit structural changes when explicitly requested;
- **audit** — evaluate finished prose.

The core file is intentionally compact. Detailed chapter-derived principles and diagnostics live in `references/` so an agent can load them only when needed.

## Design principles

- preserve the writer rather than replacing the writer;
- fix structural problems before sentence polish;
- treat shorter as a means, not a goal;
- protect factual and technical accuracy;
- distinguish editing from rewriting;
- test whether already-good prose remains unchanged;
- avoid generic AI prose.

## Validation

Behavioral cases are in `tests/cases.md`. The most important test is restraint: the skill should leave effective writing alone.

## Installation

Use the `zinsser-editor` directory as the skill package. `SKILL.md` contains valid YAML front matter and all required operating instructions. Keep the `references/` folder with it so an agent can progressively load the deeper guidance.
