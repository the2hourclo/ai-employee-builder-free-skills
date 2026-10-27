# Create a skill, part 1: discovery

You are gathering, not building. Don't write any part of a SKILL.md, pick a folder, or create files until the user confirms the brief at step 6. The building steps live in `author-skill.md` on purpose: when the building steps are in view, discovery gets rushed and the skill comes out generic.

## 0. Nothing attached yet? Ask for it

If the user started with only the job (or nothing at all), don't interview them from scratch. Get the job in one sentence, then ask them to upload what they already have, in one message:

> "Upload whatever you've already got for this job. Any of these helps, and none is required:
> - 1 to 3 of your best real examples (the standard you want it to hit);
> - how you do it, step by step (notes, a checklist, an SOP, even a voice-note transcript);
> - when you use it, and what done looks like;
> - anything you've had to correct Claude on before.
>
> Drag the files in or use the + button. If you don't have some of these, just say so, and I'll ask you instead."

Wait for the upload. Then carry on from step 1 with whatever arrived. Whatever's missing becomes interview questions in step 3. No examples at all goes to "No example yet".

## 1. Read what you have first

Before asking anything, read:

- every file the user attached or pointed at (their golden standard);
- the skills folder (`.claude/skills/` or `.agents/skills/`), to find a skill that already does this job or one the new skill should work with;
- the project's `CLAUDE.md` or `AGENTS.md`, if there is one.

Tell the user in 3 to 5 plain sentences what you found, what's missing, and what you'll reuse.

## 2. Run the worth-it check

Use "Is it worth a skill?" in `SKILL.md`. If it fails, say so and let the user decide.

## 3. Interview them about how they do the job

Open with: "Walk me through how you do this job today, step by step, as if you were training someone to do it without you."

Then work through these, skipping any the golden standard already answers. Ask one or two at a time, not all at once.

1. **The real example.** Point at 1 to 3 real pieces of excellent work. Descriptions don't count. No real example means no build yet (see "No example yet" below).
2. **What makes them good.** Concrete qualities: "the opening names the reader's problem in one line", not "a good hook".
3. **The steps.** For each quality, what did they do to get it? Work backwards from the finished piece.
4. **What it touches.** Files, folders, tools or apps the job needs.
5. **How they'd ask for it.** The real words they'd type. These become the skill's description.
6. **What done looks like.** Checks they could tick off, not a feeling. Ask: "How do you know it's good enough to send?"

Where their answer is vague, ask for an example, and keep asking until you could do the job yourself.

### No example yet

Make one together. Do the job once by hand on one real input, show it, and take their corrections. Every correction becomes a rule in the skill ("IF the opening explains the background first, THEN start with the reader's problem"). When your draft goes generic, stop and ask how they'd put it. Repeat until they say "yes, like that". That piece becomes the example.

## 4. Check it's one job

Say the job in one sentence with one verb. If it needs "and", it's probably two skills, or a skill system. Tell the user, with your recommendation first:

- one skill now (fastest, working today);
- the whole chain as a skill system (go to `build-skill-system.md`);
- two separate skills that work together.

Let them choose. Don't ask if they've already told you.

## 5. Write the brief

```
## BRIEF: <skill-name>

- THE ONE JOB: <one sentence, one verb>
- THE REAL EXAMPLE: <file path, or a short excerpt>
- WHAT MAKES IT GOOD: <the concrete qualities>
- THE STEPS: <in order, in their words>
- WHAT IT TOUCHES: <files, tools, apps>
- HOW THEY ASK FOR IT: <their real phrases>
- WHAT DONE LOOKS LIKE: <the checks>
- WHAT IT NEVER DOES: <anything they ruled out, e.g. "never sends without my yes">
```

Keep it to one screen.

## 6. Stop and confirm

Show the brief and ask: "Does this match how you do it? I'll build it once you say yes." Fold in corrections and show it again until they say yes.

Only after a clear yes, open `workflows/author-skill.md` and build from the brief.

If the user handed you a complete golden standard and answered everything, this can take one turn: show the brief, get the yes, move on. Don't re-interview someone who's already answered.
