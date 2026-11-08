---
title: Claude Code memory export
type: note
status: active
sensitivity: work
updated: 2026-11-08
tags: [inbox, ai, memory-export]
---

# Claude Code memory export

Source: Claude Code persistent memory and past Claude Code session logs on the Mac, run 2026-11-08. This covers Claude Code only. The claude.ai and ChatGPT exports still need running from the prompt in [[_system/prompts/memory-export|Memory export prompt]].

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
- Requested scope (2026-07-28): newly published critical CVEs, new KEV entries, vendor emergency advisories, zero-days, new exploit or PoC releases, ransomware-associated vulnerabilities, campaigns targeting retail or similar organisations, technologies per threat, matches against the technology inventory, and exposure validation status.
- Dashboard layout restyled from a reference screenshot Adrian supplied (Group-IB style board). Columns became a proximity ladder: Internet-facing, In our estate, Sector targeting, Under watch.
- Pulls from 17 live feeds; first cold start loaded 5,864 items in 96 seconds.
- The bundled inventory (`data/inventory.json`) is invented sample data, not the M&S estate. Versions, instance counts, owners and business units are all made up, so any headline figures from that build are not real exposure numbers. Adrian queried this on 2026-07-28.
- Real inventory and campaign files are gitignored; only `.example.json` versions are tracked. Local git repo set up 2026-07-29; pushing to a private GitHub repo was recommended. Not confirmed whether it was pushed.

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
