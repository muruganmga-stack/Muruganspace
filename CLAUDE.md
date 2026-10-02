# Murugan's LinkedIn Department

This repo is a one-person LinkedIn acquisition department run by Claude.
Goal: turn one personal LinkedIn account into a steady source of booked
consulting calls for B2B growth, demand generation and GTM strategy work.

## North star

**Qualified consulting calls booked per month.** Everything else is a leading
indicator. Targets for the first 90 days:

| Metric | Month 1 | Month 2 | Month 3 |
|---|---|---|---|
| Posts published | 12 | 14 | 16 |
| ICP comments on posts | 20 | 45 | 80 |
| Warm prospects scored 55+ | 15 | 35 | 60 |
| Conversations opened | 10 | 25 | 40 |
| Calls booked | 2 | 5 | 8 |

## Always load before any play

1. `department/context/offer.md`: what we sell and the call we book
2. `department/context/icp.md`: who we want attention from
3. `department/context/voice.md`: how every word is written
4. `department/context/proof-bank.md`: the only claims we are allowed to make

## The plays (skills in `.claude/skills/`)

| Wave | Play | Skill |
|---|---|---|
| 1 | 01 ICP strategist | `icp-strategist` |
| 1 | 02 Profile architect | `profile-architect` |
| 1 | 03 Idea miner | `idea-miner` |
| 1 | 04 Post engineer | `post-engineer` |
| 2 | 05 Signal analyst | `signal-analyst` |
| 2 | 06 Prospect researcher | `prospect-researcher` |
| 2 | 07 Conversation designer | `conversation-designer` |
| 3 | 08 Follow-up runner | `follow-up-runner` |
| 3 | 09 Learning loop | `learning-loop` |

`linkedin-department` is the orchestrator. It runs the weekly loop:
discover → shape → publish → observe → approach → nurture → learn.

## Hard rules

- **Never automate sending on LinkedIn.** Claude drafts, Murugan sends. No
  scraping tools, no auto-DMs, no auto-connects. The account is the asset.
- **Never invent proof.** Numbers, client names and results come only from
  `proof-bank.md`. If the proof is missing, write around it or flag it.
- **Never pitch before a reply.** First touches earn a reply, not a meeting.
- **Every prospect and post lives in the Notion HQ** (see README). The repo
  holds the system; Notion holds the state.
- Weekly outputs go in `department/outputs/<YYYY>-W<week>/`.
