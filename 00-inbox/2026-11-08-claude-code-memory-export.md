---
title: Claude Code memory export
type: note
status: active
sensitivity: personal
updated: 2026-11-08
tags: [inbox, ai, memory-export]
---

# Claude Code memory export

Source: Claude Code persistent memory on the Mac (`~/.claude/projects/*/memory/`), run 2026-11-08. This covers Claude Code only. The claude.ai and ChatGPT exports still need running from the prompt in [[_system/prompts/memory-export|Memory export prompt]].

## Me

- Nothing stored.

## Career

- Nothing stored.

## EASM work

- Built ThreatWatch on 2026-07-28 at `~/Claude/threatwatch`: a local web app for the M&S EASM team tracking emerging threats and zero-days.
- Purpose: cover the window between a threat being published and it becoming a scanner finding, which existing vulnerability management tooling cannot see.
- Stack: Python 3.9 standard library only, SQLite, served on 127.0.0.1:8787.
- Design choices: exploitation evidence and inventory presence weigh more than CVSS in the watch score; triage status and exposure validation are separate fields; the headline metric is internet-facing inventory matches with no validation decision.
- Campaign intelligence is split into curated entries (must carry a source URL) and auto-detected keyword matches labelled as candidates, not findings.
- Installing runtimes or pip packages on work machines may need a change request.

## iLoX Photography

- Nothing stored.

## Ember Weddings

- Nothing stored.

## The Cornish Geek

- Nothing stored.

## Home

- Nothing stored.

## Solar

- Nothing stored.

## Home Assistant

- Nothing stored.

## Finance

- Nothing stored.

## Fitness

- Nothing stored.

## Rental property

- Nothing stored.

## Vehicles

- Nothing stored.

## Travel

- Nothing stored.

## Other

- Mac (as of 2026-07-28) has no Node.js or npm, and only the system Python 3.9.6. Local tools should be Python 3.9 stdlib only, or start with a Node install step agreed first.

## Suggested filing

- ThreatWatch bullets: `20-areas/work-easm/index.md` or a new `30-projects/threatwatch.md`.
- Mac tooling constraint: `10-me/ai-behaviour.md` or a resources note on the dev setup.
