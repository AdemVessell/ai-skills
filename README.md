# AI Skills

A curated collection of AI skills, custom instructions, and agent skill files for Claude, Grok, and beyond. This repo is both a personal portfolio and a community resource — structured for easy browsing, forking, and contribution.

Built by Adem Vessell — @AdemVessell on X

---

## Master Catalog

All skills and instruction sets across the entire repo:

| Name | Type | Model | Description | Tags |
|------|------|-------|-------------|------|
| *Entries will appear here as skills and instructions are added.* | | | | |

---

## Repository Structure

```
ai-skills/
├── README.md                          ← You are here
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

### Claude

**Agent Skills (SKILL.md files)**

- **Claude Code:** Place the `SKILL.md` file in your project directory or use `.skill upload` to register it.
- **Claude.ai:** Copy the contents of `SKILL.md` into a Project's custom instructions or attach it as a knowledge file.

**Custom Instructions (INSTRUCTIONS.md files)**

- **Claude Code:** Add the contents to your `CLAUDE.md` or project instructions file.
- **Claude.ai:** Paste the contents into your profile-level or project-level custom instructions.

### Grok

**Custom Instructions & Skills**

- Open Grok and navigate to your custom instructions panel.
- Paste the contents of the relevant `INSTRUCTIONS.md` or `SKILL.md` file directly into the custom instructions field.
- Grok applies custom instructions globally to all conversations once set.

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
