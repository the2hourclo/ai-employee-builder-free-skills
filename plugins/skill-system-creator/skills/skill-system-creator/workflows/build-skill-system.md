# Build a skill system

A skill does one job. A skill system runs several jobs in order, passing each result to the next, and stops for the user's yes at the end. Example: a voice skill writes the long-form piece → a carousel skill turns it into slides → the user approves.

Plan the whole chain on paper first, then build and prove one step at a time. When a chain breaks, you need to know which hand-off broke, and you only know that if you proved each one as you went.

## 1. Read what you have first

List the skills that already exist. Steps of this job may already have a skill. Reuse it, don't rebuild it. Tell the user in 3 to 5 sentences what exists, what's missing and what you'll reuse.

## 2. Get the whole job

Ask: "Walk me through the whole job from start to finish. What starts it, what are the steps in order, and what's the finished thing at the end?" Get the real order, not a theory.

## 3. Draw the chain

Break the job into steps, one verb each. If a step needs "and", split it. Then fill this in and show it to the user:

| # | Step | Its one job | Gets | Hands on |
|---|------|-------------|------|----------|
| 1 | write the piece | write the long-form piece in my voice | the idea + notes | the finished piece |
| 2 | make the carousel | turn the piece into a cover + 6 to 8 slides | the finished piece | the slide files |
| 3 | your yes | show both and stop | the piece + slides | nothing, until the user says yes |

The "Hands on" column matters most. A fuzzy hand-off is the most common way a chain breaks, so name exactly what passes across: a file, a path, a list.

## 4. Decide where each step lives

For each step, pick one:

- **An existing skill.** One already does it, so the system calls it by name.
- **A workflow file inside the system's skill.** This is the default: the step only serves this job, and the user won't ask for it on its own.
- **Its own skill.** Only when other jobs will use it too, or the user will ask for it by name ("make a carousel"). The voice skill is a good example: it writes emails on its own AND feeds the carousel.

Fewer skills is usually better. Five separate skills for five steps tend to trigger on the wrong requests.

Show the table with this column added and ask: "Does this match how the work actually flows?" Don't build until they say yes.

## 5. Build one step at a time, in order

For each step:

1. Build it. A new skill goes through `author-skill.md`, with this step's row as the brief: don't re-interview from scratch, but ask how the user does this step if the golden standard doesn't say. A workflow file gets the same care: its job, its steps, and what it hands on.
2. Run it on its own, on a real input. Don't wire in a step that doesn't work alone.
3. Check its output matches the "Hands on" column. If it doesn't, fix the step, or fix the table and re-confirm.

## 6. Write the running order

The system's SKILL.md runs the steps in order:

```markdown
## Running it

When the user says "turn [idea] into a carousel":

1. Use the write-in-my-voice skill → the finished piece.
2. Run `workflows/carousel.md` on the finished piece → the slide files.
3. Check both against "what done looks like". Fix what fails, at most 2 rounds.
   If it still fails, show the user what's left instead of trying again.
4. Show the user the piece and the slides, and stop. Nothing gets posted without their yes.
```

Any step that can send work back must have a limit (2 rounds). When it's hit, hand the result to the user. Never loop a third time.

## 7. Run the whole thing with the user

Run it start to finish on a real input in front of the user. Watch each hand-off: did anything get lost between steps? Every correction they make goes into the step it belongs to. Then run it again.

It's done when the user has watched it run end to end on a real input and said yes.

Then tell them: "Start a new chat and ask for the whole job in your own words. It should run every step in order and stop for your yes."
