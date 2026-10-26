# AI Brain Starter

A template and a set of prompts for building your own **AI Brain**: a handful of Markdown files that tell an AI assistant who you are, what you're working on, how you write and how you like to work.

Load it at the start of a chat and the assistant stops asking the same questions every time. Keep it in Git and it gets better every week instead of being lost in old chat threads.

## What's in here

```
PROMPT.md                 The interview prompt that builds your Brain from scratch
brain/                    Empty templates for each Brain file (fill these in)
  00-index.md             One-screen summary + map of the other files
  identity.md
  goals.md
  working-style.md
  writing-voice.md
  workflows.md
  people.md
  decisions-log.md
  projects/_template.md   Copy this once per active project
prompts/
  start-session.md        Make an assistant load the Brain before it answers
  update-brain.md         End-of-chat: capture what's new, with your approval
  build-agent.md          Turn a workflow into a reusable Claude skill
  review-brain.md         Monthly clean-up of stale facts
CLAUDE.md                 Rules for Claude Code when it works inside this repo
```

## Quick start

1. **Use this template.** Click "Use this template" on GitHub (or fork it). Make your copy **private**: it will hold personal context.
2. **Run the interview.** Open a new chat with Claude, paste the prompt from [PROMPT.md](PROMPT.md), and answer the questions.
3. **Save the output.** Replace the templates in `brain/` with the files Claude gives you. Commit.
4. **Load it.** Pick one of the options below.

## Loading your Brain

| Where you work | How |
|---|---|
| **Claude.ai Projects** | Create a Project, upload the files in `brain/` as project knowledge, and paste [prompts/start-session.md](prompts/start-session.md) into the project instructions. |
| **Claude Code** | Clone your Brain repo and start Claude Code inside it, or point to it from another project's `CLAUDE.md` (for example, `Read ~/my-ai-brain/brain/00-index.md before starting.`). |
| **Any other chat** | Paste the contents of `brain/00-index.md` at the start, and the other files when they're relevant. |

## Keeping it alive

A Brain that isn't updated goes stale in about a month. Two habits keep it fresh:

- **After a useful chat**, paste [prompts/update-brain.md](prompts/update-brain.md). The assistant lists what it learned about you as a pending change set; you approve, edit or reject each item before anything gets written.
- **Once a month**, run [prompts/review-brain.md](prompts/review-brain.md) to prune what's no longer true.

When a workflow in `workflows.md` comes up every week, use [prompts/build-agent.md](prompts/build-agent.md) to turn it into a skill so you can trigger it with one line.

## Privacy

- Keep your filled-in Brain in a **private** repo. This public repo should stay a template.
- Never put passwords, API keys, account numbers, or ID numbers in it. The prompts tell the assistant to refuse to record them, but double-check before committing.
- Describe other people by role, and only with what you'd be fine with them reading.

## License

MIT. See [LICENSE](LICENSE).
