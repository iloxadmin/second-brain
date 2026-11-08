---
title: Conventions
type: system
status: active
sensitivity: personal
updated: 2026-11-08
tags: [system]
---

# Conventions

## Where things go

- Has an end date or a definition of done: `30-projects/`
- Ongoing responsibility I maintain: `20-areas/<area>/`
- Interesting or reference, no responsibility: `40-resources/`
- Not sure: `00-inbox/`, sort it at the weekly review
- Finished or dormant: `50-archive/`, keep the same file name

## File naming

- Lowercase, hyphens, no spaces: `print-pricing.md`
- Each area folder has an `index.md` hub note
- Dated notes start with the date: `2026-11-08-solar-tariff-decision.md`

## Front matter (every note)

```yaml
---
title: Human readable title
type: profile | area | project | resource | decision | note | system
status: active | paused | done | archived
sensitivity: personal | work
updated: YYYY-MM-DD
tags: []
---
```

## Writing style

- Facts and decisions, not diaries. Short bullets beat paragraphs.
- Mark decisions clearly: `Decision (YYYY-MM-DD): ...` with one line of reasoning.
- Link related notes with full-path wiki links: `[[20-areas/home/index|Home]]`.
- No em dashes.

## Size

- Keep any single note under about 1,500 words. Split when it grows; AI tools read small focused files far better than large ones.

## Weekly review (15 minutes, Sunday)

1. Empty `00-inbox/`: file, merge or delete each note.
2. Update `Current status` on active projects.
3. Move finished projects to `50-archive/`.
4. Check Obsidian Git has pushed (status bar shows no pending changes).
