# Install Systems Thinking

## Claude Code: plugin setup

Free hosted Systems Thinking access is pending deployment and verification. The standalone files below are available now. Once free access is verified, prefer the plugin so Skill content is fetched when needed. Plugin package updates are separate; third-party marketplace auto-updates are off by default until you enable them.

Copy this prompt into Claude Code in the project you want to use:

```text
Help me install AI Employee Builder from https://github.com/the2hourclo/aieb-thin-plugin in this project. First check whether ai-employee-builder@aieb-thin-plugin is already installed and preserve a working setup. If missing, show these commands and any approval needed:
claude plugin marketplace add https://github.com/the2hourclo/aieb-thin-plugin
claude plugin install ai-employee-builder@aieb-thin-plugin --scope local
Use secure browser sign-in if needed; never ask for a key in chat. Fetch Systems Thinking and verify access before saying setup is complete. If unavailable, stop and explain. Do not start a paid trial, enable an optional ledger, install a duplicate local Skill, change my repository instructions, or connect other services. Tell me when to run /reload-plugins or start a fresh session.
```

## Optional standalone snapshot

Copy this prompt into Claude Code or Codex after giving it this repository link:

```text
Inspect https://github.com/the2hourclo/systems-thinking. Install only its systems-thinking/ folder into this project's .claude/skills/systems-thinking/ for Claude Code, or .agents/skills/systems-thinking/ for Codex. Choose only the runtime I am using. Do not execute repository scripts. Check for an active plugin or existing local copy first; show differences and ask before replacing anything, and avoid duplicate active copies. Verify SKILL.md and every referenced workflow/reference file. Do not change CLAUDE.md or AGENTS.md without my separate approval. Do not install other skills, create schedules, send messages or change external services. Tell me to start a fresh session and say "Use systems thinking on this problem: ...". Report compatibility or access failures honestly.
```

A local copy is a snapshot. Review repository changes before updating it. Claude-specific compatibility has not been verified for this release.

## Optional Think in Systems

This short instruction block works independently of both the plugin and the full Skill. In Claude Code, use the project's `CLAUDE.md`; in Codex, use `AGENTS.md`. In ordinary ChatGPT Projects, paste the block into the project's instructions instead. Keep all existing instructions.

Before an assistant edits your repository instruction file, it must inspect it for the marked block or an equivalent set of instructions. If equivalent instructions already exist, leave them alone and explain; do not append a duplicate. Otherwise show the exact proposed addition and get your approval before editing or creating `CLAUDE.md` or `AGENTS.md`. Do not replace unrelated content. Re-read the result to verify the approved block appears once and existing instructions remain. This is optional; installing the plugin does not authorize an instruction-file edit.

Copy the unchanged block below, also available in [THINK-IN-SYSTEMS.md](THINK-IN-SYSTEMS.md):

```markdown
<!-- BEGIN THINK IN SYSTEMS -->
## Show me first (how to answer me)

When we plan, decide, compare options, review, or track progress together, show me before you tell me:
- one visual first (an inline visual where this app can draw one, otherwise a small table or diagram), then 2–5 lines of text and ONE question;
- options appear as cards or a short list I can pick from;
- multi-step work keeps one progress view: in progress first, then done, then blocked.
Skip this for one-line facts, code and terminal work, and finished deliverables such as emails, scripts and files.

## Think in systems (how to judge changes and big ideas)

Before you change anything (a file, a skill, an instruction, a setting, a plan), check that it fixes a real problem worth fixing: what actually went wrong, how often, and what it costs if we leave it. If it isn't worth it, say so and leave it alone.

Never judge an idea on its own. Judge it as a part of the whole (method: Jamshid Gharajedaghi, *Systems Thinking*):
1. Frame the problem without a solution in it, and name what keeps recreating it.
2. Design the ideal first, then the closest version we can ship now.
3. Check it against the whole: my stated limits, every other part of this project it touches (files, skills, instructions, tools), my time, and work already in progress.
4. State the bet: what you expect, what would prove it wrong, and when we'll know.
Skip this for work against a clear spec, plain facts and explanations.
<!-- END THINK IN SYSTEMS -->
```
