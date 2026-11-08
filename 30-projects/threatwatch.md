---
title: ThreatWatch
type: project
status: active
sensitivity: work
updated: 2026-11-08
tags: [project, code, easm]
---

# ThreatWatch

## Summary

A local web app for the M&S EASM team that tracks emerging threats and zero-days. It covers the gap between a threat being published and it showing up as a scanner finding, which existing vulnerability management tooling cannot see.

## Where the code lives

- Local: `~/Claude/threatwatch`
- Technical docs stay in the repo. This note holds goals, decisions and status only.
- Stack: Python 3.9 standard library only, SQLite, served locally on port 8787.

## Goal and definition of done

- Scope requested (2026-07-28): newly published critical CVEs, new KEV entries, vendor emergency advisories, zero-days, new exploit or PoC releases, ransomware-associated vulnerabilities, campaigns targeting retail or similar organisations, technologies per threat, matches against the technology inventory, and exposure validation status.
- Definition of done: not yet set.

## Current status

- Built 2026-07-28. Pulls from 17 live feeds; first cold start loaded 5,864 items in 96 seconds.
- Dashboard restyled from a Group-IB style reference board. Columns form a proximity ladder: Internet-facing, In our estate, Sector targeting, Under watch.
- The bundled inventory is invented sample data, not the M&S estate. Headline figures from this build are not real exposure numbers.
- Local git repo set up 2026-07-29. Not pushed: the remote is still a placeholder URL (checked 2026-11-08).

## Decisions

- Decision (2026-07-28): exploitation evidence and inventory presence weigh more than CVSS in the watch score. Exploitability and exposure predict real risk better than severity alone.
- Decision (2026-07-28): triage status and exposure validation are separate fields. Deciding a threat matters is a different question from confirming the estate is exposed.
- Decision (2026-07-28): the headline metric is internet-facing inventory matches with no validation decision. It shows the work that is outstanding, not the volume of threats.
- Decision (2026-07-28): campaign intelligence is split into curated entries, which must carry a source URL, and auto-detected keyword matches labelled as candidates, not findings. Keeps unverified matches from being read as fact.
- Decision (2026-07-29): real inventory and campaign files are gitignored; only `.example.json` versions are tracked. Keeps estate data out of the repo.

## Next actions

- Decide whether to push to a private GitHub repo.
- Installing runtimes or pip packages on work machines may need a change request; check before deploying beyond this Mac.

## Links

- [[20-areas/work-easm/index|EASM function (M&S)]]
