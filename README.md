# Insurance Portfolio Analytics

Power BI dashboard analyzing 1,338 policyholder records — connecting demographics (age, sex, BMI, children), smoking status, and region with insurance charges to identify the biggest drivers of cost.

**Dashboard includes:** KPI summary cards (policyholders, total charges, peak claim, average charge, smoker/non-smoker/high-risk counts), an average-charge-by-smoker-status chart, an average-charge-by-age-group chart, a policyholders-by-region donut chart, an average-charge-by-BMI-category chart, an average-charge-by-region-and-smoker-status chart, an average-charge-by-children line chart, and interactive filters for sex and region.

---

## Overview

| Metric | Value |
|---|---|
| Total policyholders | 1,338 |
| Total charges | $17,755,825 |
| Peak claim | $63,770 |
| Average charge | $13,270 |
| Smoker count | 274 |
| Non-smoker count | 1,064 |
| High-risk count (smoker + obese) | ~144 |

---

## Key Findings

### 1. Policyholder Snapshot

| Sex | Policyholders |
|---|---|
| Male | 676 |
| Female | 662 |

| Region | Policyholders |
|---|---|
| Southeast | 364 |
| Southwest | 325 |
| Northwest | 325 |
| Northeast | 324 |

Policyholders are almost evenly split across sex and region.

### 2. Smoking Status Is the Biggest Cost Driver

| Smoking Status | Policyholders | Avg. Charge |
|---|---|---|
| Non-smoker | 1,064 | $8,434 |
| Smoker | 274 | $32,050 |

**Smokers are charged nearly 4x more than non-smokers on average** — $32,050 vs. $8,434 — despite making up only 274 of 1,338 policyholders (about 1 in 5).

### 3. Charges by Region and Smoker Status

| Region | Non-smoker Avg. Charge | Smoker Avg. Charge |
|---|---|---|
| Southeast | $8,032 | $34,845 |
| Southwest | $8,019 | $32,269 |
| Northwest | $8,556 | $30,192 |
| Northeast | $9,166 | $29,674 |

The smoker/non-smoker cost gap holds in every region, and Southeast has the highest average charge for smokers ($34,845).

### 4. Charges by Age, BMI, and Children

| Age Group | Policyholders | Avg. Charge |
|---|---|---|
| 18–25 | 306 | $9,087 |
| 26–35 | 268 | $10,495 |
| 36–45 | 264 | $13,493 |
| 46–55 | 284 | $15,987 |
| 56–64 | 216 | $18,796 |

Average charge rises steadily with age — the 56–64 group pays roughly double the 18–25 group.

| BMI Category | Policyholders | Avg. Charge |
|---|---|---|
| Obese | 707 | $15,552 |
| Overweight | 386 | $10,988 |
| Normal | 225 | $10,409 |
| Underweight | 20 | $8,852 |

707 of 1,338 policyholders (about 1 in 2) fall into the Obese category, and this group carries the highest average charge.

| Children | Policyholders | Avg. Charge |
|---|---|---|
| 0 | 574 | $12,366 |
| 1 | 324 | $12,731 |
| 2 | 240 | $15,074 |
| 3 | 157 | $15,355 |
| 4 | 25 | $13,851 |
| 5 | 18 | $8,786 |

Average charge rises from 0 to 3 children, then drops off for policyholders with 4 or 5 children — though these are the smallest groups (25 and 18 people).

---

## Key Insights

- **Smoking status is the single strongest cost driver in the portfolio** — the ~4x charge gap between smokers and non-smokers holds consistently across every region.
- **About 144 policyholders are both smokers and obese**, a compounding high-risk group that likely drives a disproportionate share of the $17.8M in total charges.
- **Cost rises predictably with age**, making age-based premium tiers a reasonable and data-supported pricing lever.
- **Obesity alone (independent of smoking) adds roughly $5,000–$7,000** to average charges compared to Normal or Overweight BMI categories.
- **The children-vs-charge relationship is less clear-cut**, especially for 4–5 children — the smaller sample sizes there mean this pattern should be viewed with caution rather than treated as a firm trend.

---

## Recommendations

1. Use smoking status as the primary risk-adjustment factor in pricing — it's the clearest, most consistent driver of cost across every region.
2. Target the ~144 smoker-and-obese policyholders for wellness or smoking-cessation program outreach, given their compounded risk profile.
3. Apply age-based premium tiers, since average charges rise steadily and predictably from the 18–25 to 56–64 age groups.
4. Incorporate BMI into risk scoring alongside smoking status, since Obese policyholders carry meaningfully higher charges even as non-smokers.
5. Collect more data on higher-children-count policyholders (4–5 children) before drawing firm conclusions — current sample sizes there are too small to generalize confidently.

---

*Source: Insurance Portfolio Analytics dashboard (Power BI), 1,338-record policyholder dataset.*
