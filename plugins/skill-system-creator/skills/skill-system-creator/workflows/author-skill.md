# Create a skill, part 2: build it from the brief

Don't start here. If there's no brief the user said yes to in this conversation, go back to `workflows/create-skill.md`. (A confirmed step from `build-skill-system.md` counts as a brief.)

Every step below uses the brief. If you need an answer that isn't in it, ask the user and add it to the brief. Don't guess.

## 1. Pick the shape

- **One file** (`SKILL.md` only): the job fits in about 250 lines.
- **SKILL.md plus `workflows/`**: the job has variants (an email vs a newsletter) or long steps.
- **Plus `references/`**: the real example or a long checklist, kept in its own file so SKILL.md stays short.

Tell the user the shape in one line before creating anything.

## 2. Write SKILL.md

Start from `templates/SKILL-template.md`. It must have:

1. **Frontmatter**: `name` (lowercase-with-dashes) and `description`. The description says what the skill does and when to use it, using the user's real phrases from the brief. Claude reads this line to decide when to run the skill, so make it specific. Keep it under 1,024 characters.
2. **The steps**, in the user's order, as instructions: "Open with the reader's problem," not "The skill should open with…".
3. **The real example** as the bar: "Match this." Put a short example inline, or reference a longer one by path in `references/`.
4. **What done looks like**: the user's checks as a short list the skill runs through before showing its result.
5. **The stop**: "Show the user the result and stop. Nothing gets sent, posted or published without their yes."
6. **When not to use it**: the jobs next door that look similar.

Give each rule its reason in a few words ("open with the problem, because readers decide in the first line"). Rules with reasons get followed. Bare ALWAYS/NEVER lists get ignored.

## 3. Check the files

- The frontmatter has `name` and `description`, and the name matches the folder.
- Every file SKILL.md mentions exists, and every file in the folder is mentioned.
- The real example is in it.
- It reads as instructions, not a description of a skill.

## 4. Run it once, now

Follow the SKILL.md you just wrote yourself, on one real input from the user (not the example you were given), and show them the result. This catches the step that can't actually be followed. If something's off, fix the skill and run it again.

## 5. Show them how to test it

Tell the user:

> "Type `/skills` to see it in the list. Then start a new chat, ask for the job in your normal words, and don't name the skill or attach anything. It should pick the skill by itself. If it doesn't show up, start a new session. If it picks the wrong thing, tell me and I'll sharpen the description."

## 6. Tell them how to improve it

> "When something's off, say 'fix the skill' and what was wrong. I'll show you the change before I make it, and it stays in the skill from then on."

## Done means

- The skill folder is in the right place (see "Where skills go" in `SKILL.md`).
- The user has seen it run once on a real input.
- The user knows how to test it in a new chat and how to say "fix the skill".
