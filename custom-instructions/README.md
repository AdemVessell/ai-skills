# Custom Instructions

Reusable instruction sets that shape how AI models behave across conversations. Custom instructions define personality, tone, reasoning style, output format, and domain expertise — they turn a general-purpose model into a specialized one.

Each instruction set lives in a model-specific subfolder (`claude/`, `grok/`) with its own `INSTRUCTIONS.md` file. Some instruction sets are portable across models; others are tuned for a specific model's strengths.

Built by Adem Vessell — @AdemVessell on X

---

## Index

| Name | Description | Model | Tags |
|------|-------------|-------|------|
| *Entries will appear here as instruction sets are added.* | | | |

---

## Structure

```
custom-instructions/
├── README.md        ← You are here
├── claude/
│   └── <name>/
│       ├── INSTRUCTIONS.md
│       └── references/   (optional)
└── grok/
    └── <name>/
        ├── INSTRUCTIONS.md
        └── references/   (optional)
```

---

## How to Use

**Claude:** Paste the contents of `INSTRUCTIONS.md` into your Claude.ai custom instructions (profile or project level), or add them to your `CLAUDE.md` file for Claude Code.

**Grok:** Paste the contents into Grok's custom instructions panel. Instructions apply globally to all conversations.
