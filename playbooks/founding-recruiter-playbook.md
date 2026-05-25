# Founding Recruiter Playbook — Building from 0→1

**For:** First in-house recruiters, founding recruiting hires, early TA leads at seed to Series B startups  
**Maintained by:** Chandra Buduri · [linkedin.com/in/chandrabuduri](https://linkedin.com/in/chandrabuduri)

> This is the playbook I build at every engagement. It's designed for the reality of early-stage companies: no process, no pipeline, urgent roles, and a founding team that's never hired at scale. Everything here is field-tested across 15+ startups from seed through Series D.

---

## The Founding Recruiter Mandate

Being the first recruiter is not the same as being a recruiter at a company that already has recruiting. The job is different in kind, not just in scale.

You are simultaneously:
- The sourcer, screener, coordinator, closer, and onboarder
- The person who builds the infrastructure that outlasts you
- The talent advisor who shapes how the founders think about hiring
- The culture carrier who decides what "good" looks like before anyone else does

The failure mode is spending all your time filling reqs and none building systems. Six months in, you're still running the same manual process on every search. The goal is to build infrastructure fast enough that each hire gets easier — not harder — than the last.

---

## Step 1 — Discovery & Audit (Week 1–2)

Before sourcing a single candidate, understand the company deeply enough to represent it authentically.

### Founder / CEO Intake (60 min, 1:1)

**On the business:**
- What does the company do, and what's the 18-month vision?
- What's the current headcount and what does it need to be in 12 months?
- What are the 3 most critical hires right now — and why those three?
- What's broken without them?

**On hiring history:**
- Who have you hired that you'd clone? What made them exceptional?
- Who didn't work out, and what did you learn?
- Have you worked with recruiters before? What worked, what didn't?

**On culture:**
- How do you describe the way people work here?
- What kind of person fails here?
- What's a non-negotiable value you'd turn down a strong candidate over?

**On compensation:**
- What's the approved comp range for priority roles?
- What's the equity philosophy — how do you think about option grants?
- Are there any constraints (visa sponsorship, remote, relocation)?

### Hiring Manager Intake (45 min, per role)

Run this before writing a JD or sourcing a single profile:

```
Role: _______________
Level: _______________
Team size this person joins: _______________
Reports to: _______________

Must-haves (true dealbreakers):
1.
2.
3.

Nice-to-haves (preferences, not filters):
1.
2.
3.

What does the first 90 days look like?
What does success look like at 6 months? 12 months?
Who is the strongest person you've seen do this job? What made them exceptional?
Where have you looked already? What hasn't worked?
Interview process (stages, interviewers, format):
Target start date:
```

### Audit What Exists

Before building anything, document what's already there:

- [ ] Is there an ATS? If so, what's in it?
- [ ] Are there any job descriptions? Any scorecards?
- [ ] Is there a careers page?
- [ ] How are candidates currently being tracked?
- [ ] Are there any agency relationships or retainers?
- [ ] What does the current offer letter and onboarding process look like?

Present findings to the CEO or Head of People in week 2.

---

## Step 2 — Infrastructure Build (Week 2–4)

Build the minimum viable recruiting stack. Don't over-engineer — build what you need for the next 6 months, not the next 3 years.

### ATS Selection

| ATS | Best for | Key strength |
|---|---|---|
| **Ashby** | Seed–Series B, technical founders | Best analytics, modern UI, strong automation |
| **Greenhouse** | Series B+, investor-recommended | Most integrations, industry standard, scalable |
| **Lever** | Series A–C, CRM-first orgs | Strong nurture/CRM features, good reporting |

Avoid: Workable (limited for technical roles), JazzHR (too basic), Workday (enterprise overhead at wrong stage).

**ATS setup checklist:**
- [ ] Configure job stages: Applied → Recruiter Screen → HM Screen → Technical → Onsite → Offer → Hired
- [ ] Build custom rejection reasons (reviewable, not hired, withdrew, duplicate)
- [ ] Set up email templates (application confirmation, rejection, interview scheduling)
- [ ] Connect to careers page
- [ ] Set up Slack or email notifications for hiring managers
- [ ] Configure reporting: pipeline velocity, conversion rates, time-in-stage, source tracking

### Job Description Template

```markdown
## [Role Title] — [Company Name]

**About [Company]**
2–3 sentences. What you do, why it matters, what stage you're at.
Avoid: "We're a fast-growing startup." Be specific.

**The role**
What will this person actually do? Write in second person ("You will...").
Be honest about what's hard. Early-stage candidates respect candor.

**What you'll do**
4–6 outcome-oriented bullets.
Bad: "Attend team meetings and contribute"
Good: "Own the design and implementation of our real-time inference pipeline"

**What we're looking for**
Must-haves only — 3–5 bullets maximum.
If you'd still interview someone without it, it's not a must-have.

**Nice to have**
2–3 genuine preferences, not disguised requirements.

**Compensation**
- Salary: $X–$Y (be transparent)
- Equity: X–Y options
- Benefits: [list]
- Remote/hybrid/onsite policy

**Interview process**
[List stages and timeline — candidates value this]
```

**JD hygiene rules:**
- No "rockstar," "ninja," "guru," or "passionate"
- No "X+ years" unless legally required — use level descriptors
- No laundry lists — 20 bullets means you haven't prioritized
- Run every JD through a bias checker before posting

### Interview Loop Design

Design the loop before sourcing begins. A loop that doesn't exist when the first candidate arrives creates chaos.

**Standard technical loop (IC roles):**

```
Stage 1: Recruiter Screen (30 min)
  → Purpose: Sell the role, assess baseline fit, check logistics
  → Output: Pass / No Pass / Hold

Stage 2: Hiring Manager Screen (45–60 min)
  → Purpose: Technical depth, experience validation, culture signal
  → Output: Pass / No Pass

Stage 3: Technical Assessment (60–90 min)
  → Format: Take-home OR live coding OR system design (one, not all)
  → Output: Pass / No Pass / Borderline

Stage 4: Onsite / Virtual Onsite (3–4 hours)
  → Deep technical (60 min)
  → System design / architecture (60 min)
  → Cross-functional / working style (45 min)
  → Founder / exec (30 min)
  → Output: Strong Hire / Hire / No Hire / Strong No Hire

Stage 5: Reference Checks (before offer)
  → Minimum 2: 1 manager, 1 peer
  → Ask behavioral questions, not just "would you rehire"
```

**Rules:**
- Every stage must have a defined owner and a scorecard
- No "let's just chat" interviews — every conversation has a stated purpose
- No more than 5 business days between stages
- Debrief within 24 hours of onsite while feedback is fresh

### Scorecard Template

```markdown
## [Role] Interview Scorecard — [Stage]

Interviewer: _______________ | Candidate: _______________ | Date: _______________

| Competency | Weight | Score (1–4) | Evidence / Notes |
|---|---|---|---|
| [Skill 1] | High | | |
| [Skill 2] | High | | |
| [Skill 3] | Medium | | |
| [Culture signal] | Medium | | |
| [Communication] | Low | | |

Scoring:
- 4 = Strong Hire — exceptional, would advocate strongly
- 3 = Hire — meets bar, no significant concerns
- 2 = No Hire — below bar on one or more weighted competencies
- 1 = Strong No Hire — significant concerns

Overall: Strong Hire / Hire / No Hire / Strong No Hire

Top strength:
Primary concern:
Questions for debrief:
```

Run a calibration session with all interviewers before the first candidate screens. Align on what a 4 looks like vs. a 3. Surface disagreements before they affect a real candidate.

---

## Step 3 — Sourcing & Pipeline (Week 3–6)

### Source Mix Targets

| Source | Target % | Notes |
|---|---|---|
| Direct outbound | 50–60% | Highest quality, lowest competition |
| Employee referrals | 20–30% | Fastest time-to-hire, highest retention |
| Inbound / job boards | 10–20% | Volume play, lower signal |
| Agency | 0–10% | Last resort for senior/niche roles |

If you're relying on inbound for more than 30% of pipeline at an early-stage company, you're not sourcing aggressively enough.

### Outbound Sourcing Workflow

1. **Build the target list** — 40–60 names before sending a single message
   - Technical roles: ArXiv, GitHub, Papers With Code, Google Scholar, conference proceedings
   - All roles: LinkedIn X-Ray, SeekOut, Gem
   - Hardware/semiconductor: IEEE Xplore, patent databases

2. **Prioritize by signal strength**
   - Tier 1: Referrals + warm intros → contact immediately
   - Tier 2: Strong match + tenure signals → contact within 48hr
   - Tier 3: Good match, unclear fit → contact in batch

3. **Write personalized outreach**
   - Reference something specific: their paper, repo, company, or project
   - One sentence on why this role fits them specifically
   - One honest sentence on the company (stage and risk included)
   - Clear ask: 20 minutes, not "let me know if you're interested"

4. **Follow-up cadence**
   - Day 1: Initial outreach
   - Day 5: One follow-up if no response
   - Day 10: Final touch — different channel or angle
   - After Day 10: Move on, mark for future nurture

5. **Track everything in ATS**
   - Every sourced name → logged as prospect
   - Every message → logged with date and channel
   - Every response → moved to appropriate stage

### Referral Program Setup

- [ ] Define the referral bonus (cash, equity, or both)
- [ ] Create a simple submission process (Google Form or ATS integration)
- [ ] Send all-hands message from CEO introducing the program
- [ ] Share open roles with the full team weekly
- [ ] Close the loop: tell the referrer what happened and why
- [ ] Pay quickly — slow bonuses kill referral culture

**Referral ask script:**
```
"Hey [Name] — we're hiring a [Role] and I'd love your help.
The ideal person has [2–3 specific criteria].
You don't need to vouch for them — just make the intro and I'll take it from there.
Anyone come to mind?"
```

---

## Step 4 — Candidate Experience (Week 4–8)

Every candidate interaction is a brand impression. You often don't have brand recognition to absorb a bad experience.

**Non-negotiables:**
- Respond to every application within 5 business days
- Confirm every interview within 24 hours of scheduling
- Send an agenda before every onsite
- Debrief and deliver feedback within 48 hours of final interview
- Never ghost — a rejection is better than silence

**Interview day prep (send 24 hours before):**
```
- Confirmed schedule with interviewer names and LinkedIn profiles
- Interview format for each session
- Parking / building access / video link
- Day-of contact number
- What to expect from the process after today
```

---

## Step 5 — Offer Construction

Before extending any offer, align internally on:

- [ ] Compensation (base, bonus if applicable, equity)
- [ ] Equity details (strike price, cliff, vesting, last 409A)
- [ ] Start date
- [ ] Offer expiration (minimum 5 business days — never pressure close)
- [ ] Approval chain (who needs to sign off)

**Offer call structure:**
1. Open with genuine enthusiasm — this is a celebration, not a transaction
2. Walk through comp clearly: base → equity → benefits → total comp
3. Explain equity in plain language — most candidates don't know how to value options
4. Pause: "How are you feeling about this?"
5. Surface objections early — don't wait for a written decline
6. Set a clear follow-up: "I'll send the written offer today. When can we reconnect?"

**Common objections:**

*"The base is lower than I expected"*
→ Understand the gap. Is equity the lever? Be honest about what you can and can't do.

*"I need more time"*
→ "Of course — how long do you need?" Give the time. Pressure-closing loses candidates.

*"I have another offer"*
→ "That's great — can you tell me more?" Understand the competing offer before deciding to compete.

*"I'm worried about startup risk"*
→ Be honest. Share runway, investors, momentum. If you can't make a compelling case, the candidate is right to be worried.

---

## Step 6 — Metrics & Reporting

### Weekly CEO/Founder Sync (30 min)

Come prepared with:

```
Open Roles Update:
[Role] — [# in pipeline] — [Stage breakdown] — [Blockers]

Offers:
[Pending offers, expected close dates]

Hires This Week:
[Names, roles, start dates]

Metrics:
- Total pipeline: X candidates across Y roles
- Interviews scheduled: X
- Offers extended: X | Accepted: X
- Time-to-hire (rolling 30 days): X days

Asks:
- [Decisions needed from founders]
- [Roles needing re-prioritization]
- [Process blockers]
```

### Core Metrics

| Metric | What it tells you | Target |
|---|---|---|
| Time-to-hire | Speed of full process | <30 days IC, <45 days leadership |
| Time-in-stage | Where candidates stall | No stage >7 days |
| Offer acceptance rate | Quality of process + offer | >85% |
| Source-to-hire | Which channels produce hires | Know your best 2 |
| Pipeline conversion | Funnel health by stage | Track week over week |

---

## Step 7 — Common Failure Modes

**Hiring managers who don't give feedback**
→ No scorecard = no debrief = no next candidate. Set this expectation in week 1.

**Interview loops that expand endlessly**
→ Cap at onsite. More than 5 stages signals indecision, not rigor. Candidates notice.

**Founders who interview everyone**
→ Reserve founder time for the final stage only. Define this upfront.

**Slow decisions after onsites**
→ 48-hour debrief and decision SLA. Put it in the interviewer onboarding email.

**No sourcing when the pipeline is full**
→ Build pipeline continuously, not reactively. Next quarter's roles need pipeline built today.

**ATS becomes a black hole**
→ Every candidate should have a clear next action and owner. A weekly 15-min pipeline review prevents candidates going cold.

---

## Step 8 — Templates & Assets Checklist

By end of month 1, you should have:

- [ ] ATS configured with stages, email templates, and rejection reasons
- [ ] Intake questionnaire (role-level and company-level)
- [ ] JD template and at least 3 live JDs
- [ ] Interview loop defined for each active role
- [ ] Scorecards for each interview stage
- [ ] Offer letter template (approved by legal/finance)
- [ ] Referral program live and communicated
- [ ] Weekly hiring sync cadence established with CEO/founders
- [ ] Sourcing pipeline of 30+ names per open role
- [ ] Candidate experience SLAs documented and followed

---

## The 30/60/90 Day Milestones

**Day 30:**
- ATS live and configured
- All active roles have JDs, intake notes, and defined interview loops
- First hires in pipeline for priority roles
- Weekly sync cadence established with founders

**Day 60:**
- First 2–3 hires closed or at offer stage
- Referral program active
- Source mix tracked and reported
- Hiring manager calibration sessions run for all active loops

**Day 90:**
- Recruiting infrastructure documented and replicable
- Metrics dashboard live and shared with leadership
- Employer brand touchpoints improved (careers page, JDs, Glassdoor)
- Pipeline healthy enough that you're ahead of demand, not behind it

---

## Related Files in This Portfolio

| Topic | Location |
|---|---|
| Market mapping & competitive intelligence | [`/market-intelligence/market-mapping-guide.md`](../market-intelligence/market-mapping-guide.md) |
| Compensation benchmarking & band building | [`/market-intelligence/comp-benchmarking-guide.md`](../market-intelligence/comp-benchmarking-guide.md) |
| Employer branding & JD writing | [`/employer-branding/employer-branding-playbook.md`](../employer-branding/employer-branding-playbook.md) |
| Pre-boarding, Day 1, onboarding | [`/onboarding/pre-boarding-checklist.md`](../onboarding/pre-boarding-checklist.md) |
| IT equipment & access procurement | [`/onboarding/it-equipment-procurement-guide.md`](../onboarding/it-equipment-procurement-guide.md) |
| AI/ML sourcing channels | [`/sourcing/ai-ml-sourcing-guide.md`](../sourcing/ai-ml-sourcing-guide.md) |
| Advanced web mining & resume scraping | [`/sourcing/advanced-web-mining-guide.md`](../sourcing/advanced-web-mining-guide.md) |

---

*Part of the [recruiting-portfolio](https://github.com/marvelchandra/recruiting-portfolio) by Chandra Buduri*
