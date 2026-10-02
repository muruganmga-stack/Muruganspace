# Muruganspace: the LinkedIn Department

A one-person B2B acquisition department for Murugan's personal brand (B2B
growth, demand gen, AI in marketing). It runs on Claude skills in this repo
and a Notion HQ that holds the data. Goal: booked consulting calls for GTM
strategy and client acquisition work.

## How to use it

Open Claude Code in this repo and say one of:

| Say | Runs |
|---|---|
| "run the week" | `linkedin-department` (full weekly loop) |
| "here are this week's signals" + paste | `signal-analyst` |
| "research Priya at Northwind" | `prospect-researcher` |
| "draft the opener for Priya" | `conversation-designer` |
| "what follow-ups are due" | `follow-up-runner` |
| "fix my profile" + paste profile | `profile-architect` |
| "weekly review" | `learning-loop` |

## Rollout: three waves

Everything is built. You switch the plays on in this order because each wave
feeds the next.

| Wave | Weeks | Plays on | Exit criteria |
|---|---|---|---|
| 1. Foundation | W40 to W41 | 01 ICP, 02 Profile, 03 Ideas, 04 Posts | Profile rewritten, 6 posts live, proof bank has 3 rows |
| 2. Signal | W42 to W44 | + 05 Signals, 06 Research, 07 Conversations | 20+ prospects scored, 10 conversations opened |
| 3. Compounding | W45 on | + 08 Follow-ups, 09 Learning loop | First weekly review with 3 changes, 2+ calls booked |

Why this order: signals need content, content needs a profile worth
landing on, and the learning loop needs at least 3 weeks of data to say
anything true.

## Notion HQ (private, in Murugan's workspace)

| Item | Link | Data source ID |
|---|---|---|
| HQ page | https://app.notion.com/p/3edd727b3c8f8192a8b8c572ccd18729 | n/a |
| Content | https://app.notion.com/p/c605002571314a0fa2d31b837fd8737c | `37bcdc88-b23a-4a9d-8616-b7ca754ee605` |
| Prospects | https://app.notion.com/p/9735b480c1514ce4a9c32580c86af5e8 | `1bb80435-aab3-47f2-b49e-b23d206ad0de` |
| Touches | https://app.notion.com/p/0f04a166fcbe43519685b27680ccf12b | `b55b1141-4aa8-41b6-bf10-8b9492d9b20f` |

Prospects calculates `Total` and `Tier` automatically from `Fit` and `Intent`.
Touches links to Prospects so follow-ups can read the full history.

## Connected tools the plays use

- **Notion**: state for content, prospects and touches
- **Apollo / Clay**: company size, funding, hiring, verified contacts (plays
  01, 05, 06). Credit cost is reported before any spend.
- **Web search**: market shifts for idea mining, company news for briefs
- **Calendly**: booking link for the Pipeline Teardown (add to `offer.md`)

## What it will never do

Send, connect, like or scrape on LinkedIn. Claude drafts. Murugan sends.

## Repo map

```
CLAUDE.md                      department rules, targets, play index
.claude/skills/                orchestrator + 9 play skills
department/context/            offer, ICP, voice, proof bank (load every time)
department/playbooks/          scoring rubric, message rules
department/inputs/             signals, call notes, current profile (you drop files here)
department/outputs/<week>/     ideas, posts, briefs, reviews
```

## Your to-do list to finish wave 1

1. `offer.md`: pricing band and the Calendly link for the Pipeline Teardown
2. `proof-bank.md`: 3 real results with numbers (this unlocks better posts)
3. `inputs/profile/current.md`: paste your current headline and About
4. React to the ICP v1 and the 10 ideas: keep, kill or change
