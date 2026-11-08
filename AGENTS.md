# Instructions for AI assistants

This repository is Adrian's second brain. It is shared by Claude (claude.ai, Claude Code) and ChatGPT (chat, Codex). Treat it as the authoritative record of his context. If something here conflicts with your own memory, this repository wins.

## Always read first

1. `10-me/about-me.md` (identity, communication preferences, recommendation framework)
2. `10-me/ai-behaviour.md` (what good and bad help looks like)

## Read when the topic comes up

| Topic | File |
|---|---|
| Values, life goals, what matters | `10-me/motivation.md` |
| Purchases, product recommendations | `10-me/brand-preferences.md` and Purchasing in `10-me/ai-behaviour.md` |
| Career, leadership, progression | `20-areas/career/index.md` |
| M&S, EASM, vulnerability management, security leadership | `20-areas/work-easm/index.md` |
| Fine art landscape photography, prints | `20-areas/iloxphotography/index.md` |
| Wedding photography | `20-areas/ember-weddings/index.md` |
| thecornishgeek.co.uk, small business security content | `20-areas/thecornishgeek/index.md` |
| House, renovation, smart home, solar | `20-areas/home/` |
| Money, debt, saving, investing | `20-areas/finance/index.md` |
| Training, nutrition, body composition | `20-areas/fitness/index.md` |
| Landlord, tenant, letting | `20-areas/rental-property/index.md` |
| Car | `20-areas/vehicles/index.md` |
| A named project | `30-projects/<name>.md` |

If no file matches, check `README.md` and `40-resources/`.

## How to respond

- Executive summary first, recommendation second, detail third.
- Give the objectively best option, then the option you would choose for Adrian, then the trade-offs.
- British English. No em dashes. No decorative icons. No buzzwords.
- Challenge assumptions when there is a better approach.

## Updating the second brain

Adrian approves every change. Follow `_system/conventions.md`.

- If you can write files (Claude Code, Codex): edit the relevant note, update its `updated:` date, and commit with a message starting `brain:`. Never delete notes; move them to `50-archive/`.
- If you cannot write files (chat on web or mobile): when you learn something durable, end your reply with a block titled `Proposed second brain update` containing the target file path and the exact Markdown to add. Adrian will paste it in.
- Only record facts Adrian has stated or confirmed. Do not store your own suggestions as his decisions.

## Never store

- Passwords, API keys, tokens, recovery codes
- Bank, card or account numbers, balances, National Insurance or passport numbers
- M&S internal data: findings, hostnames, IPs, asset lists, tool exports, incident details, colleague names or performance notes
- Tenant or client personal data
