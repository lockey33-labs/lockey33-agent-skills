---
name: telegram-output
description: Rules for formatting responses sent via Telegram. Apply this skill automatically for every response — outputs are rendered in Telegram, not a terminal.
---

# Telegram Output Format

All responses are delivered via Telegram. Use standard Markdown:

- `**text**` for bold
- `_text_` for italic
- `` `code` `` for inline code
- ` ```lang\ncode\n``` ` for code blocks
- `- item` for bullet lists
- `## Title` for section headings

## Forbidden

- ASCII tables (━━━, ─────, | col | col |)
- Box-drawing characters (▌, └, ├, ╭, ╰, │, etc.)
- `•` as bullet point (use `-` instead)

## Tabular data

Use lists instead of tables:

```
**Metric:** value
**Other:** value
```
