# Second-Order Thinking: check the whole (ch 2, 5, 6, 9)

> **Standing rules (they travel with this file):**
> - book tools, traced forward round the loops; *(our rule)* no 5 whys and no tracing back to one root cause;
> - frame the mess before designing (the gate);
> - every number is sourced or recomputed, and every estimate or threshold shows its basis (a count or a stated calculation; with none, "baseline first"); the text matches the table; dates come from a date tool (none available: no weekday, marked unchecked);
> - plain words for the owner: no book labels (Type I/II/III, "serve and police") and no case names;
> - scale the card to the problem: a small business or a single job gets about one screen per stage;
> - one visual, then 2–5 lines, then one question.

Contents: Purpose · When to Use · Prerequisites (incl. standalone spec collection) · Steps 1–6 (dissolve · consequence trace · levers · structure · compatibility · re-score) · Output · Example

## Purpose

Test a design or an existing idea against the whole system it joins. A part improved on its own can make the whole worse (p. 225). Success is a property of the interactions, so manage those rather than the actions (p. 69).

## When to Use

- Stage 3 of a design run
- On its own, when the owner brings an idea or plan and asks "does this fit" or "what could this break"

## Prerequisites

- **Desired specs.** On a design run they come from the design card. On the standalone route ("does this fit"), collect them here instead and never open `interactive-design.md`:
  - list the owner's stated limits for this task, in their words;
  - add what each affected stakeholder (clients, team, partners) expects, and mark any expectation nobody actually stated as an assumption;
  - check the set agrees with itself, and flag any two that pull against each other.
- A mess card if one exists. Without one, treat the map nodes as the parts.

## Steps

```
Progress:
- [ ] 1 Dissolve check: every theme and part
- [ ] 2 Consequence trace: follow each first effect forward, then four questions over time
- [ ] 3 Lever table: control / influence / appreciate
- [ ] 4 Structure: implicit functions, serve vs police, integration, contribution
- [ ] 5 Compatibility: vertical, horizontal, temporal
- [ ] 6 Re-score T1 (or the owner's idea) after the check
```

### Step 1: Dissolve check (ch 5)

For each mess theme, and each part of the system the idea touches, mark one of:
- **dissolved**
- **eased:** a compromise, or a hold that keeps the theme down while the mess stays (the book's "resolve" and "contain", pp. 128, 271; a mess can't be partly dissolved, p. 191)
- **new conflict**

Add a one-line reason to each. Use the owner's map; without one, sketch the parts of the business (getting clients, selling, delivering, getting paid) plus the owner's hours, per SKILL.md "Applied to your business". Include work already in flight for the same people. What happens to a **new conflict** depends on the route:
- **Design run:** it sends the design back to `interactive-design.md`, at most twice.
- **Standalone route:** it goes to the owner as an open conflict. Offer a full design run, which starts at `formulate-the-mess.md`.
- **Either route:** if the check shows the mess itself was framed wrong, say so and go back to `formulate-the-mess.md`. The problem may be redefined as the design evolves (p. 160).

### Step 2: Trace the consequences forward (ch 2, pp. 71–72; ch 6, pp. 135–145)

