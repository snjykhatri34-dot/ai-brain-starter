# Turn a workflow into a reusable skill

When a workflow in `brain/workflows.md` comes up every week, make it a skill so you can run it with one line instead of re-explaining it.

```text
Read the workflow called "<NAME>" in my brain/workflows.md, plus working-style.md and writing-voice.md.

Turn it into a Claude skill: a SKILL.md file with
1. YAML frontmatter: `name` (kebab-case) and a `description` that says exactly when to use it, including the phrases I'd naturally type to trigger it.
2. A short "Goal" section.
3. "Inputs": what to ask me for if it's missing, and what to assume by default.
4. "Steps": numbered, specific, in the order I actually do them.
5. "Output": the exact format, with a short example.
6. "Checks before finishing": the quality bar from the workflow's "Good looks like" and "Watch out for" lines.
7. "Ask first": any step that sends, publishes, spends money, or deletes something.

Keep it under 400 words. Before writing it, ask me up to 3 questions about anything in the workflow that's ambiguous.
```

Save the result as `skills/<name>/SKILL.md` in your Brain repo, then add it to Claude (Settings > Capabilities > Skills on claude.ai, or `~/.claude/skills/` for Claude Code).
