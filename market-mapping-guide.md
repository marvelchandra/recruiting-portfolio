# Market Mapping Guide — Talent Intelligence Before You Source

**For:** Founding recruiters, heads of talent, and recruiting leads running searches in competitive or niche talent markets  
**Maintained by:** Chandra Buduri · [linkedin.com/in/chandrabuduri](https://linkedin.com/in/chandrabuduri)

> Market mapping is the work that happens before sourcing begins. It answers the question every founder eventually asks: "Who are the 50 best people in the world for this role, and where are they?" Done well, it gives you a defensible point of view on the talent landscape — not just names, but pools, movement patterns, and competitive dynamics.

---

## When to Run a Market Map

Not every search needs a full market map. Run one when:

- Any Director+ or leadership search
- First hire in a new domain (first AI/ML hire, first hardware engineer, first sales leader)
- A search that's been open 60+ days without traction
- Founders say "we don't know where to look"
- A role where comp expectations are unclear or contested
- Any search where you're competing against well-funded, well-known companies

For IC roles at known disciplines, a lightweight version (Steps 1–3 below) is usually enough.

---

## Step 1: Define the Talent Pool

Before opening any tool, answer these questions with the hiring manager:

```
What does this person actually do day-to-day?
What's the output we're hiring for, not the inputs?
What prior experience reliably predicts success in this role?
What companies have people doing this exact work?
What's the career path that produces this person?
```

Then build the pool map:

### Primary Feeder Companies
Companies where the highest concentration of qualified people work right now.

```markdown
## Talent Pool Map: [Role Title]

### Primary feeders (most qualified people, highest priority)
| Company | Why they're a fit | Approx. # people |
|---|---|---|
| [Company A] | [specific team or function] | ~[N] |
| [Company B] | [specific team or function] | ~[N] |
| [Company C] | [specific team or function] | ~[N] |

### Secondary feeders (adjacent skills, transferable background)
| Company | Transferable signal | Notes |
|---|---|---|
| [Company D] | [what transfers] | [any caveats] |
| [Company E] | [what transfers] | [any caveats] |

### University pipelines (for research or PhD-level roles)
| Institution | Program | Pipeline strength |
|---|---|---|
| Stanford | CS / AI Lab | Strong |
| Berkeley | EECS / BAIR | Strong |
| CMU | ML Department | Strong |
| MIT | CSAIL | Strong |
| Cornell / Caltech | Varies by domain | Moderate |

### Career path patterns
- [Path 1]: e.g. Backend engineer → ML infra → Staff ML Engineer
- [Path 2]: e.g. PhD researcher → Applied scientist → Research engineer
- [Path 3]: e.g. NVIDIA CUDA engineer → Inference startup → Staff infra
```

---

## Step 2: Size the Market

Calibrate how hard this search will actually be. Present this to founders as context — unrealistic expectations kill searches before they start.

### LinkedIn Signal (Quick Sizing)

Run this search in LinkedIn Recruiter or Sales Navigator:

```
Title: [exact title] OR [variant 1] OR [variant 2]
Location: [target geography]
Skills: [2–3 core skills]
```

| Result count | What it means | Implication |
|---|---|---|
| >10,000 | Wide market | Speed and process are differentiators |
| 2,000–10,000 | Competitive market | Outreach quality and brand matter |
| 500–2,000 | Tight market | Every name matters, expand criteria |
| <500 | Very tight market | Re-scope or open geography |

### Response Rate Signal

After first wave of outreach (20–30 messages sent):

| Response rate | Market temperature | Action |
|---|---|---|
| >35% | Soft — candidates are open | Move fast, you have leverage |
| 20–35% | Normal competitive market | Standard cadence |
| 10–20% | Hot — candidates are fielding offers | Improve outreach, speed up process |
| <10% | Very hot or wrong channel | Change channel, re-examine targeting |

### Tenure Signal (Movement Likelihood)

Use SeekOut or LinkedIn filters to find people at the 18–24 month mark at their current company. This cohort is statistically most likely to be open to a conversation.

```
Filter: Current company tenure = 1.5 – 2.5 years
Cross-reference: Company went through layoffs, funding slowdown, or leadership change
Cross-reference: Recent funding announcements at competitors (people follow opportunity)
```

---

## Step 3: Competitive Landscape Analysis

Who else is hiring for this role right now? What are they offering? What are you up against?

### Active Competitor Mapping

```markdown
## Competitive Landscape: [Role] — [Date]

| Company | Stage | # Open roles (similar) | Known comp range | Hiring speed | Notes |
|---|---|---|---|---|---|
| [Co A] | Series C | 3 | $220–250K | Fast | Strong employer brand |
| [Co B] | Series B | 1 | $200–240K | Slow | Known for long process |
| [Co C] | Public | 5 | $250–300K + RSUs | Medium | Hard to compete on cash |

**Our competitive position:**
- vs. Series C peers: [on par / below / above] on cash; [stronger / weaker] on equity upside
- vs. public companies: below on cash; significantly stronger on equity upside if we exit
- Key differentiator we can lead with: [mission / team / technical challenge / autonomy / upside]
```

### Intelligence Sources

**For active job postings:**
```
LinkedIn Jobs → filter by title, date posted (last 30 days), company size
levels.fyi/jobs → comp-transparent job listings
greenhouse.io/jobs → direct ATS postings
```

**For comp intelligence:**
```
levels.fyi → offer data by company, role, level
blind.co → anonymous candidate chatter on offers and interview experience
glassdoor.com → salary data + interview reviews
teamblind.com → real-time offer comparisons
```

**For company momentum (are they growing or contracting?):**
```
LinkedIn company page → headcount trend (growing / flat / shrinking)
Crunchbase → recent funding rounds
Layoffs.fyi → recent layoffs at target companies
builtin.com → job posting volume as proxy for hiring health
```

---

## Step 4: Talent Movement Patterns

Understanding where people move to and from tells you who's likely open and what's drawing them.

### Movement Mapping Workflow

1. Find 10–15 people who recently left your target feeder companies
2. Track where they went
3. Identify the pattern — are they going to startups? Bigger companies? Specific competitors?

```markdown
## Movement Map: [Feeder Company] Alumni (last 12 months)

| Name (anonymized) | Left | Went to | Why (if known) | Signal |
|---|---|---|---|---|
| Sr ML Engineer | Google Brain | Mistral AI | Founding team equity | Startup open |
| Staff Engineer | Meta AI | Anthropic | Mission + comp | Mission-driven |
| Research Scientist | OpenAI | Started own co | Autonomy | Entrepreneurial |
| Principal Engineer | NVIDIA | Series B startup | Equity | Startup open |
```

### Signals That Someone Is Likely Open

- Tenure at current company: 18–24 months
- Their company recently had layoffs (even if they weren't affected — culture shifts)
- Their company recently had a down round or funding struggles
- They recently posted on LinkedIn (engagement = active presence = more receptive)
- They recently spoke at a conference or published a paper (public visibility = open to conversations)
- Their manager or close colleagues recently left

---

## Step 5: The One-Page Market Map Deliverable

Present to founders and hiring managers as a single-page brief. This is what earns trust as a strategic partner — not just a sourcer.

```markdown
## Market Map: [Role Title]
**Prepared by:** Chandra Buduri · **Date:** [Date] · **Search:** [Company] / [Role]

---

### Talent Pool
Approximately [N] qualified people in [geography] match this profile.
Top feeder companies: [Co A], [Co B], [Co C], [Co D], [Co E]
Key career paths: [1–2 sentence summary]

### Market Temperature
**[Hot / Competitive / Accessible]**
[2–3 sentences explaining why — response rates, competing offers, market dynamics]

### Competitive Landscape
We are competing primarily against [type of company].
Our strongest differentiator: [specific, honest answer]
Our biggest comp challenge: [specific, honest answer]

### Sourcing Strategy
Primary channels: [top 2–3 channels for this specific search]
Secondary channels: [1–2 backup channels]
Estimated pipeline needed: [N] qualified prospects to generate [N] offers

### Comp Expectation
Base: $[X] – $[Y] (market P50: $[Z])
Equity: [X,000 – Y,000] options (see comp benchmarking doc)
Total comp at midpoint: ~$[Z]

### Realistic Timeline
Time-to-first-qualified-candidate: [X] weeks
Time-to-offer: [X] weeks from start
Full time-to-hire estimate: [X–Y] weeks

### Risks & Mitigations
| Risk | Likelihood | Mitigation |
|---|---|---|
| Below-market cash comp | Medium | Lead with equity story and upside |
| Long interview process | Low | Process already defined — commit to <3 week close |
| Low brand recognition | Medium | Personalized outreach referencing their specific work |
| Visa / relocation required | [depends] | [specific plan] |

### Recommendation
[2–3 sentences: go / no-go / modify criteria / adjust comp]
```

---

## Appendix: Market Mapping Tool Stack

| Tool | Use | Cost |
|---|---|---|
| LinkedIn Recruiter | Pool sizing, movement tracking, tenure filters | Paid |
| SeekOut | Advanced filters: publications, patents, OSS, diversity | Paid |
| Crunchbase | Company funding, headcount, momentum | Freemium |
| Layoffs.fyi | Recent layoffs at target companies | Free |
| Levels.fyi | Comp data by company/role/level | Free |
| Glassdoor | Interview reviews, salary ranges, culture signals | Free |
| Blind / Teamblind | Real-time candidate chatter on offers | Free |
| LinkedIn Company Pages | Headcount trends | Free |
| Google X-Ray | Profile mining beyond LinkedIn network | Free |

---

*Part of the [recruiting-portfolio](https://github.com/marvelchandra/recruiting-portfolio) by Chandra Buduri*
