# AI Skills

A curated collection of AI skills, custom instructions, and agent skill files for Claude, Grok, and beyond. This repo is both a personal portfolio and a community resource — structured for easy browsing, forking, and contribution.

Built by Adem Vessell — @AdemVessell on X

---

## Master Catalog

All skills and instruction sets across the entire repo:

| Name | Type | Model | Description | Tags |
|------|------|-------|-------------|------|
| [Ethereal Burn](agent-skills/claude/ethereal-burn/) | Agent Skill | Claude | Constrained poetic prompt engine — burns default probability basins to produce sensation-driven image prompts from material truth, tactile paradox, and atmospheric residue | `image-prompting`, `creative-writing`, `style-system` |

---

## Repository Structure

```
ai-skills/
├── README.md                          ← You are here
├── INSTALL.md                         ← Full install guide
├── custom-instructions/
│   ├── README.md                      ← Index of all custom instruction sets
│   ├── claude/
│   │   └── README.md
│   └── grok/
│       └── README.md
└── agent-skills/
    ├── README.md                      ← Index of all agent skills
    ├── claude/
    │   └── README.md
    └── grok/
        └── README.md
```

Each skill or instruction set lives in its own subfolder containing:

- **SKILL.md** (agent skills) or **INSTRUCTIONS.md** (custom instructions) — the primary file
- **references/** — supporting docs, research, or context (optional)
- **scripts/** — automation helpers (optional)
- **assets/** — images, diagrams, or media (optional)

---

## Install Instructions

See the full **[Install Guide](INSTALL.md)** for detailed step-by-step instructions.

### Quick Start

**Claude Code (Agent Skills)**

```bash
# Personal install (available in all projects)
mkdir -p ~/.claude/skills/<skill-name>
cp agent-skills/claude/<skill-name>/SKILL.md ~/.claude/skills/<skill-name>/
# Copy supporting files if they exist
cp -r agent-skills/claude/<skill-name>/references ~/.claude/skills/<skill-name>/ 2>/dev/null

# Project install (this repo only)
mkdir -p .claude/skills/<skill-name>
cp agent-skills/claude/<skill-name>/SKILL.md .claude/skills/<skill-name>/
```

**Claude.ai** — Copy the contents of `SKILL.md` into a Project's custom instructions or attach it as a knowledge file.

**Claude Code (Custom Instructions)** — Add the contents of `INSTRUCTIONS.md` to your `CLAUDE.md` or project instructions file.

**Claude.ai (Custom Instructions)** — Paste the contents into your profile-level or project-level custom instructions.

**Grok** — Paste the contents of `SKILL.md` or `INSTRUCTIONS.md` into Grok's custom instructions panel. Instructions apply globally to all conversations.

---

## Tag Vocabulary

Skills and instructions are tagged for discoverability:

`image-prompting` · `video-prompting` · `cognitive-architecture` · `memory-systems` · `compression` · `creative-writing` · `code-generation` · `workflow-automation` · `multi-model` · `style-system`

Tags expand as the collection grows.

---

## Contributing

1. Fork this repo
2. Add your skill or instruction set following the structure above
3. Update the relevant index READMEs and the master catalog
4. Open a PR

---

## License

MIT — see [LICENSE](LICENSE) for details.
