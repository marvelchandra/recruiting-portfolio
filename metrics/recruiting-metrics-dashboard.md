# 📊 Recruiting Metrics Dashboard

> A practical KPI framework for TA teams and founding recruiters — the exact metrics used to report to CEOs at Arrcus, Factory VC, and CommScope. Includes templates, formulas, and a Google Sheets dashboard.

[![Portfolio](https://img.shields.io/badge/Portfolio-marvelchandra-008080?style=flat-square)](https://marvelchandra.github.io/recruiting-portfolio)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-chandrabuduri-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/chandrabuduri)

---

## Why Metrics Matter for Recruiters

Most TA teams track vanity metrics — reqs opened, reqs closed. The CEOs and VPs I've worked with want to know:

- **Is the pipeline healthy?** (leading indicators)
- **Are we hiring fast enough?** (velocity)
- **Are our hires working out?** (quality)
- **Where are we losing candidates?** (conversion)

This framework answers all four.

---

## The Core Metrics

### 1. Pipeline Health (Weekly)

| Metric | Formula | Target |
|---|---|---|
| Pipeline Coverage | Candidates in pipeline / Open reqs | 5:1 minimum |
| Stage Conversion | Candidates advancing / Candidates reviewed | Track by stage |
| Source Mix | % from each source channel | No single source >60% |
| Active Reqs | Reqs with active pipeline | >80% of open reqs |

### 2. Velocity (Speed)

| Metric | Formula | Benchmark |
|---|---|---|
| Time to Fill (TTF) | Offer accepted date − Req open date | <45 days (IC), <60 days (Mgr+) |
| Time to Screen | First screen date − Application date | <3 business days |
| Time to Offer | Offer sent date − First screen date | <21 days |
| Interview-to-Offer | Offers / Final round interviews | >50% |

### 3. Quality

| Metric | Formula | Target |
|---|---|---|
| Offer Acceptance Rate | Offers accepted / Offers extended | >85% |
| 90-Day Retention | Employees at 90 days / Total hires | >95% |
| Hiring Manager Satisfaction | Post-hire HM survey score | >4/5 |
| Quality of Hire | Performance score at 6 months | Track over time |

### 4. Source Effectiveness

| Metric | Formula | Why It Matters |
|---|---|---|
| Source-to-Hire | Hires by source / Total hires | Shows where to double down |
| Source-to-Screen | Screens / Applications by source | Quality per channel |
| Cost per Hire | Total recruiting cost / Total hires | Budget efficiency |
| Referral Rate | Referral hires / Total hires | High performers refer high performers |

---

## Weekly CEO Report Template

```
RECRUITING SNAPSHOT — Week of [Date]
Prepared by: [Name]

━━━━━━━━━━━━━━━━━━━━━━━━━━━
OPEN REQS SUMMARY
━━━━━━━━━━━━━━━━━━━━━━━━━━━
Total Open:        [n]
  Active:          [n]
  On Hold:         [n]
  New This Week:   [n]
  Closed This Week:[n]

━━━━━━━━━━━━━━━━━━━━━━━━━━━
PIPELINE HEALTH
━━━━━━━━━━━━━━━━━━━━━━━━━━━
Applications:      [n]  (↑/↓ vs last week)
Screens Completed: [n]  ([x]% conversion)
HM Interviews:     [n]  ([x]% conversion)
Final Rounds:      [n]  ([x]% conversion)
Offers Extended:   [n]
Offers Accepted:   [n]  ([x]% acceptance)

━━━━━━━━━━━━━━━━━━━━━━━━━━━
HIRES CLOSED THIS WEEK
━━━━━━━━━━━━━━━━━━━━━━━━━━━
[n] total hires
  • [Name] | [Role] | Start: [Date] | Source: [channel]
  • [Name] | [Role] | Start: [Date] | Source: [channel]

━━━━━━━━━━━━━━━━━━━━━━━━━━━
VELOCITY
━━━━━━━━━━━━━━━━━━━━━━━━━━━
Avg Time to Fill:  [n] days (target: <45)
Avg Time to Offer: [n] days (target: <21)

━━━━━━━━━━━━━━━━━━━━━━━━━━━
SOURCE BREAKDOWN (MTD)
━━━━━━━━━━━━━━━━━━━━━━━━━━━
LinkedIn Outbound: [x]%
Referrals:         [x]%
Inbound / Apply:   [x]%
Agency:            [x]%
Other:             [x]%

━━━━━━━━━━━━━━━━━━━━━━━━━━━
BLOCKERS & ESCALATIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━
• [Role] — [specific blocker, what you need from leadership]
• [Role] — [specific blocker]

━━━━━━━━━━━━━━━━━━━━━━━━━━━
NEXT WEEK PRIORITIES
━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. [Priority]
2. [Priority]
3. [Priority]
```

---

## Google Sheets Dashboard Setup

### Tab 1: Req Tracker
Columns:
```
Req ID | Role | Level | HM | Status | Open Date | Target Fill | Stage | Pipeline Count | Notes
```

### Tab 2: Candidate Pipeline
Columns:
```
Req ID | Candidate Name | Source | Applied | Screened | HM Interview | Final Round | Offer Date | Decision | Start Date
```

### Tab 3: Metrics (Auto-calculated)
Key formulas:

**Time to Fill:**
```
=IF(AND(K2<>"",C2<>""), NETWORKDAYS(C2,K2), "Open")
```

**Stage Conversion (Screen → HM):**
```
=COUNTIF(F:F,"<>") / COUNTIF(E:E,"<>")
```

**Offer Acceptance Rate:**
```
=COUNTIF(J:J,"Accepted") / COUNTIF(H:H,"<>")
```

**Source Mix:**
```
=COUNTIF(D:D,"LinkedIn") / COUNTA(D:D)
```

### Tab 4: Weekly Snapshot
Pull the key numbers here each Friday → copy/paste into your CEO report.

---

## ATS-Specific Reporting

### Greenhouse
- **Reports → Pipeline** → filter by req, date range, stage
- **Reports → Source** → best for source mix analysis
- **Reports → Time in Stage** → identifies interview process bottlenecks

### Lever
- **Analytics → Pipeline** → stage-by-stage conversion
- **Analytics → Sources** → source quality breakdown
- **Analytics → Velocity** → TTF and stage timing

### Ashby
- **Reporting → Funnel** → most visual, best for CEO presentations
- **Reporting → Hiring Velocity** → TTF by role/team
- Strong built-in dashboards — less manual work than Greenhouse

### SuccessFactors
- Custom report builder: pull req data + candidate stages + offer data
- Export to Excel → build pivot tables for exec reporting

---

## Quarterly Business Review (QBR) Template

```
Q[n] Recruiting QBR — [Quarter/Year]

WHAT WE PLANNED vs. WHAT WE DELIVERED
  Target hires:    [n]
  Actual hires:    [n]
  Attainment:      [x]%

KEY METRICS VS. TARGETS
  Avg TTF:         [n] days  (target: [n])
  Offer accept:    [x]%      (target: >85%)
  Source: Referral [x]%      (target: >30%)
  Quality of hire: [score]   (based on 90-day reviews)

WHAT WORKED
  • [Specific win]
  • [Specific win]

WHAT DIDN'T WORK
  • [Specific miss + root cause]
  • [Specific miss + root cause]

Q[n+1] PLAN
  Headcount plan: [n] hires across [functions]
  Key hard-to-fill roles: [list]
  Investments needed: [tools / agency / headcount]
  Projected TTF: [n] days
```

---

## About

Built by **Chandra Buduri** — Head of TA at Arrcus Series D and Factory VC, where weekly KPI dashboards went directly to the CEO. 10+ years in Talent Acquisition, 1000+ hires closed.

🌐 [Portfolio](https://marvelchandra.github.io/recruiting-portfolio) · 💼 [LinkedIn](https://linkedin.com/in/chandrabuduri)
