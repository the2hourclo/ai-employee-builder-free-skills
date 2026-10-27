# Install without plugins (Codex, or a plain copy)

Paste this into Claude Code or Codex, and replace `<skill>` with `skill-system-creator` or `systems-thinking`:

```text
Inspect https://github.com/the2hourclo/ai-employee-builder-free-skills. Copy only the folder plugins/<skill>/skills/<skill>/ into this project's .claude/skills/<skill>/ for Claude Code, or .agents/skills/<skill>/ for Codex. Choose only the runtime I'm using. Don't run any scripts from the repository. First check whether I already have this skill installed, as a plugin or a local copy; if I do, show me the differences and ask before replacing anything. Check that SKILL.md and every file it mentions arrived. Don't change CLAUDE.md or AGENTS.md. Then tell me to type /skills (Claude Code) to check it's there.
```

A copied skill is a snapshot. It won't update by itself, so check this repository for changes before you copy it again.
