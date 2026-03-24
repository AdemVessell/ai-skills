# Agent Skills

Modular skill files that give AI agents specialized capabilities. Unlike custom instructions (which shape general behavior), agent skills are task-specific — they teach an agent how to perform a particular workflow, apply a framework, or produce a specific kind of output.

Each skill lives in a model-specific subfolder (`claude/`, `grok/`) with its own `SKILL.md` file. Skills can include supporting references, scripts, and assets.

Built by Adem Vessell — @AdemVessell on X

---

## Index

| Name | Description | Model | Tags |
|------|-------------|-------|------|
| [Ethereal Burn](claude/ethereal-burn/) | Constrained poetic prompt engine — burns default probability basins to produce sensation-driven image prompts from material truth, tactile paradox, and atmospheric residue | Claude | `image-prompting`, `creative-writing`, `style-system` |

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

See the full **[Install Guide](../INSTALL.md)** for detailed step-by-step instructions.

**Claude Code (personal — all projects):**
```bash
mkdir -p ~/.claude/skills/<skill-name>
cp claude/<skill-name>/SKILL.md ~/.claude/skills/<skill-name>/
```

**Claude Code (project — single repo):**
```bash
mkdir -p .claude/skills/<skill-name>
cp path/to/claude/<skill-name>/SKILL.md .claude/skills/<skill-name>/
```

Skills are auto-discovered — invoke with `/<skill-name>` or Claude picks them up automatically.

**Claude.ai:** Copy the contents of `SKILL.md` into a Project's custom instructions or attach it as a knowledge file.

**Grok:** Paste the contents of `SKILL.md` into Grok's custom instructions panel.
