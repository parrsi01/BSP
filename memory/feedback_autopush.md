---
name: Auto-push after every prompt
description: User requires git commit and push at the end of every response in BSP project
type: feedback
---

Always run `git add . && git commit && git push` at the end of every response in the BSP project.

**Why:** User's team of 4 pulls from the repo — changes need to be live immediately after each session turn.

**How to apply:** No exceptions. Every prompt = commit + push, even small edits. Commit message should summarize what changed that turn.