Start from what T1 (or the owner's idea) changes first, and follow each effect forward until it comes back round. One event has several effects, each arriving at its own time and often somewhere else, and they can return to change what started them (p. 71). Keep it to 3–5 rows:

| First effect | Lands on (stock or actor) | Up / down | Lag | What it sets off next | Closes which loop (R/B), or hits which limit | Stops if we stop? |
|---|---|---|---|---|---|---|

**Draw it, the way the book draws its cause-and-effect maps** (welfare and smoking, pp. 72–73; the failing product division, pp. 187–188): start from T1's first effect (not a copy of the mess map), make each effect an arrow to the next, and follow it until an arrow comes back to where it started. Put each lag on its arrow, label each loop R or B, and show weak links in red. Lay it out in two lanes from the first change: soon (days to weeks) above, later (months) below, each arrow ending on the stock or actor it hits. Outline in red any effect that helps soon and hurts later, because those are the effects that mislead (p. 73). Show one, not both: where the app can draw, the drawing is the check stage's one visual, with Step 1's new conflicts marked on it in red; otherwise show the table.

- **Follow each row,** saying why each arrow happens, until it closes a loop, hits a limit (a stock that runs out, a capacity), or reaches a link nobody knows. Write "unknown" rather than guessing the link.
- **Stocks** are what accumulates: hours, client trust, backlog, referrals. Only a flow changes a stock.
- **Project the stock that runs out** (usually the owner's hours) from today's real counts to the end of the longest lag in this trace, and show the sum; measure-and-learn Step 3 sets the read date on or after it. When a loop grows against a limit, draw the limit as a dotted line beside the projected path, and name the shape: it levels off, it overshoots and swings, or it collapses because the growth wears the limit down (p. 137). When loops interact in a way that could change the decision, or capacity binds, build a small model from real counts instead of guessing (pp. 142–144, 149).
- **Improve the weakest link first,** and don't overbuild the other stages (pp. 149–150).

Then ask four questions over time:
1. **Repeat it:** if this runs every week for a year, what piles up? (p. 185)
2. **Re-rank it:** which effect matters most now, and which by the end of the longest lag? (p. 71)
3. **Undo it:** where a row's last column says no (effects can outlive their cause), try T1 on one segment first (pp. 71, 271, 284).
4. **More of it:** is more still better, or does it turn harmful past some point? (Conclusion, p. 359)

Check the four backfire patterns as you go: a fix that moves the failure somewhere else (p. 151); a correction made before the delay has passed, which makes the result swing (p. 135); growth that eats its own capacity, then overshoots and collapses (p. 136); and a roughly 10x change in a key variable, which turns known facts false (pp. 75–76).

Each traced effect that hurts a spec goes into Step 6; the bet watches that spec at the effect's lag.

### Step 3: Lever table (ch 2, pp. 52–55)

| Lever | Control / Influence / Appreciate | Who else produces the result | Why they'd act (rational / emotional / cultural) |
|---|---|---|---|

- **Control:** the owner's action is enough.
- **Influence:** the owner is one of several producers. Design for the other producer instead of forecasting them.
- **Appreciate:** it affects the owner but can't be moved. Never make it the goal; plan around it, or find a way to use it.

### Step 4: Structure (ch 7, 9)

- Every implicit function of a replaced part has a new owner.
- **No part both serves and polices** (pp. 218–219, 223). *(our rule)* For AI parts this extends to grading: no part grades its own work. When one does either, split the two jobs and measure each one separately.
- **Integrate what you add.** When the design adds parts (skills, agents, steps), name what holds them together: one module, a shared decision rule, or one owner of the linked work. A coordinator placed over separate parts isn't integration. Check the new part fits how decisions and rewards already work (pp. 96–97, 152–153, 161).
- Score each part on its own result **plus** what it adds to the others, never on its size (p. 224).

### Step 5: Compatibility (ch 7, pp. 173–179)

- **Vertical:** a part wins only when the whole wins.
- **Horizontal:** one part's success must not mean another's failure. People survive conflicting criteria by not taking them seriously (p. 177); AI agents are likely to follow them literally *(our inference)*, so conflicts must be fixed in the design.
- **Temporal:** don't win today at the future's cost. How past clients were treated sets the trust of present ones.

### Step 6: Re-score after the check

Carry every finding through to the scores and the recommendation:
1. Map each new conflict, red weak link, backfire risk and harmful traced effect (Step 2) to the spec it hurts. If no spec covers it (often the owner's hours or the team's capacity), add that spec and score it.
2. Re-score every row, not only T1: the current path, each option, the ideal and T1 (on the standalone route, the owner's idea). A spec touched by a finding can't stay a pass: mark it partial or fail, with the reason. Show the before → after.
3. Mark a theme "dissolved" only when T1 itself removes it, not a later version.
4. **Verdict: must-pass cells first, then count.** Must-pass specs are a limit the owner stated, or a spec the whole fails without (marked in interactive-design Step 2; on the standalone route, mark them here).
   - Compare the must-pass cells of T1 and every other row before anything else. A cell nobody can check yet is "unknown", never a pass; an unknown on a must-pass spec counts as a partial.
   - A fail on a must-pass spec decides against that row on its own, and passes elsewhere never outvote it. A partial makes the row conditional: name what must change for it to pass, make that the verdict's condition, and give it its own signal in the bet.
   - If any row matches or beats T1 on the must-pass cells, the verdict opens "On today's scores, T1 does not beat <row>", then says what T1 needs. A want spec or an unknown can appear only as the condition under which T1 would win, never as the reason it wins now.
   - If every row fails a must-pass spec, say the design isn't ready or the limit needs talking through with the owner.
   Then give the counts (passes / partials / fails / unknowns) for T1 and the strongest other row as a summary. The verdict must agree with the table: a reason for preferring T1 that isn't a spec either becomes a spec and is scored, or is dropped. Model: "On today's scores, the first version does not beat the hire: its cost against the limit is unknown. It wins once <condition>." *(our rule: the pass/partial/fail table is our device; the book uses specs to steer the design with the people involved, and warns against scoring factors one at a time, pp. 138–139, 159.)*
5. Give each spec T1 fell on its own signal in the bet (measure-and-learn Step 3).

If the check found nothing, one line says so.

## Output

```
CHECK TABLE: <theme/part | dissolved / eased / new conflict | reason>
CONSEQUENCE TRACE: <the drawing: the chain closing into loops, a delay on each arrow (where the app can't draw: the 3–5 rows)> · stock that runs out: <today → read date, with the sum> · repeat / re-rank / undo / more of it: <one line each, where it changes the design>
WHAT ELSE COULD BREAK: <2–4 lines, only what changes the design or the bet: a lever someone else holds and why they'd act, a part that would win at another's cost, a win today at the future's cost>
STRUCTURE: implicit functions → new owner <…> · any part that both does the work and checks it <…> · what integrates the new parts <…>
RE-SCORE: <finding → spec it hurts | every row before → after | reason>, or "no change"
VERDICT: <must-pass specs: T1 passes all | fails <spec>> · counts T1 vs <strongest other row> · <T1 wins | T1 loses: change, or what T1 needs>
```

Always show the consequence trace. Work Steps 3–5 fully, but show only what changes the design or the bet, as the one "what else could break" list; tables that repeat the actor table or confirm nothing are left out, and so is any "what else could break" or STRUCTURE line that repeats the trace. The trace drawing is that one visual (inline where the app can draw one, otherwise the trace table), with weak links and new conflicts in red; ask one question.

## Example

Read `references/book-cases.md` § "The welfare loop" before drawing the trace, and § "The telephone company" before writing the table. Copy the way it found that every local fix moved the failure, that rewards for volume bred the conflict, and that intake had to be capped by spare capacity.

---
**Last Updated:** 2026-10-18
