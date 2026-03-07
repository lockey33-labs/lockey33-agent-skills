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

Never use markdown tables (`| col |`). Use this exact format instead:

**2 columns (key-value):**
```
**Key:** value
**Other:** value
```

**3+ columns:**
Header line with all cells bold, then one bullet per row, first cell bold, cells separated by ` — `:
```
**Col1** | **Col2** | **Col3**

- **Row1Col1** — Row1Col2 — Row1Col3
- **Row2Col1** — Row2Col2 — Row2Col3
```

Always put a blank line between the header and the rows.
