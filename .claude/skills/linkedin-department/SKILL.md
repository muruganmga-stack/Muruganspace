---
name: linkedin-department
description: Orchestrator for Murugan's LinkedIn acquisition department. Use when Murugan says "run the week", "weekly loop", "what should I do on LinkedIn this week", "/dept", or asks for a status of the department. Runs discover → shape → publish → observe → approach → nurture → learn by calling the nine play skills in order.
---

# LinkedIn department: weekly operating loop

Load `CLAUDE.md` and all four files in `department/context/` first.
Create `department/outputs/<YYYY>-W<week>/` for this week's outputs.

## Monday (45 min of Murugan's time)

1. **Learn** (`learning-loop`): review last week's numbers from the Notion
   Content and Prospects databases. Write `review.md`. Carry its 3 changes
   into every step below.
2. **Discover** (`idea-miner`): produce `ideas.md` with 15 ideas from
   `department/inputs/calls/`, objections in `offer.md`, and market news.
3. **Shape** (`post-engineer`): turn the best 4 ideas into drafts in
   `posts.md`. Mix: 2 familiarity, 1 curiosity, 1 conversation opener.
   Add them to the Notion Content database with status `Drafted`.

## Daily (15 min)

4. **Publish**: Murugan posts Tue / Wed / Thu at 8:30 local time. Spend 10 min
   before and after commenting on 5 ICP accounts' posts.
5. **Observe** (`signal-analyst`): Murugan pastes or drops a CSV of
   reactions, comments, viewers and new connections into
   `department/inputs/signals/`. Score everyone, update Notion Prospects.
6. **Approach** (`prospect-researcher` → `conversation-designer`): for every
   Hot prospect, write a brief and a first touch. Murugan sends manually.

## Friday (20 min)

7. **Nurture** (`follow-up-runner`): pull every prospect with a touch due in
   the next 3 days, draft the next touch, classify any replies.
8. Write `week-summary.md`: posts shipped, ICP comments, prospects by tier,
   conversations opened, calls booked, one thing to change.

## Status mode

If asked for status, query Notion and answer with this table only:
posts this week, ICP comments, Hot / Warm / Watch counts, touches due,
replies waiting, calls booked this month vs target in `CLAUDE.md`.

## Rules

Never send anything on LinkedIn. Never invent proof. No em dashes.
