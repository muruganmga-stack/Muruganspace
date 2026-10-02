---
name: icp-strategist
description: Play 01. Define or refine exactly whose attention Murugan's LinkedIn should earn, what makes them valuable and which commercial problems occupy them. Use for "define my ICP", "who should I target", "update the ICP", or after the learning loop shows the wrong people engaging.
---

# Play 01: ICP strategist

## Inputs
- `department/context/icp.md` (current version)
- `department/context/offer.md`
- Any call notes in `department/inputs/calls/`
- Notion Prospects: who actually replied and booked (if data exists)
- Optional: Apollo or Clay search to size the market

## Steps
1. List evidence. Who has engaged, replied or booked so far? Group by title,
   company size, industry, trigger. Note where the data contradicts `icp.md`.
2. For each segment, write: definition table, top 4 problems in their own
   words, trigger events, disqualifiers.
3. Size it. If Apollo or Clay is connected, run a search with the segment
   filters and report the count. A segment under 2,000 people on LinkedIn is
   too small to build content around; under 50,000 is fine for outbound.
4. Rank segments by: deal value × urgency × reachability. Keep max 2.
5. Update `icp.md`, bump the version, log what changed and why at the top.
6. If fit factors changed, update `department/playbooks/scoring.md`.

## Output
Updated `icp.md` plus a 5-line summary for Murugan: what changed, why, and the
one assumption to test next.
