# AI Employee Builder Free Skills

Free Claude skills you can install one at a time. Each one is its own plugin, so install only the ones you want.

| Skill | What it does |
|---|---|
| [Skill System Creator](plugins/skill-system-creator/) | Hand Claude your golden standard (your best examples, how you do the job, and when to use it). It interviews you, builds the skill, then grows it into a skill system that stops for your yes. |
| [Systems Thinking](plugins/systems-thinking/) | Work one business problem through as a whole system before you change anything. |

## Install in Claude Code

Type this in Claude Code, either in the terminal or in the Code tab of the Claude desktop app:

```
/plugin install skill-system-creator --marketplace the2hourclo/ai-employee-builder-free-skills
```

On an older Claude Code, use two lines instead:

```
/plugin marketplace add the2hourclo/ai-employee-builder-free-skills
/plugin install skill-system-creator@ai-employee-builder-free-skills
```

Swap `skill-system-creator` for `systems-thinking` to install the other one. Run `/reload-plugins` afterwards, or start a new session.

Or paste this prompt and let Claude do it:

```text
Install the skill-system-creator plugin from the GitHub marketplace the2hourclo/ai-employee-builder-free-skills. Show me each command before you run it.
```

## Update

Run `/plugin marketplace update ai-employee-builder-free-skills`, then `/reload-plugins`.

## Using Codex, or no plugins?

See [INSTALL.md](INSTALL.md) to copy a skill straight into your project.

## What these free skills don't do

They build, run and fix skills. They don't add automatic checks, test sets, library audits or scheduling, which are the parts that keep a skill system reliable as it grows. Those, plus production-grade skills kept up to date, come with the AI Employee Builder plugin inside [AI Employee Builders](https://aiemployeebuilders.com/ai-employee-builders-invitation).
