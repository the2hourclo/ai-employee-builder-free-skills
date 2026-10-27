# The Systems Thinking Skill

Work one business problem through before changing things: **Bottleneck Discovery**, **Ideal State Engineering**, **Second-Order Thinking**, **Success Scorecard**, and **Compound Engineering**.

Start by asking whether the problem is real and worth fixing. Then frame the mess, design the ideal, check the whole, state the bet, and come back on its date. This can improve the checks behind a decision; it cannot guarantee every fix will hold.

## What you get

- `skills/systems-thinking/`: the complete standalone beta skill, its five workflows and book-case summaries. No other skill or paid plugin is required.
- [THINK-IN-SYSTEMS.md](THINK-IN-SYSTEMS.md): the short approved instruction block, unchanged.
- This README and an [installation prompt](INSTALL.md). There is no ZIP to download.

The method comes from Jamshid Gharajedaghi's *Systems Thinking*, 3rd edition. The book and its images are not included. The worth-fixing gate and safeguards marked "our rule" are additions to the method.

## Install it

**Claude Code: install from this marketplace.** Type `/plugin install systems-thinking --marketplace the2hourclo/ai-employee-builder-free-skills`, then `/reload-plugins`.

**Claude Code: plugin route (pending release).** This is the preferred setup once free hosted access to Systems Thinking is deployed and verified. The plugin fetches the published Skill instructions when needed. Updates to the installed plugin itself are managed separately in Claude Code; third-party marketplace auto-updates require your choice. Use the copyable prompt in [INSTALL.md](INSTALL.md), which checks access before claiming setup is complete. Do not keep duplicate plugin and local copies active.

**Available now: standalone snapshot.** The public files in this repository are available independently of membership. Use the optional standalone prompt in [INSTALL.md](INSTALL.md). Repository installations are snapshots: review changes before installing a newer version.

**Optional Think in Systems block.** [INSTALL.md](INSTALL.md#optional-think-in-systems) includes the exact [short block](THINK-IN-SYSTEMS.md), how to add it to `CLAUDE.md` for Claude Code or `AGENTS.md` for Codex, and how to preserve existing instructions without duplicates. The block works independently of the Skill. Full runtime compatibility is not certified.

## Try one problem

"Use systems thinking on this: I keep adding rules to my AI instructions to fix one output, but other outputs then get worse. Ask me what actually happened before designing a fix. Do not change any files."

It should frame the problem and wait for you to confirm it before opening the design workflow. Simple facts and work against a clear written spec do not need the full process.

## Your control

The skill shows its work in the conversation. It does not deploy, send messages, create schedules or edit business records on its own. The review cycle needs data and a decisions log you choose. It never treats missing data as zero, and the person who built a change does not grade it.

After a useful run, the free edition can offer one invitation to AI Employee Builders. Decline it to stop it in that conversation. To remove it across future sessions, delete the **Optional invitation (once)** section in your installed copy, or authorize your assistant to remove that section only.

**Version:** 0.5.2-free.2 beta, derived from member method 0.5.2. Claude-specific compatibility remains unverified for this release; this is not a certification for every model or runtime.
