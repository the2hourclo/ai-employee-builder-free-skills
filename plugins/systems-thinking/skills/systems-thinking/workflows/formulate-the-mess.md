# Bottleneck Discovery: formulate the mess (ch 8: search, map, tell the story)

> **Standing rules (they travel with this file):**
> - book tools, traced forward round the loops; *(our rule)* no 5 whys and no tracing back to one root cause;
> - frame the mess before designing (the gate);
> - every number is sourced or recomputed, and every estimate or threshold shows its basis (a count or a stated calculation; with none, "baseline first"); the text matches the table; dates come from a date tool (none available: no weekday, marked unchecked);
> - plain words for the owner: no book labels (Type I/II/III, "serve and police") and no case names;
> - scale the card to the problem: a small business or a single job gets about one screen per stage;
> - one visual, then 2–5 lines, then one question.

Contents: Purpose · When to Use · Prerequisites · Steps 1–7 (restate · search · pause · map · second-order machine · story · GATE) · Output: the mess card · Traps · Example

## Purpose

Build a shared picture of why the system behaves the way it does, before any solution exists. A mess is a set of problems that keep each other alive. Remove one piece and the rest rebuild it, so it can't be fixed locally (pp. 182, 191). The output is the thing the owner recognizes and says "yes, that's it" to.

## When to Use

- A "why" question, a recurring problem, a stall, or a fix that didn't hold
- The first stage of every design job (a lighter pass is fine when the system is small)

## Prerequisites

- The request in the owner's words
- Access to real counts (the owner's tools or words) and to in-flight work, per SKILL.md "Applied to your business"

## Steps

```
Progress:
- [ ] 1 Restate the problem with no solution in it
- [ ] 2 Search, pass 1 (three inquiries)
- [ ] 3 Pause: write the assumptions, then run pass 2 on the gaps
- [ ] 4 Map 3–7 themes and how they interact
- [ ] 5 Name the second-order machine
- [ ] 6 Tell the story
- [ ] 7 GATE: the owner recognizes it
```

### Step 1: Restate the problem

Write the problem as the current behavior. Reject the three faulty frames that keep reproducing the same problem (ch 7, pp. 166–167):
- **A deviation from normal** ("signups dipped")
- **A lack of resources** ("not enough time / money")
- **A missing solution we already own** ("we need a new page / skill / price")

If the request arrived in one of these shapes, say so in one line and restate it.

### Step 2: Search, pass 1 (from a high altitude, pp. 183–185)

Run all three inquiries. Keep pass 1 wide and shallow.

**Systems analysis.** A snapshot with no value judgments. Fill the actor table:

| Actor | Wants (stake) | Controls | Influences | Why they act: rational / emotional / cultural |
|---|---|---|---|---|

The "why" is required for every actor the problem touches, the owner included: a design that ignores motives fixes the mechanics while the motive rebuilds the behavior (ch 2). A blank "why" is a question for the owner, or a labeled assumption in an unattended run.

Then add one line each:
- **Function:** what the system produces, for whom, and why
- **Process:** how the output gets made, and what it costs, including the owner's hours

**Obstruction analysis.** Scan the five dimensions for scarcity, maldistribution or insecurity:
- wealth
- power (decisions)
- knowledge
- beauty (belonging, excitement)
- values (conflict)

Ask about each of these: the measure of success, the reward, the early warning, feedback delays, the bottleneck, where the money comes from, policies that contradict each other, and what is **not** being done. Organizations fail more from omission than commission (p. 194).

**System dynamics.**
- Critical past events, and plausible future ones
- Drivers written as "from → to"
- Every fix already tried, and what it did
- The pattern over time: growth, S-curve, swing, plateau or slow decline. A slow decline is the most dangerous, because the strength to respond is gone before anyone notices (p. 77).
- Any loop you can see

**Real counts and in-flight work** are part of the system. Pull the numbers with their source, and ask once what else is already running for the same people.

### Step 3: Pause, then pass 2 (p. 186)

Write the working assumptions about the critical drivers and how they connect, plus a short list of gaps. Run pass 2 on the gaps, one level further out (the system that contains this one). Stop when a pass adds nothing new.

### Step 4: Map the mess (pp. 186–188)

- Group the findings into **3–7 themes**. Each theme is a cluster of behaviors that produce something together.
- Give each theme its evidence: a count, or how widespread it is. A one-off isn't a theme.
- **Map, not list:** before showing it, check that every theme links to at least one other theme and that the outcome feeds back into one. Arrows that only point at the outcome make a list of separate causes, not a map (pp. 138–139).
- **Draw** how the themes feed each other, with arrows and loop labels (R = reinforcing, B = balancing). Where the app can draw an inline visual, use it; elsewhere, use a small mermaid or ASCII loop.

### Step 5: Name the second-order machine (p. 188)

Name the simple, innocent assumptions that keep regenerating the themes. Check the three usual sources:
- **A winning formula pushed too far** (suboptimization: a strength turned into a weakness)
- **A changed game:** success changed the problem
- **The wrong measure or reward:** something easy to count, rewarded for volume

Frame it as the legacy of past success, never as someone's failure (pp. 191–192).

### Step 6: Tell the story (p. 189)

Write 3–6 sentences on where today leads if nothing changes. Assume everything that can go wrong does, at the same time. Name each stakeholder's stake, influence and interest. Blame no one. This is an early warning, not a forecast.

### Step 7: GATE — the owner recognizes it

Show the mess card. Ask one question: **"Is this the mess?"** Revise until they recognize it; the book's validity test is the "aha" from the people inside (p. 186). **Propose no solutions in this workflow.** Only a recognized mess moves to `interactive-design.md`.

Unattended runs (no person in the session: a scheduled task, or a helper with no channel to the owner; never an attended chat) label the card "UNCONFIRMED", list the assumptions it rests on, and continue.

## Output: the mess card

```
MESS: <problem as current behavior, no solution in it>
ACTORS: <actor | wants | controls | why they act (rational / emotional / cultural)>, the owner included
THEMES (3–7): <theme — evidence with source> …
INTERACTIONS: <the drawn map; loops labeled R/B>
SECOND-ORDER MACHINE: <the innocent assumptions + which source>
STORY: <3–6 sentences, no blame>
ASSUMPTIONS / GAPS: <what this rests on; what is still unknown>
NUMBERS: every figure in the answer, each with its source or basis (estimates and thresholds included; with no basis, "baseline first") · derived numbers recomputed · dates <from a date tool | unchecked>
STATUS: confirmed by the owner (<their words>) | UNCONFIRMED
```

## Traps

- Proposing a fix while still defining the problem
- An actor table with no "why", which turns the design into mechanics
- Listing causes as if each one acts alone, or chasing back to one root cause (tracing effects forward round the loops is fine)
- Blaming people for what the system produces; denial keeps the mess alive (p. 197)
- Drowning in data instead of synthesizing
- Presenting the mess as a forecast

## Example

Read `references/book-cases.md` § "The utility mess" before writing the card, and match its shape, not its count: themes grounded in evidence, a drawn interaction map, one named second-order machine, and a story told as the cost of past success.

---
**Last Updated:** 2026-10-18
