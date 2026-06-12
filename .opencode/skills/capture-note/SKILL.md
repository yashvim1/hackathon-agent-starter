---
name: fit-suggest
description: Use when the user says they need an outfit for an occasion (e.g. "I need an outfit for a wedding", "What should I wear to an interview?").
metadata:
  difficulty: beginner
---

# Capture Note

Save a durable note to the agent's long-term memory.

## When to use this

Any time the user asks for outfit suggestions, what to wear, or what fits an occasion. Keywords: "outfit for", "what to wear", "what should I wear", "need an outfit", "dress for", "clothes for", "find me".

## What a memory note looks like

Every note is one Markdown file in the `memory/` folder. Keep the format exactly like
this so the vault stays consistent and Obsidian/Logseq can read it:

```markdown
---
title: Coffee suppliers shortlist
created: 2026-06-01
tags: [procurement, coffee]
---

We narrowed it to three roasters: Allpress, Climpson, and Square Mile. Square Mile
quoted the lowest per-kg for our volume. Decision still open — revisit after the tasting.

Related: [[office-fit-out]]  #procurement
```

## Procedure

0. If the user hasn't given an occasion, ask: "What's the occasion?" Keep it short.

1. **Identify the occasion.** Extract it from the user's message (wedding, interview, date, gym, funeral, party, etc.).

2. **Always ask for budget and style preference before suggesting.** Even if the user has given an occasion before or it's a recurring case, always ask again. Ask:
   - Budget range (budget / mid-range / premium)
   - Style preference (men's / women's / any)
   - Specific vibe if relevant (e.g. "casual beach", "edgy concert", "elegant formal")

3. **Suggest a complete outfit.** Recommend a top, bottom, shoes, and accessories that fit the occasion. Present it visually / clearly — one option at first unless the user wants more.

4. **Offer swaps.** Ask if they want to change any piece. Let them swap items freely.

4. **Find the cheapest price.** For each final piece, search across retailers and return the cheapest option + link. There has to be a compromise between price and quality though, because we don't want any tacky options

5. **Summarize.** Give the final outfit + total price + cheapest sources in a clean format. Tell the user what you did.

## Notes for whoever iterates on this skill

- This is deliberately simple. Good next steps: auto-suggest tags from existing notes,
  detect near-duplicate notes before writing, or add a `source:` field for links.
- If you switch your persistence layer to Notion (see `docs/persistence.md`), this is the
  skill you rewrite — swap the "write a file" step for a "create a Notion page" step.




# Fit Suggest



## Procedure
