# Fit × intent scoring

Every warm person gets two scores out of 50. Total = fit + intent (0 to 100).

## Fit (0 to 50). Static, scored once from profile + company

| Factor | Points |
|---|---|
| Title: Founder/CEO/CRO = 15, Head of Growth/Marketing/VP = 12, Manager-level = 6, other = 0 | 0 to 15 |
| Company size: 15 to 150 = 10, 151 to 300 = 7, 5 to 14 = 4, other = 0 | 0 to 10 |
| Industry: B2B SaaS = 10, tech-enabled B2B services = 8, other B2B = 4, B2C = 0 | 0 to 10 |
| GTM gap visible (founder-led sales, hiring first SDR or marketer, no content engine) | 0 to 10 |
| Geo in target list | 0 or 5 |

Any disqualifier from `icp.md` sets fit to 0.

## Intent (0 to 50). Dynamic, recalculated weekly

| Signal | Points |
|---|---|
| Profile view (named) | 5 |
| Reacted to a post | 3 |
| Commented on a post | 12 |
| Commented with a question or their own situation | 18 |
| 3+ engagements in 14 days | +10 bonus |
| Followed you / sent connection request | 6 |
| Connection request with a note | 15 |
| Commented a lead magnet keyword | 12 |
| Inbound DM | 25 |
| Trigger event (funding, new sales leader, hiring SDR/marketer) | 10 each, max 20 |
| Posted publicly about a pipeline or growth problem | 10 |

**Decay:** signals older than 14 days count half. Older than 30 days count zero.
Cap intent at 50.

## Tiers and actions

| Total | Tier | Action | SLA |
|---|---|---|---|
| 75 to 100 | Hot | Research brief + first touch (play 06, 07) | 24 hours |
| 55 to 74 | Warm | Engage on their content twice, then first touch | 5 days |
| 35 to 54 | Watch | Keep in tracker, re-score weekly | n/a |
| < 35 or fit < 25 | Ignore | Don't approach, even with high intent | n/a |

Fit under 25 is never approached. A high-intent bad fit is a fan, not a lead.

## Worked example

Priya S., Founder, 60-person B2B SaaS, Bengaluru, hiring first SDR.
Fit: 15 + 10 + 10 + 10 + 5 = **50**.
Intent this week: comment with a question (18) + profile view (5) + hiring
trigger (10) = **33**. Total **83 → Hot**. Brief and first touch within 24h.
