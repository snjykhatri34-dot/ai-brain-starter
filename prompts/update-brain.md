# Update your Brain after a chat

Paste this at the end of any conversation where you shared something new about yourself, your work, or your preferences.

```text
Look back over this conversation and list anything you learned about me that belongs in my Brain and isn't already there.

Rules:
- Only include things I stated or clearly confirmed. No inferences about my personality.
- Nothing secret: no passwords, keys, account numbers, ID numbers, or health details.
- If something contradicts what the Brain already says, show both versions.

Format it as a pending change set, grouped by file:

### brain/<file>.md
1. ADD | CHANGE | REMOVE: <exact text>
   Why: <one line, quoting what I said if possible>

Then stop and wait. I'll reply with the numbers I approve (e.g. "approve 1, 3; edit 2 to say ..."). Only after that, output the full updated text of each changed file with today's date on its "Last reviewed" line.
```

If you use Claude Code, run this inside your Brain repo and let it apply the approved changes and commit them.
