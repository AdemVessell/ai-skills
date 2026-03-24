# Install Guide

Step-by-step instructions for downloading, installing, and using skills and custom instructions from this repo.

---

## 1. Download

**Option A — Clone the repo:**

```bash
git clone https://github.com/AdemVessell/ai-skills.git
cd ai-skills
```

**Option B — Download a single file:**

Browse to the skill or instruction set you want on GitHub and click the "Raw" button, then save the file locally.

---

## 2. Install Agent Skills

Agent skills are `SKILL.md` files found under `agent-skills/`.

### Claude Code

Claude Code auto-discovers skills from `.claude/skills/` directories. No upload command is needed — just place the files in the right location.

**Personal install (available in all your projects):**

```bash
# Example: install the "ethereal-burn" skill
mkdir -p ~/.claude/skills/ethereal-burn
cp agent-skills/claude/ethereal-burn/SKILL.md ~/.claude/skills/ethereal-burn/

# If the skill has supporting reference files, copy those too
cp -r agent-skills/claude/ethereal-burn/references ~/.claude/skills/ethereal-burn/ 2>/dev/null
```

**Project install (available only in one repo):**

```bash
# Run this from your project root
mkdir -p .claude/skills/ethereal-burn
cp path/to/agent-skills/claude/ethereal-burn/SKILL.md .claude/skills/ethereal-burn/
cp -r path/to/agent-skills/claude/ethereal-burn/references .claude/skills/ethereal-burn/ 2>/dev/null
```

**Verify it works:**

- In Claude Code, type `/<skill-name>` (e.g. `/ethereal-burn`) to invoke it directly
- Or just start a conversation — Claude picks up installed skills automatically

**Uninstall:**

```bash
rm -rf ~/.claude/skills/ethereal-burn        # personal
rm -rf .claude/skills/ethereal-burn           # project
```

### Claude.ai (Projects)

Claude.ai does not use the `SKILL.md` file format directly. Instead:

1. Open [claude.ai](https://claude.ai) and create or open a **Project**
2. Go to **Project settings → Custom instructions**
3. Paste the full contents of the `SKILL.md` file into the custom instructions field
4. **Or** click **Add knowledge** and upload the `SKILL.md` file directly

The skill will apply to all conversations within that project.

### Grok

1. Open Grok and navigate to the **custom instructions** panel
2. Paste the full contents of the `SKILL.md` file
3. The skill applies globally to all conversations

---

## 3. Install Custom Instructions

Custom instructions are `INSTRUCTIONS.md` files found under `custom-instructions/`.

### Claude Code

Add the contents to your project's `CLAUDE.md` file:

```bash
# Append to an existing CLAUDE.md (or create one)
cat custom-instructions/claude/<name>/INSTRUCTIONS.md >> CLAUDE.md
```

Or copy the contents manually into your `CLAUDE.md`.

### Claude.ai

1. Go to [claude.ai](https://claude.ai) → **Settings → Profile**
2. Paste the contents of `INSTRUCTIONS.md` into the **Custom instructions** field
3. Or add them at the **Project level** for project-specific behavior

### Grok

1. Open Grok → **Custom instructions** panel
2. Paste the contents of `INSTRUCTIONS.md`
3. Instructions apply globally to all conversations

---

## Quick Reference

| What you have | Where it goes (Claude Code) | Where it goes (Claude.ai) | Where it goes (Grok) |
|---|---|---|---|
| `SKILL.md` | `~/.claude/skills/<name>/` (personal) or `.claude/skills/<name>/` (project) | Project custom instructions or knowledge file | Custom instructions panel |
| `INSTRUCTIONS.md` | Append to `CLAUDE.md` | Profile or project custom instructions | Custom instructions panel |

---

## Troubleshooting

**Skill not showing up in Claude Code?**
- Verify the path: `ls ~/.claude/skills/<name>/SKILL.md` or `ls .claude/skills/<name>/SKILL.md`
- The directory name becomes the skill's command name — use lowercase with hyphens
- Restart Claude Code after adding new skills

**Skill not working in Claude.ai?**
- Make sure you pasted the *full contents* of `SKILL.md`, not just the filename
- Check that the text is in the Project's custom instructions, not just the chat

---

## More Info

- [Claude Code Skills docs](https://docs.anthropic.com/en/docs/claude-code/skills)
- [Claude.ai Projects](https://support.anthropic.com/en/collections/4775303-projects)
