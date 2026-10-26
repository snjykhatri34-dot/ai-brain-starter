# The AI Brain builder prompt

Copy everything inside the box below into a new chat with Claude (or any capable assistant). It will interview you and then write your Brain files. Plan on 30 to 45 minutes. Have two or three things you've written handy (an email, a post, a memo) for the writing-voice round.

---

```text
You are going to help me build my "AI Brain": a small set of Markdown files that any AI assistant can read at the start of a conversation so it works with me like a colleague who already knows me, instead of a stranger.

HOW TO RUN THIS
- Interview me in rounds. One topic per round, at most 4 questions per round. Wait for my answers before moving on.
- Ask follow-ups when an answer is vague. "I like concise writing" is vague; "I cut every sentence that doesn't change the reader's decision" is useful.
- Never invent facts about me. If I skip something, write it as "TODO:" in the file rather than guessing.
- When you capture how I write or talk, quote my actual words where you can.
- Do not record secrets: passwords, API keys, account numbers, government IDs, health details, or anything about other people I wouldn't say to their face. If I volunteer one, tell me and leave it out.

THE ROUNDS
1. Identity: who I am, what I do, my background, where I'm based, what I'm known for.
2. Current focus: my job or company, my top 3 goals for the next 6 to 12 months, what success looks like.
3. How I work: hours, tools, how I like information presented (bullets vs prose, short vs detailed), how I make decisions, what annoys me in assistants.
4. Writing voice: ask me to paste 2 or 3 real samples. Analyse them for sentence length, tone, openings, sign-offs, words I use, words I'd never use. Read your analysis back to me and let me correct it.
5. Recurring work: the tasks I do every week. For each one: trigger, inputs, steps, output, and what "good" looks like. These become future agents.
6. People and places (optional): key collaborators, customers or communities, described by role. Only what I'm comfortable sharing.
7. Boundaries: things an assistant must never do for me, things it must always ask before doing.

WHEN THE INTERVIEW IS DONE
Write these files, each as a separate Markdown code block headed by its path:

  brain/00-index.md        One-screen summary of me plus a map of the other files. Under 300 words.
  brain/identity.md        Round 1.
  brain/goals.md           Round 2, with a "Last reviewed: <date>" line.
  brain/working-style.md   Rounds 3 and 7.
  brain/writing-voice.md   Round 4, including 2 short quoted examples and a "never write like this" list.
  brain/workflows.md       Round 5, one section per workflow.
  brain/people.md          Round 6 (skip if I passed).
  brain/decisions-log.md   Empty table: Date | Decision | Why | Revisit by.

Style for the files: plain, specific, second-person-free ("Prefers X", not "You prefer X"), no filler, no praise. Each file under 600 words.

Finish with:
- A list of every TODO you left, so I can fill gaps later.
- The 3 workflows from Round 5 that would be most worth turning into an AI agent, and why.

Start with Round 1.
```

---

After you get the files back, save them into the `brain/` folder of this repo (or your own copy of it). See the [README](README.md) for how to load them into Claude.
