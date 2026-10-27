# Ideal State Engineering: interactive design (ch 7: idealize, then approximate)

> **Standing rules (they travel with this file):**
> - book tools, traced forward round the loops; *(our rule)* no 5 whys and no tracing back to one root cause;
> - frame the mess before designing (the gate);
> - every number is sourced or recomputed, and every estimate or threshold shows its basis (a count or a stated calculation; with none, "baseline first"); the text matches the table; dates come from a date tool (none available: no weekday, marked unchecked);
> - plain words for the owner: no book labels (Type I/II/III, "serve and police") and no case names;
> - scale the card to the problem: a small business or a single job gets about one screen per stage;
> - one visual, then 2–5 lines, then one question.

Contents: Purpose · When to Use · Prerequisites · Steps 1–8 (purpose and functions · desired specs · shared assumption · idealize · successive approximation · score · target cost · hand off) · Output: the design card · Traps · Example

## Purpose

Design the system you'd want, rather than choose among the options already on the table. Picking the best given option repeats the assumptions they all share. Design challenges those assumptions to create new options (pp. 157–158).

## When to Use

After `formulate-the-mess.md`, once the mess card is confirmed (or marked UNCONFIRMED in an unattended run). Never open this file earlier; the gate is in SKILL.md.

## Prerequisites

- A mess card
- The owner's stated limits in their own words: every limitation they have given in this task or its source docs

## Steps

```
Progress:
- [ ] 1 Purpose and functions (explicit and implicit)
- [ ] 2 Desired specs from every stakeholder
- [ ] 3 Name the assumption all the options share
- [ ] 4 Idealize (three tests), sketch it, and write decision rules for AI-run parts
- [ ] 5 Realize by successive approximation: T1 and the constraint types
- [ ] 6 Score the current path, the options, the ideal and T1 against the specs
- [ ] 7 Target cost
- [ ] 8 Hand to check-the-whole.md
```

### Step 1: Purpose and functions (pp. 160, 169)

- **Purpose:** what this system does for the larger whole it belongs to, and its effect on each stakeholder in the actor table.
- **Functions:** list them all. For anything being replaced, list the **implicit** functions as well as the stated ones; a replacement that drops a function nobody wrote down breaks something quietly.

### Step 2: Desired specs (ch 7; cases pp. 271, 305, 341)

- Turn each stakeholder's expectations into specs that describe **the whole**. The owner's stated limits come first, in their words. Mark any expectation nobody actually stated as an assumption.
- Mark each spec **must pass** or **want**. A limit the owner stated, or a spec the whole fails without, is must-pass. Note which specs reinforce, complement or pull against each other (p. 159): pulling pairs get the added-dimension search below, and the verdict weighs the must-pass marks, not counts.
- Each spec should answer a theme or conflict from the mess. Butterworth wrote specs that way (p. 271).
- Check the specs as a set, the way the book checks decision criteria (pp. 121–124). They should:
  - agree with each other;
  - leave room for judgment;
  - state their assumption and the expected outcome.
- Where two specs pull against each other, look for the added dimension that makes them complements before compromising (ch 2.3, ch 5): put each spec on its own axis of a 2×2 and name the design in the high-high corner. With no design named there, the theme can only be eased, never dissolved (pp. 62, 129).

### Step 3: The shared assumption (p. 157)

List the options already on the table, including "keep the current path". Name the assumption they all share, and challenge it in one line.

### Step 4: Idealize (pp. 167–169)

Assume the system vanished last night while its environment stayed the same. Design what you'd build today. The ideal must pass three tests:
1. **Existing technology only,** on a platform that can take in new technology.
2. **Viable:** it sustains itself in today's environment, covers its own cost, and **dissolves the mess themes**.
3. **A learning system:** it records its assumptions, indicators and expected outcomes, so results can correct it.

Then:
- **Sketch it** as a concrete picture of the result, not a motherhood statement (p. 161).
- **Keep it modular.** Work that interacts closely sits in one module behind a thin, fixed interface. A cross-trained team beats a relay of hand-offs (pp. 161–164).
- **Decision rules for any part an AI Employee or helper will run** (pp. 121–124, 216, 302). Write them for the AI-run parts T1 keeps. For each one, write down:
  - what it may decide alone: how it does its job, never what the job is for;
  - the criteria it decides by, consistent with each other and agreed by the people who act on them, each with its assumption and its expected effect on money, people and customers, leaving room for judgment (pp. 123–124);
  - what goes to the owner: anything that touches another part's work, money, or a promise to a customer;
  - what it does when no rule fits: a call that touches another part's work, money or a customer promise, can't be undone, or reaches outside the business waits for the owner; any other call it makes, logs with its reason, and proposes as a rule for the owner to accept *(our rule)*;
  - whom it serves, what it hands over, and how its contribution to the other parts is measured (ch 9, pp. 214–224).
