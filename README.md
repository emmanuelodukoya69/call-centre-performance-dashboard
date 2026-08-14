# Call Centre Data Analysis (PwC Dashboard)
<img width="900" height="450" alt="pwc 1" src="https://github.com/user-attachments/assets/65af69be-1244-4196-a36a-8e612e68c98e" />

Power BI dashboard analyzing 5,000 call records from a call centre's Q1 2021 operations (Jan–Mar 2021) — covering call volume, resolution, satisfaction, and agent performance.

**Dashboard includes 4 pages:** an intro page, a Main Overview dashboard (KPI cards, agent performance table, satisfaction levels, call volume by hour/day), an Operational Dashboard (monthly volume, answer rate by agent, topic distribution), and an Agent Dashboard (talk duration, CSAT, and resolution by topic per agent) — all with interactive filters for agent, topic, month, and weekday.

---

## Overview
<img width="673" height="381" alt="pwc 2" src="https://github.com/user-attachments/assets/98c29763-b61c-4db4-8f43-35f540280352" />

| Metric | Value |
|---|---|
| Total call volume | 5,000 |
| CSAT | 68.07% |
| Calls answered | 81.08% |
| Calls abandoned | 18.92% |
| Avg. speed of call answer | 67.52 sec |
| Avg. call handling time (talk duration) | 224.92 sec |

---

## Key Findings

### 1. Call Outcomes
<img width="673" height="380" alt="pwc 3" src="https://github.com/user-attachments/assets/1d8cd915-7215-49ca-b9a4-0ccdac3ee9d2" />

| Outcome | Calls |
|---|---|
| Answered | 4,054 |
| Abandoned | 946 |

Of the 4,054 answered calls, 3,646 were marked resolved — a 89.94% true resolution rate among calls that connected. That means roughly 1 in 10 answered calls still went unresolved.

| Satisfaction Level | Calls |
|---|---|
| Normal | 1,218 |
| Satisfied | 1,180 |
| Not Served | 946 |
| Very Satisfied | 843 |
| Very Dissatisfied | 417 |
| Dissatisfied | 396 |

"Not Served" (946) lines up exactly with the number of abandoned calls — every unanswered call is logged as a satisfaction gap.

### 2. Agent Performance
<img width="672" height="380" alt="pwc 4" src="https://github.com/user-attachments/assets/40eac2ba-4b1a-430d-a412-fcb640b09685" />


| Agent | Total Calls | Answer Rate | Avg. Speed (sec) | True Resolution Rate | CSAT |
|---|---|---|---|---|---|
| Martha | 638 | 80.56% | 69 | 89.69% | 69.42% |
| Dan | 633 | 82.62% | 67 | 90.06% | 68.95% |
| Diane | 633 | 79.15% | 66 | 90.22% | 68.10% |
| Greg | 624 | 80.45% | 68 | 90.64% | 68.09% |
| Stewart | 582 | 81.96% | 66 | 88.89% | 68.01% |
| Jim | 666 | 80.48% | 66 | 90.49% | 67.87% |
| Becky | 631 | 81.93% | 65 | 89.36% | 67.43% |
| Joe | 593 | 81.62% | 71 | 90.08% | 66.61% |

Performance is tightly clustered — no single agent stands out as a major outlier, though Martha leads on CSAT (69.42%) while Greg leads on true resolution rate (90.64%).

### 3. Call Volume Patterns

| Day | Calls |
|---|---|
| Monday | 770 |
| Saturday | 768 |
| Sunday | 716 |
| Thursday | 712 |
| Friday | 680 |
| Wednesday | 679 |
| Tuesday | 675 |

Monday and Saturday are the busiest days, roughly 90 calls higher than the quietest day (Tuesday).

| Month | Calls |
|---|---|
| January 2021 | 1,772 |
| February 2021 | 1,616 |
| March 2021 | 1,612 |
| **Total** | **5,000** |

Call volume by hour peaks between 11:00–17:00, dropping off sharply after 17:00 as the centre's operating hours end.

### 4. Call Topics

| Topic | Calls (answered) | Resolved | Unresolved |
|---|---|---|---|
| Streaming | 847 | 749 | 98 |
| Technical Support | 805 | 736 | 69 |
| Payment Related | 818 | 729 | 89 |
| Contract Related | 789 | 709 | 80 |
| Admin Support | 795 | 723 | 72 |

Call volume is spread almost evenly across the five topics, and resolution rates stay close together (around 90–91% for each) — no single topic category is a clear resolution bottleneck.

---

## Key Insights

- **Nearly 1 in 5 calls are abandoned (946 of 5,000)**, and this exactly matches the "Not Served" satisfaction bucket — unanswered calls are the single biggest driver of dissatisfaction in the data.
- **Even among answered calls, about 1 in 10 still go unresolved** (10.06%), meaning resolution — not just pickup — deserves its own tracking metric.
- **Agent performance is consistent rather than polarized** — the spread between the best and weakest agent on CSAT is under 3 percentage points, suggesting training and process standards are working evenly across the team.
- **Monday and Saturday carry the heaviest call load**, which is useful for staffing and shift planning.
- **No single call topic is disproportionately harder to resolve** — the resolution rate stays in a tight 89–91% band across all five categories.

---

## Recommendations

1. Prioritize reducing the 18.92% abandonment rate first — it's the largest single driver of "Not Served" dissatisfaction and likely the highest-leverage fix available.
2. Track true resolution rate (not just answer rate) as its own KPI, since roughly 1 in 10 answered calls still go unresolved.
3. Align staffing levels with the Monday/Saturday call volume peaks to reduce wait times and abandonment on the busiest days.
4. Since agent performance is already tightly clustered, focus coaching on process consistency (e.g., speed of answer) rather than singling out any one agent.
5. Continue monitoring topic-level resolution rates for early warning if any single topic (e.g., Streaming, currently the largest unresolved count at 98) starts to drift from the ~90% band.
