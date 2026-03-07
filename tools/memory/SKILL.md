---
name: memory
description: Manage long-term memory across sessions. Apply at session end (when the user says goodbye or /reset).
---

# Memory Management

## Context file location

- With a repo: `.ai-context/context.md` at the repo root
- Without a repo: `~/.agent-memory/context.md`

If the file doesn't exist yet, create it.

## What to write

At session end, write a concise summary (max 150 lines):

- Current state of the work
- Key decisions made
- Last actions taken
- Next steps

Remove anything obsolete or redundant. The file must remain under 150 lines.

## Compaction

If the file exceeds 500 lines, rewrite it entirely before doing anything else — keep only the essential.