- **If even the ideal fails the tests,** the obstruction probably sits in the environment (p. 172). Say so, then look outward: which part of it could the owner influence, and who else would have to act? Call it "appreciate" only once influencing it has been tried or ruled out (Conclusion, p. 359).

### Step 5: Realize by successive approximation (pp. 170–173)

- Pick the closest version you can ship now (T1), and list what it gives up compared with the ideal.
- Type each constraint between T1 and the ideal:
  - **Type I:** can't move it now. Build toward it, and watch for it to lift.
  - **Type II:** short of time, money or knowledge. This becomes the plan, and T2 is the next approximation.
  - **Type III:** self-imposed. A habit or default (the second-order machine), and also mistrust, insecurity, people who gain from the old way, or missing buy-in (pp. 171–173). Ask for every reservation candidly first, then surface it openly with the owner: keep what serves the design and drop what feeds the mess. A worry takes real work with the people involved, not a decision alone.
- Tell the owner the types in plain words: "can't change it yet", "short of time, money or know-how", "a habit or worry we can work through".

### Step 6: Score *(our device; the book uses specs to steer the design, not to grade options)*

Build a matrix with these rows: the current path, every option on the table, the ideal, and **T1, the version you'll actually ship**. The desired specs are the columns. Mark each cell pass, partial, fail or unknown (a cell nobody can check yet is never a pass), with one reason, and mark the must-pass columns. Score T1 on its own: it usually passes fewer specs than the ideal, and that gap is the plan for T2. The recommendation is T1, so the ideal's passes never stand in for it. Show the matrix as a visual (inline where the app can draw one, otherwise a small table) and ask the owner one question.

### Step 7: Target cost (pp. 179–180)

The market sets the price; the design owns the cost. Work backward from what the user gives (price, attention, time) to what the design may spend, **including the owner's hours**. A design with no budget isn't finished. Take the current price from the owner's current offer, never from an old page or email.

### Step 8: Hand off

Pass the design card to `workflows/check-the-whole.md`, which re-scores T1 after the check. If the check finds a new conflict, come back here, at most twice; if it shows the mess was framed wrong, go back to `formulate-the-mess.md`.

## Output: the design card

```
PURPOSE: <for the whole; effect on each stakeholder>
FUNCTIONS: explicit <…> · implicit <…>
DESIRED SPECS: <numbered; the owner's first, verbatim; each marked must-pass or want>
SHARED ASSUMPTION: <the one all options share> → challenged: <…>
IDEAL: <sketch> · tests: tech ✓/✗ · viable + dissolves mess ✓/✗ · learning ✓/✗
T1 NOW: <closest shippable> · gives up: <…>
CONSTRAINTS: can't change yet <…> · short of time, money or know-how <…> (plan → T2) · a habit or worry we can work through <…> (raise with the owner)
DECISION RULES: <for each AI-run part T1 keeps: decides alone · decides by · goes to the owner · when no rule fits · serves whom, hands over what, measured how> | none (no AI-run part)
SCORE: <rows: current path · each option · ideal · T1> × specs
TARGET COST: <price/attention → allowed cost incl. the owner's hours>
```

## Traps

- Choosing among the given options and calling it design
- Scoring the ideal and recommending T1, so the table approves what it never tested
- A vague ideal ("a better funnel") instead of a concrete picture
- Dropping an implicit function of the thing being replaced
- Handing an AI-run part a job with no decision rules, so it either asks about everything or decides what it shouldn't
- Compromising between conflicting specs before looking for the redesign that dissolves the conflict
- Imposing a design on the owner instead of co-designing it from the sketch (p. 165)

## Example

Read `references/book-cases.md` § "Butterworth" before writing the card, and match its depth: specs that each answer a named conflict, and an architecture that dissolves the conflict rather than picking a side.

---
**Last Updated:** 2026-10-18
