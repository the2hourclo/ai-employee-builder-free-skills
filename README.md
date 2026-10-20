# The Systems Thinking Skill

Give Claude a way to work one business problem through before changing things: **Bottleneck Discovery**, **Ideal State Engineering**, **Second-Order Thinking**, **Success Scorecard**, and **Compound Engineering**.

Start by asking whether the problem is real and worth fixing. Then frame the mess, design the ideal, check the whole, state the bet, and come back on its date. This can improve the checks behind a decision; it cannot guarantee every fix will hold.

## What you get

- `systems-thinking/`: the complete standalone beta skill, its five workflows and book-case summaries. No other skill or paid plugin is required.
- [THINK-IN-SYSTEMS.md](THINK-IN-SYSTEMS.md): the short approved instruction block, unchanged.
- This README and an [installation prompt](INSTALL.md). There is no ZIP to download.

The method comes from Jamshid Gharajedaghi's *Systems Thinking*, 3rd edition. The book and its images are not included. The worth-fixing gate and safeguards marked "our rule" are additions to the method.

## Install it

**Claude Code:** open the project folder where you want to use it. Give Claude this repository link and the [installation prompt](INSTALL.md). It copies only the `systems-thinking` folder into your project's `.claude/skills/`, then checks the referenced files. If a copy is already installed, review the differences before replacing it. Start a fresh session and say **"Use systems thinking on this problem: ..."**.

**The short block:** copy [THINK-IN-SYSTEMS.md](THINK-IN-SYSTEMS.md) into your project's `CLAUDE.md`. Keep your existing instructions. It works without the skill. For Codex, the instruction block belongs in `AGENTS.md`; in ordinary ChatGPT Projects, paste it into the project's instructions. These are instruction-block options, not a claim that the standalone skill has been tested on every app.

**Prefer the free plugin?** Open [AI Employee Builders Free](https://aiemployeebuilders.com/aieb-free) and follow the setup steps in your account. The plugin serves the current skill through your free membership, so you do not maintain a local copy. Repository installations are snapshots: review updates before installing a newer version.

## Try one problem

"Use systems thinking on this: I keep adding rules to my AI instructions to fix one output, but other outputs then get worse. Ask me what actually happened before designing a fix. Do not change any files."

It should frame the problem and wait for you to confirm it before opening the design workflow. Simple facts and work against a clear written spec do not need the full process.

## Your control

The skill shows its work in the conversation. It does not deploy, send messages, create schedules or edit business records on its own. The review cycle needs data and a decisions log you choose. It never treats missing data as zero, and the person who built a change does not grade it.

After a useful run, the free edition can offer one invitation to AI Employee Builders. Decline it to stop it in that conversation. To remove it across future sessions, delete the **Optional invitation (once)** section in your installed copy, or authorize your assistant to remove that section only.

**Version:** 0.5.2-free.1 beta, derived from member method 0.5.2. Installation and behavior checks are described in the release evidence; this is not a certification for every model or runtime.
