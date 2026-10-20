# Installation prompt

Give this prompt to Claude Code after giving it the repository link:

> Inspect this repository. Install only its `systems-thinking/` folder into `.claude/skills/systems-thinking/` in the project I opened. Do not execute repository scripts. If that destination already exists, show the differences and ask before replacing it. Check that SKILL.md and every referenced workflow/reference file exist. Offer to append THINK-IN-SYSTEMS.md to my project CLAUDE.md without replacing my instructions; wait for my answer before editing that file. Do not install any other skills, create a schedule, send messages, or change external services. Tell me to start a fresh session and say "Use systems thinking on this problem: ...".

The skill folder and the instruction block are independent. Installing one does not require the other.
