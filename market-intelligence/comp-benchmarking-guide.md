# Compensation Benchmarking Guide — Building Comp Bands That Win Candidates

**Maintained by:** Chandra Buduri · [linkedin.com/in/chandrabuduri](https://linkedin.com/in/chandrabuduri)

> Comp is rarely the only reason a candidate accepts or declines. But it's almost always the first reason a candidate self-selects out. Getting comp right means being competitive enough to stay in the conversation — and structured enough to make offers confidently.

---

## Part 1: Data Sources

### Primary Sources by Use Case

| Source | Best for | Precision | Cost |
|---|---|---|---|
| **Levels.fyi** | Software, ML, data roles at tech companies | High | Free |
| **Pave** | Startup-specific, all functions, equity data | High | Paid (startup pricing) |
| **Radford (Aon)** | Enterprise benchmark, all functions | Very high | Paid (subscription) |
| **Carta Total Comp** | Early-stage startups, equity modeling | High | Free with Carta |
| **Glassdoor** | General market sentiment | Medium | Free |
| **Blind / Teamblind** | Real-time offer data, candidate chatter | Medium | Free |
| **LinkedIn Salary** | Broad market, less precise | Low-Medium | Free (limited) |
| **Offer letters (internal)** | Most accurate — your own closed offers | Very high | Internal |
| **Recruiter network** | Qualitative, directional | Medium | Relationships |

### How to Triangulate

Never rely on a single source. For each role, pull from at least 3:

```
Step 1: Levels.fyi → get tech-company P50 for the title and level
Step 2: Pave or Radford → get startup-adjusted range (typically 10–15% below big tech)
Step 3: Blind/Glassdoor → gut-check against candidate-reported offers
Step 4: Internal offer history → anchor to what you've actually closed
Step 5: Recruiter network → qualitative sense of current market movement
```

---

## Part 2: Building a Comp Band

### The Four-Step Process

**Step 1: Define the level**

Before pulling data, define what level this role actually is. Most comp misalignment comes from level disagreement, not data disagreement.

```markdown
## Level Definition: [Role]

| Level | Criteria | Typical YOE | Decision autonomy |
|---|---|---|---|
| Mid (L3/L4) | Executes defined work with some guidance | 3–6 years | Task-level |
| Senior (L5) | Owns work end-to-end, raises quality of team | 6–10 years | Project-level |
| Staff (L6) | Multiplies others, drives cross-team initiatives | 10+ years | Team-level |
| Principal (L7) | Shapes org direction, defines technical strategy | 12+ years | Org-level |

**This role is:** [Level] because [specific rationale]
```

**Step 2: Pull market data**

For each data source, record the P25, P50, and P75 for base salary and total compensation:

```markdown
## Raw Market Data: [Role Title] — [Level] — [Geography] — [Date]

| Source | Base P25 | Base P50 | Base P75 | Total TC P50 | Notes |
|---|---|---|---|---|---|
| Levels.fyi | $X | $Y | $Z | $Y | N=[sample size] |
| Pave | $X | $Y | $Z | $Y | Startup-adjusted |
| Radford | $X | $Y | $Z | $Y | [survey date] |
| Glassdoor | $X | $Y | $Z | $Y | Self-reported |
| Blind | $X | $Y | $Z | $Y | Anecdotal |
| Internal history | $X | $Y | $Z | $Y | Last [N] offers |

**Composite P50 (average across sources):**
- Base: $[X]
- Total cash: $[X]
- Total comp (incl. equity at 409A): $[X]
```

**Step 3: Apply startup adjustment**

If you're an early-stage company, you typically cannot match big tech on cash. Know your discount and compensate with equity:

```
Startup cash discount vs. big tech:
- Seed: 20–30% below big tech P50 on base
- Series A: 15–25% below
- Series B: 10–15% below
- Series C: 5–10% below
- Pre-IPO: at or near market (recruiting against public cos directly)

Equity premium to offset cash discount:
- The option grant should be meaningful enough that candidates can model
  a realistic scenario where total compensation exceeds the big tech offer
  upon exit
```

**Step 4: Set the band**

```markdown
## Approved Comp Band: [Role] — [Level]

**Base salary:**
| Position in band | Amount | Used for |
|---|---|---|
| Floor (P25) | $[X] | Candidates below market expectations or limited experience |
| Midpoint (P50) | $[X] | Standard offer for fully qualified candidates |
| Ceiling (P75) | $[X] | Exceptional candidates, competing offers, retention risk |
| Above band (exception) | $[X]+ | Requires CEO/CFO approval |

**Equity grant (options, 4-year vest, 1-year cliff):**
| Position in band | # Options | Value at 409A | Approx. annual vest value |
|---|---|---|---|
| Floor | [N] | $[X] | $[X]/yr |
| Midpoint | [N] | $[X] | $[X]/yr |
| Ceiling | [N] | $[X] | $[X]/yr |

**Signing bonus (if applicable):**
| Scenario | Amount | Rationale |
|---|---|---|
| Unvested equity left behind | $[X] | Bridge to compensate for walk-away cost |
| Competing offer gap | $[X] | One-time close tool, not base comp |
| Relocation | $[X] | Actual cost coverage |

**Total comp at midpoint:**
- Base: $[X]
- Equity (annual vest value at 409A): $[X]
- Benefits value: ~$[X]
- **Total: ~$[X]**

**Approval required:**
- Within band: Recruiting Lead sign-off
- At ceiling: VP/Head of Department sign-off
- Above band: CEO + CFO sign-off
```

---

## Part 3: The Comp Band Spreadsheet

Build this in Google Sheets or Excel. One tab per function, updated quarterly.

### Sheet Structure

**Tab 1: Master Band Table**

| Role | Level | Base Floor | Base Mid | Base Ceiling | Equity Floor | Equity Mid | Equity Ceiling | Last Updated | Source |
|---|---|---|---|---|---|---|---|---|---|
| ML Engineer | L4/Mid | $180K | $200K | $220K | 15K opts | 22K opts | 30K opts | Q1 2025 | Levels/Pave |
| ML Engineer | L5/Senior | $220K | $245K | $270K | 30K opts | 45K opts | 60K opts | Q1 2025 | Levels/Pave |
| ML Engineer | L6/Staff | $270K | $300K | $335K | 60K opts | 90K opts | 120K opts | Q1 2025 | Levels/Pave |
| Software Eng | L4/Mid | $165K | $185K | $205K | 12K opts | 18K opts | 25K opts | Q1 2025 | Levels/Pave |
| Software Eng | L5/Senior | $200K | $225K | $250K | 25K opts | 38K opts | 50K opts | Q1 2025 | Levels/Pave |
| AE | Mid-Market | $100K | $120K | $140K | 8K opts | 12K opts | 18K opts | Q1 2025 | Pave/Glassdoor |
| AE | Enterprise | $130K | $155K | $180K | 12K opts | 18K opts | 25K opts | Q1 2025 | Pave/Glassdoor |

**Tab 2: Equity Value Calculator**

| Input | Value |
|---|---|
| Current 409A (common stock price) | $[X] |
| Last preferred price (most recent round) | $[X] |
| Current option pool | [N] shares |
| Total shares outstanding (fully diluted) | [N] shares |

| Scenario | Exit multiple | Company valuation | Common stock value | Value per option |
|---|---|---|---|---|
| Conservative | 3x | $[X] | $[X] | $[X] |
| Base case | 5x | $[X] | $[X] | $[X] |
| Optimistic | 10x | $[X] | $[X] | $[X] |

**Tab 3: Offer Tracker**

| Candidate | Role | Level | Base offered | Equity offered | Signing | Accepted? | Competing offer | Decline reason |
|---|---|---|---|---|---|---|---|---|
| [Name] | Sr ML Eng | L5 | $245K | 45K opts | $0 | Yes | Google $280K TC | — |
| [Name] | Staff Eng | L6 | $300K | 90K opts | $25K | No | Anthropic $380K TC | Comp gap |

**Tab 4: Market Data Log**

Track every data point you gather, with date and source. This builds your own proprietary comp intelligence over time.

| Date | Role | Level | Geography | Source | Base P50 | Total TC P50 | Notes |
|---|---|---|---|---|---|---|---|
| [Date] | Sr ML Eng | L5 | SF Bay | Levels.fyi | $245K | $380K | N=142 data points |
| [Date] | Sr ML Eng | L5 | SF Bay | Recruiter network | $240–260K | N/A | Directional |

---

## Part 4: Equity Modeling for Candidates

Most candidates — even senior engineers — don't know how to value startup equity. Help them model it. This is one of the most effective closing tools available to a recruiter.

### The Five Questions to Ask Before Modeling

Before showing a candidate any numbers, get these from the finance team:

```
1. What is the current 409A valuation (common stock strike price)?
2. What was the last round price (preferred)?
3. How many shares outstanding (fully diluted cap table)?
4. What is the liquidation preference structure?
5. What exit scenarios are the investors modeling?
```

### Equity Conversation Script

```
"I want to walk you through how to think about the equity,
because I know option grants can feel abstract compared to RSUs.

You'd receive [N] options at a strike price of $[X].
The most recent 409A valued the common stock at $[Y].
So today, on paper, your grant is worth approximately $[Z].

Here's how to think about upside:
Our last round was at a $[X]M valuation.
If we exit at 3x that — which is a conservative outcome for a company at our stage —
your grant would be worth approximately $[A].
At 5x, you're looking at $[B].
At 10x — which is what our investors are underwriting — $[C].

That vests over 4 years with a 1-year cliff.
So in year 1 you get 25% of that, roughly $[D] at the base case.

Compare that to the RSU offer you have:
$[X] in RSUs vesting over 4 years at a company that's already fully valued
and has limited room to move from here.

The question isn't which is worth more today.
The question is: which do you think will be worth more in 4 years?"
```

### Underwater Options — How to Handle It

If your 409A has moved significantly since the last round (common in down markets), options may be close to or at the money. Be transparent:

```
"I want to be straightforward with you about the equity.
The 409A was set at $[X], and the last preferred round was at $[Y].
There's a gap — the common is worth less than the preferred right now.
What that means is: the equity upside is real, but it depends on the company
getting to a meaningful exit above the current preferred stack.
I'd rather you go in with eyes open than be surprised later."
```

Candidates respect honesty here. The ones who self-select in are more committed.

---

## Part 5: Presenting Comp Data to Leadership

Comp conversations with founders go sideways when recruiters arrive with opinions instead of data. Always lead with market data, then recommendation.

### Comp Review Presentation Structure (15 min)

```markdown
## Comp Review: [Role] — [Date]

**Market context (5 min)**
"Here's what the market looks like for this role right now..."
[Show the comp band table with sources]

**Our current position (3 min)**
"Here's where our approved band sits relative to market..."
[Show gap analysis — are we at P50? Below? Above?]

**Offer recommendation (5 min)**
"For [Candidate], I'm recommending..."
[Base / equity / signing — and the rationale]

**Decision needed (2 min)**
"To move forward, I need sign-off on [specific number or range]."
[Clear ask — don't leave the meeting without a decision]
```

### When You Need to Raise the Band

Bring data, not feelings:

```
"We've had 3 strong candidates decline in the last 6 weeks.
In two cases they cited comp — they accepted offers averaging $[X] base.
Our ceiling is currently $[Y], which is $[Z] below what they took.

I'm recommending we raise the ceiling to $[X] for this level.
Here's what Levels.fyi and Pave show for the current market..."
```

---

## Part 6: Comp Band Maintenance

Comp data goes stale. Market moves fast — especially in AI/ML where demand outpaces supply.

### Refresh Triggers

| Trigger | Action |
|---|---|
| Offer declined citing comp | Immediate comp review for that role |
| 2+ declines citing comp in 30 days | Band revision required |
| New funding round (yours or competitor) | Full band refresh |
| 6 months since last update | Scheduled quarterly review |
| Candidate brings competing offer | Document the offer, update tracking sheet |
| New data from Levels/Pave/Radford | Update source row, recalculate composite |

### Quarterly Comp Review Agenda (30 min with Finance/CFO)

```
1. Offer acceptance rate last quarter (target: >85%)
2. Decline reasons — how many were comp-related?
3. Competing offers received — what were they?
4. Market data update by function
5. Band adjustments needed
6. Budget impact of proposed changes
7. Approved band for next quarter
```

---

## Appendix: Comp Band Template (Copy-Paste Ready)

```markdown
## Comp Band: [Company Name] — [Date] — [Confidential]

**409A (current):** $[X] per share
**Last round price:** $[X] per share (Series [X], [Date])

---

### Engineering

| Role | Level | Base Floor | Base Mid | Base Ceiling | Options Floor | Options Mid | Options Ceiling |
|---|---|---|---|---|---|---|---|
| Software Engineer | L3 | | | | | | |
| Software Engineer | L4 | | | | | | |
| Senior Software Engineer | L5 | | | | | | |
| Staff Software Engineer | L6 | | | | | | |
| Principal Engineer | L7 | | | | | | |
| ML Engineer | L4 | | | | | | |
| Senior ML Engineer | L5 | | | | | | |
| Staff ML Engineer | L6 | | | | | | |

### GTM

| Role | Level | Base Floor | Base Mid | Base Ceiling | OTE Floor | OTE Mid | OTE Ceiling | Options Mid |
|---|---|---|---|---|---|---|---|---|
| BDR/SDR | | | | | | | | |
| Account Executive (MM) | | | | | | | | |
| Account Executive (Enterprise) | | | | | | | | |
| Solutions Engineer | | | | | | | | |
| Customer Success Manager | | | | | | | | |

### Product & Design

| Role | Level | Base Floor | Base Mid | Base Ceiling | Options Floor | Options Mid | Options Ceiling |
|---|---|---|---|---|---|---|---|
| Product Manager | L4 | | | | | | |
| Senior Product Manager | L5 | | | | | | |
| Staff Product Manager | L6 | | | | | | |
| Product Designer | L4 | | | | | | |
| Senior Product Designer | L5 | | | | | | |

### G&A

| Role | Level | Base Floor | Base Mid | Base Ceiling | Options Mid |
|---|---|---|---|---|---|
| Recruiter | Mid | | | | |
| Senior Recruiter | Senior | | | | |
| Head of Finance | | | | | |
| Legal Counsel | | | | | |

---

**Approval:** CEO _______ CFO _______ Date _______
**Next review:** [Date]
```

---

*Part of the [recruiting-portfolio](https://github.com/marvelchandra/recruiting-portfolio) by Chandra Buduri*
