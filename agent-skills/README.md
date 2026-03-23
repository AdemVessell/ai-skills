# Agent Skills

Modular skill files that give AI agents specialized capabilities. Unlike custom instructions (which shape general behavior), agent skills are task-specific — they teach an agent how to perform a particular workflow, apply a framework, or produce a specific kind of output.

Each skill lives in a model-specific subfolder (`claude/`, `grok/`) with its own `SKILL.md` file. Skills can include supporting references, scripts, and assets.

Built by Adem Vessell — @AdemVessell on X

---

## Index

| Name | Description | Model | Tags |
|------|-------------|-------|------|
| *Entries will appear here as skills are added.* | | | |

---

## Structure

```
agent-skills/
├── README.md        ← You are here
├── claude/
│   └── <name>/
│       ├── SKILL.md
│       ├── references/   (optional)
│       ├── scripts/      (optional)
│       └── assets/       (optional)
└── grok/
    └── <name>/
        ├── SKILL.md
        ├── references/   (optional)
        ├── scripts/      (optional)
        └── assets/       (optional)
```

---

## How to Use

**Claude Code:** Place the `SKILL.md` file in your project directory or use `.skill upload` to register it. The agent will pick up the skill automatically.

**Claude.ai:** Copy the contents of `SKILL.md` into a Project's custom instructions or attach it as a knowledge file.

**Grok:** Paste the contents of `SKILL.md` into Grok's custom instructions panel.
