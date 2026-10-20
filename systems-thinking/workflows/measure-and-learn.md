# Success Scorecard: measure and learn (ch 6.3, 7, 9)

> **Standing rules (they travel with this file):**
> - book tools, traced forward round the loops; *(our rule)* no 5 whys and no tracing back to one root cause;
> - frame the mess before designing (the gate);
> - every number is sourced or recomputed, and every estimate or threshold shows its basis (a count or a stated calculation; with none, "baseline first"); the text matches the table; dates come from a date tool (none available: no weekday, marked unchecked);
> - plain words for the owner: no book labels (Type I/II/III, "serve and police") and no case names;
> - scale the card to the problem: a small business or a single job gets about one screen per stage;
> - one visual, then 2–5 lines, then one question.

## Purpose

Decide what success means before choosing a number, and write the recommendation down as a bet that a later decision can learn from. The way you keep score defines the game (ch 9, p. 228).

## When to Use

- Stage 4 of a design run
- On its own, for "how do we measure this", "design the scoreboard", or any recommendation that needs its bet recorded

## Prerequisites

- A design card or a clear recommendation
- Real counts with sources, per SKILL.md "Applied to your business"

## Steps

```
Progress:
- [ ] 1 Criteria before measures
- [ ] 2 Viability check (scorecards and dashboards only)
- [ ] 3 Bet card
- [ ] 4 Log the bet
- [ ] 5 Read it on the date, on a miss, or on an early warning
```

### Step 1: Criteria before measures (pp. 225–228)

- Write what success means and why it matters. Then choose how to count it, and iterate between the two.
- **Relevance beats accuracy.** A precise count of the wrong thing backfires: it rewards what is easy to measure, usually inputs or volume (p. 196).
- An emergent result (growth, trust, a working AI Employee) needs **two or more signs**. Growth alone can come from moves that ruin the business (p. 226).
- A measure must cost less than the information it gives. Pooled judgment from varied judges is allowed (p. 227).
- **Flag any convention being treated as a cause.** An allocation or attribution rule can trigger cut after cut. The book's supermarket chain shrank itself out of the market this way (pp. 227–228).

### Step 2: Viability check (Table 9.1, p. 228; scorecards only)

Cross three rows (throughput, synergy, latency) with four columns (structure, function, environment, process). Any empty cell is a blind spot. It's usually in latency: early warning, bench strength, planning. List the empty cells and say which one matters most.

### Step 3: Bet card (pp. 153–154, 168–169)

```
BET: <the recommendation, one line>
ASSUMPTIONS: <what must be true>
EXPECTED EFFECT: money <…> · people, incl. the owner's hours <…> · customers <…>
BASELINE: <what, from YYYY-MM-DD to YYYY-MM-DD> · CHANGE STARTS: <YYYY-MM-DD, after the baseline ends> | none needed (<why>)
CAN IT TELL: no change ≈ <range> · works ≈ <range> · separate: yes | no (then lengthen the window)
PROVES IT WRONG: <the signal and its threshold, placed between the two ranges, with its basis>
ALSO WATCH: <one signal per spec T1 fell on in the check, read at the lag of the effect behind it>
READ ON: <the owner's local date, YYYY-MM-DD, on or after the longest lag in the consequence trace (no trace: after the delay)> · don't re-tune the design before then
EARLY WARNING: <who watches what, and how often: each assumption, whether it was done as designed, one early sign that moves before the result, each with its threshold and basis> · an assumption or the implementation breaks: act at once · the early sign moves the wrong way: run Step 5's four checks, no re-tune before READ ON
SOURCES: <where each number came from>
NUMBERS: every figure in the answer, each with its source or basis (estimates and thresholds included; with no basis, "baseline first") · derived numbers recomputed · dates <from a date tool | unchecked>
```

The read date sits **after** the delay: re-tuning the design before the effect can show makes a balancing loop swing (p. 135). That rule covers the design, not the evidence. Watch the assumptions, the implementation and the early signs the whole time, and act at once when an assumption or the implementation breaks (p. 169). An early sign moving the wrong way triggers Step 5's four checks, not a re-tune.

**Before showing the bet, check it can tell you something** *(our rules, in the spirit of the book's relevance over accuracy)*:
- **Baseline first, change second.** If the bet needs a baseline, it ends before the change starts. Give both dates; a baseline that runs alongside the change, or uses up the window, measures nothing.
- **A window that can separate the outcomes.** Write what the signal would show with no change (from the baseline's normal week-to-week swing) and what it would show if the bet works. If those ranges overlap, lengthen the window or say the bet can't be read yet. Small counts need longer windows.
- **Put "proves it wrong" between those two ranges,** not at the target and not at the edge of the no-change range (such as the baseline's worst week). A line at the target fails a bet that worked about half the time; a line at the edge lets a change that did nothing pass about half the time.
- **One change per count.** If anything else lands in the same count (another campaign, a broadcast), name it or separate it.
- **Add a signal for each spec T1 fell on** in check-the-whole Step 6, read at the lag of the effect behind it.
If the owner sets the threshold themselves, use theirs and flag a weak window once.

### Step 4: Log the bet

- Show the bet card. If the owner keeps a decisions or task log as a file in their folder, offer to append it there, and write it only on the owner's yes. An append-only log is the book's "read-only memory": assumptions nobody can rewrite later.
- The bet is labeled as a recommendation. Every number and fact in it names its source (the owner's words or a named file), and unknown stays unknown. Never write it into another app.

### Step 5: Read it on the date, on a miss, or when an early warning fires (p. 169)

Before redesigning, check all four causes of a miss. This order puts the cheapest check first *(our rule)*:
1. **Data:** was the number right?
2. **Implementation:** was it done as designed?
3. **Decision:** was the bet wrong?
4. **Environment:** did something outside change?

A plateau in the results means the slack is used up. Redesign rather than tune harder (ch 1.7, ch 6.3).

## Output

A measure sheet (criteria → measures → the behavior each one rewards), the viability gaps when relevant, and the bet card, logged or offered for logging.

## Example

Read `references/book-cases.md` § "The telephone company", the part on what changed. Copy how the reward moved from volume to results, and how intake was tied to spare capacity.

---
**Last Updated:** 2026-10-18
