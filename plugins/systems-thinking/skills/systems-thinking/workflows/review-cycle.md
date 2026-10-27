# Compound Engineering: the review cycle (ch 7, pp. 168–169; ch 6, p. 135)

> **Standing rules (they travel with this file):**
> - book tools, traced forward round the loops; *(our rule)* no 5 whys and no tracing back to one root cause;
> - frame the mess before designing (the gate);
> - every number is sourced or recomputed, and every estimate or threshold shows its basis (a count or a stated calculation; with none, "baseline first"); the text matches the table; dates come from a date tool (none available: no weekday, marked unchecked);
> - plain words for the owner: no book labels (Type I/II/III, "serve and police") and no case names;
> - scale the card to the problem: a small business or a single job gets about one screen per stage;
> - one visual, then 2–5 lines, then one question.

Contents: Purpose · When to Use · Prerequisites · Steps 1–6 · Output: the review card · Guardrails · Example

## Purpose

Run the method as a loop, not a one-off. The book's ideal design is a learning system: it writes down what it expected, watches the signs, and corrects itself when the results come in (pp. 168–169). This route is the part that comes back. On a schedule, it reads the scorecard and every open bet, and decides for each one whether to wait, act, keep it, or redesign. Re-tuning before a change can show makes results swing (p. 135), so in most weeks most bets get "wait".

## When to Use

- An agent running the skill on a cadence, usually weekly: a scheduled task, or another agent the owner runs, that can read the owner's files
- The owner asks to "check our bets", "see what's due", or "run the review cycle"
- Not for a new problem someone brings in (that's the mess route), and not for building a dashboard

## Prerequisites

- **The KPIs in scope**, each with its source: the owner's connected tools or a file they keep. With neither, the number is "unknown".
- **Targets:** a threshold in the owner's own scorecard, or a target the owner set in words you can quote.
- **The open bets:** the decisions or task log the owner keeps as a file. A bet with a later "BET CLOSED" entry is closed.
- **A runner that can't read the log** reports "bets: unreadable here", never "no bets".
- **Today's date** from a date tool. With none, say the dates are unchecked.

## Steps

```
Progress:
- [ ] 1 Check the data is fresh and whole
- [ ] 2 List the open bets by their labels
- [ ] 3 Before a read date: early warnings only
- [ ] 4 On or after a read date: read it
- [ ] 5 A red KPI with no bet: frame it, then stop
- [ ] 6 Log, hand over, and report on one screen
```

### Step 1: Fresh and whole data

For each KPI, check when it last updated, whether its status says complete, and whether any days are missing or doubled. Read the KPI only if its own fields are complete for the window, and name the days you dropped; otherwise read nothing from it and report it under "data" (the four causes of a miss start with data: `measure-and-learn.md` Step 5). Bad data still there at the next review becomes its own Step 5 item.

### Step 2: The open bets

List every open bet by its labels: READ ON, PROVES IT WRONG, CAN IT TELL, ALSO WATCH and EARLY WARNING (the bet card, `measure-and-learn.md` Step 3). A bet missing READ ON or PROVES IT WRONG can't be read: name the missing part under NEEDS THE OWNER. Never invent one.

### Step 3: Before a read date

Follow the bet's EARLY WARNING line (`measure-and-learn.md` Step 3). If an assumption or the implementation broke, hand it over at once (Step 6). If the early sign moved the wrong way, run the four checks (`measure-and-learn.md` Step 5). Otherwise the answer is "wait"; never re-tune before the read date.

### Step 4: On or after a read date

Compare the signal with the bet's CAN IT TELL ranges and its PROVES IT WRONG line, then read each ALSO WATCH signal at its own lag.
- **Keep:** it worked and every ALSO WATCH signal held. Say what to keep doing, and close the bet ("BET CLOSED: … | keep").
- **Worked, but an ALSO WATCH signal broke or can't be read:** keep the bet open. A broken one is a miss on that spec: follow `measure-and-learn.md` Step 5 for it. One that can't be read goes under NEEDS THE OWNER. For example, sign-ups beat their "works" range but the owner's hours went past the stated limit: the bet stays open, and the hours go to Step 5.
- **Missed, or a plateau:** follow `measure-and-learn.md` Step 5. A plateau calls for a redesign, which goes to the owner as an offer.

### Step 5: A red KPI with no bet

A KPI is red only when it is past its warning threshold in the owner's scorecard, or past a target the owner set in words you can quote. With neither, log "no target: baseline first" and move on.

For a red KPI with no bet, draft a mess card with `formulate-the-mess.md` Steps 1–6, mark it UNCONFIRMED, and **stop**. The unattended "continue" doesn't apply on this route: no design and no bet. Watch for the same fix recommended again and again with no owner and no read date. That repetition is part of the mess, not a plan.

### Step 6: Log, hand over, report

- **Log** each decision as one line in the owner's decisions log, and write it only on the owner's yes. In an unattended run, write the review card only to the file the owner named when they set up the schedule; with none named, keep it in the run's output. Without a log the owner allowed, a kept bet can't be closed and comes back next run; say so once on the card.
- **Hand fixes** to the agent that owns the surface, inside its decision rules (`interactive-design.md` Step 4). Anything that sends, deploys, publishes, changes a price or edits a skill waits for the owner.
- **Anything that needs the owner** goes under NEEDS THE OWNER, and the run carries on. Never wait for an answer or guess one. The review card is the run's output.
- **Report on one screen:** what is due, what moved, and what needs the owner. If nothing needs the owner, say so in one line.

## Output: the review card

```
REVIEW: <date, from a date tool> · scope <KPIs> · data <fresh | stale / partial / doubled: which days dropped>
BETS: <bet | read date | wait / act: … / keep / open: ALSO WATCH <signal> broke or unreadable / missed: cause / redesign | signal, with its source> | bets: unreadable here
RED, NO BET: <KPI | threshold and its source | UNCONFIRMED mess card | handed to whom> | no target: baseline first
NEEDS THE OWNER: <decisions only the owner can make, and bets that need another reader> | none
NEXT REVIEW: <date>
```

## Guardrails *(our rules)*

- **Read only.** The review reads the KPIs and the bets and writes only its log lines. It never sends, deploys, publishes, changes a price or edits a skill, this one included.
- **The builder doesn't grade.** If this runner logged the bet or handed over the change it is reading, list that bet under NEEDS THE OWNER as "needs another reader" (`check-the-whole.md` Step 4).
- **No re-tuning before the read date.** "Wait" is usually the right answer.
- **One screen.** The owner's hours are the stock this route protects.
- **Before it runs on a schedule:** three trigger tests ("check our bets" runs it; "show my dashboard" doesn't; "review the scorecard" is the borderline case) and one unattended run. Run these with outward actions disabled. Scheduling itself needs the owner's separate approval and a runner that can read the allowed log; this package does not create a schedule.

## Example

Read `references/book-cases.md` § "The telephone company", the part on what changed. The review cycle is the part of that redesign that kept checking: intake held to spare capacity, and reward tied to results.

---
**Last Updated:** 2026-10-20
