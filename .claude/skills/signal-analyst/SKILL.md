---
name: signal-analyst
description: Play 05. Read account activity (reactions, comments, profile views, follows, connection requests, DMs) for intent clues, then separate casual attention from genuine commercial interest using fit × intent scoring. Use when Murugan pastes engagement data, drops a CSV in department/inputs/signals, or says "score my signals".
---

# Play 05: Signal analyst

Rules live in `department/playbooks/scoring.md`. Follow them exactly.

## Inputs (any of these)
- Pasted list: name, headline, action, post, date
- CSV in `department/inputs/signals/` (LinkedIn exports or copy-paste)
- Screenshots of notifications or "Who viewed your profile"
- Optional enrichment via Apollo `people_match` / Clay for company size,
  industry, funding and hiring. Report credit cost before spending.

## Steps
1. Normalize to one row per person: name, title, company, signals with dates.
2. Match to existing Notion Prospects (by name + company). Append new signals,
   don't duplicate people.
3. Score fit (enrich only if fit can't be judged from the headline).
4. Score intent with decay.
5. Assign tier. Flag anything that changed tier since last week.
6. Upsert to Notion Prospects: Fit, Intent, Tier, Last signal, Signal log.

## Output
A table sorted by total score: name, company, fit, intent, total, tier,
top signal, recommended action. Then a 3-line read: what's working, which
post pulled the best-fit people, who to approach today.
