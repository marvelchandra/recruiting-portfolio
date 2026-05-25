# Advanced Sourcing: Web Crawling, Resume Mining & Deep Candidate Intelligence

**Level:** Advanced  
**For:** Technical recruiters doing deep passive sourcing in AI/ML, Semiconductor, Infrastructure, and GTM  
**Maintained by:** Chandra Buduri · [linkedin.com/in/chandrabuduri](https://linkedin.com/in/chandrabuduri)

> This guide covers methods that go significantly beyond LinkedIn Recruiter. Everything here is legal, uses publicly available data, and follows robots.txt and platform ToS. The goal is to find candidates that no other recruiter has already messaged.

---

## Part 1: X-Ray Search (Google Boolean Deep Crawling)

X-Ray search uses Google to crawl the public-facing index of any website — including LinkedIn, GitHub, university pages, company directories, and resume hosting sites. Google's crawler has already indexed billions of pages; you're just querying it with precision.

### The Core X-Ray Formula

```
site:[domain] "[role keyword]" "[location]" "[skill]" -intitle:"jobs" -intitle:"hiring"
```

The `-intitle` exclusions filter out job postings and recruiting noise, leaving actual profiles and resumes.

---

### 1.1 LinkedIn X-Ray

LinkedIn blocks most profile views without login — but Google has already crawled and indexed public profiles. This surfaces candidates you cannot find inside LinkedIn Recruiter because they have privacy settings, no premium, or are outside your network.

**Staff ML Engineer — Bay Area:**
```
site:linkedin.com/in "staff engineer" OR "principal engineer" ("machine learning" OR "deep learning") (pytorch OR jax OR tensorflow) "San Francisco" OR "Bay Area" OR "California"
```

**AI Research Scientist — PhD required:**
```
site:linkedin.com/in "research scientist" ("PhD" OR "Ph.D") (NeurIPS OR ICML OR ICLR OR CVPR OR "arxiv") ("machine learning" OR "deep learning" OR "AI")
```

**LLM / GenAI Engineers:**
```
site:linkedin.com/in ("large language model" OR LLM OR "generative AI" OR "foundation model") ("engineer" OR "researcher") (pytorch OR "fine-tuning" OR RLHF OR vllm OR triton)
```

**ASIC / Hardware Engineers (Semiconductor):**
```
site:linkedin.com/in ("ASIC design" OR "RTL design" OR "physical design" OR "SoC") ("Synopsys" OR "Cadence" OR "Mentor") "San Jose" OR "Santa Clara" OR "Austin"
```

**PCIe / CXL Engineers:**
```
site:linkedin.com/in ("PCIe" OR "CXL" OR "SerDes") ("verification engineer" OR "design engineer" OR "architect") ("Broadcom" OR "Marvell" OR "Intel" OR "AMD" OR "Astera")
```

**Compiler / Runtime Engineers:**
```
site:linkedin.com/in ("compiler engineer" OR "runtime engineer" OR "LLVM" OR "MLIR") ("machine learning" OR "AI" OR "GPU" OR "accelerator")
```

**GTM — Enterprise AE, deep tech:**
```
site:linkedin.com/in ("account executive" OR "AE") ("enterprise" OR "strategic") ("infrastructure" OR "cloud" OR "networking" OR "AI") "quota" OR "ARR" OR "ACV"
```

**Solutions Engineer / Pre-Sales:**
```
site:linkedin.com/in ("solutions engineer" OR "sales engineer" OR "pre-sales") ("networking" OR "cloud" OR "AI/ML" OR "infrastructure") "San Francisco" OR "Austin" OR "New York"
```

---

### 1.2 GitHub X-Ray

GitHub profiles are fully public and indexed. This reaches engineers who are not active on LinkedIn at all.

**ML Framework Contributors:**
```
site:github.com "machine learning" "open to opportunities" OR "open to work" location:"San Francisco" OR "Bay Area"
```

**CUDA / GPU Engineers:**
```
site:github.com "CUDA" "triton" OR "tensor cores" "machine learning" location:"United States"
```

**Distributed Systems / Infrastructure:**
```
site:github.com "distributed systems" "golang" OR "rust" OR "C++" "kubernetes" OR "eBPF" OR "DPDK" location:"San Francisco"
```

**Compiler Engineers:**
```
site:github.com "LLVM" OR "MLIR" "compiler" "machine learning" OR "GPU" OR "accelerator"
```

**Firmware / Embedded Engineers:**
```
site:github.com "firmware" "embedded systems" "RTOS" OR "bare metal" "C" OR "C++"
```

---

### 1.3 University Faculty & Lab Pages

University lab pages list PhD students, postdocs, and research staff — most of whom are not on LinkedIn or have minimal profiles. These are the highest-signal passive candidates for research roles.

**Stanford AI Lab:**
```
site:ai.stanford.edu "PhD student" OR "postdoc" OR "research scientist" [topic]
```

**Berkeley AI Research (BAIR):**
```
site:bair.berkeley.edu "PhD" OR "graduate student" OR "researcher" [topic]
```

**MIT CSAIL:**
```
site:csail.mit.edu "graduate student" OR "postdoctoral" OR "research scientist" [topic]
```

**CMU ML Department:**
```
site:ml.cmu.edu "PhD student" OR "research" [topic]
```

**Broad search across all top programs:**
```
site:*.edu "PhD student" "machine learning" OR "deep learning" (pytorch OR jax OR tensorflow) "graduating" OR "graduation" OR "2024" OR "2025"
```

**Finding candidates about to graduate (pipeline building):**
```
site:*.edu "PhD candidate" "machine learning" "expected graduation 2024" OR "expected graduation 2025"
```

---

### 1.4 Resume & CV Mining

Many researchers and engineers post their CVs publicly — on personal sites, university pages, or resume hosting platforms. These contain full work history, publications, and skills in a single document.

**CVs on university pages:**
```
site:*.edu filetype:pdf "curriculum vitae" "machine learning" "San Francisco" OR "Bay Area" OR "California"
```

**CVs on personal sites:**
```
filetype:pdf "curriculum vitae" "machine learning engineer" OR "ML researcher" site:github.io OR site:*.io
```

**Resumes on public hosting:**
```
site:resume.io OR site:visualcv.com "machine learning" "pytorch" OR "tensorflow" "San Francisco"
```

**General resume mining by role:**
```
filetype:pdf OR filetype:doc "resume" "staff engineer" "machine learning" "San Francisco" -site:job -site:indeed -site:glassdoor
```

**PhD CV mining — semiconductor:**
```
site:*.edu filetype:pdf "curriculum vitae" ("VLSI" OR "ASIC" OR "RTL" OR "SoC") "PhD" 2023 OR 2024
```

**Compiler/PL researcher CVs:**
```
site:*.edu filetype:pdf "curriculum vitae" ("LLVM" OR "MLIR" OR "compiler" OR "programming language") "PhD"
```

---

## Part 2: Platform-Specific Deep Mining

### 2.1 Google Scholar Profile Mining

Scholar profiles are public and contain full publication history, citation counts, co-authors, and institutional affiliations.

**Search by research topic + institution:**
```
scholar.google.com → "reinforcement learning from human feedback" → filter by Recent → click author names
```

**Citation network traversal:**
1. Find a landmark paper (e.g. "InstructGPT", "LoRA", "Flash Attention")
2. Click "Cited by [N]"
3. Sort by Recent
4. Every recent citing author is an active researcher in that area
5. Click their profile → get co-authors → repeat

**Google Scholar X-Ray:**
```
site:scholar.google.com "machine learning" "UC Berkeley" OR "Stanford" OR "CMU" 2023 OR 2024
```

**Finding researchers at companies (not just academia):**
```
site:scholar.google.com "Google DeepMind" OR "Meta AI" OR "Microsoft Research" "machine learning" 2024
```

---

### 2.2 Semantic Scholar

Semantic Scholar (by Allen Institute for AI) has better filtering than Google Scholar and shows author affiliations, h-index, and field of study.

**URL pattern for topic search:**
```
semanticscholar.org/search?q=[TOPIC]&sort=Relevance&fields-of-study=Computer+Science
```

**Examples:**
```
semanticscholar.org/search?q=efficient+transformer+inference&sort=Total+Citations
semanticscholar.org/search?q=RLHF+language+model&sort=Pub+Date
semanticscholar.org/search?q=graph+neural+network+drug+discovery&sort=Total+Citations
```

**What to do:**
- Click paper → Authors tab → click author profiles
- Filter by "Highly Influential Citations" to find who the field considers most credible
- Check "Fields of Study" to confirm relevance

---

### 2.3 ORCID

ORCID is a researcher identifier system — nearly every active academic researcher has one. Profiles include employment history, publications, grants, and peer review activity.

**Search:**
```
orcid.org/orcid-search/search?searchQuery=[NAME+OR+TOPIC]
```

**X-Ray via Google:**
```
site:orcid.org "machine learning" "San Francisco" OR "Bay Area"
site:orcid.org "ASIC" OR "VLSI" "PhD" employment:[company]
```

**Why it matters:** ORCID profiles often contain current employer even when LinkedIn is sparse or absent. Useful for verifying researcher identity and finding contact email (many link to institutional pages with public email).

---

### 2.4 ResearchGate

ResearchGate is a researcher social network with 20M+ members. Profiles include papers, questions asked/answered (shows domain depth), and follower networks.

**X-Ray:**
```
site:researchgate.net "machine learning" "PhD" "San Francisco" OR "Mountain View" OR "Menlo Park"
site:researchgate.net "ASIC design" OR "SoC" OR "PCIe" "engineer" OR "researcher"
```

**Topic pages:**
```
researchgate.net/topic/Machine-Learning → Members tab → filter by institution/location
researchgate.net/topic/Compiler-Design → Members tab
```

---

### 2.5 IEEE Xplore (Semiconductor & Hardware)

IEEE Xplore is the primary publication database for electrical engineering and computer science hardware research.

**Author search:**
```
ieeexplore.ieee.org/search/searchresult.jsp?queryText=[AUTHOR+NAME]&newsearch=true
```

**Topic + recent papers:**
```
ieeexplore.ieee.org/search/searchresult.jsp?queryText=PCIe+CXL+2023&newsearch=true
ieeexplore.ieee.org/search/searchresult.jsp?queryText=ASIC+machine+learning+accelerator+2024
```

**Conference-specific mining (ISSCC, HotChips, DAC):**
```
site:ieeexplore.ieee.org "ISSCC 2024" "SerDes" OR "PCIe" OR "CXL"
site:ieeexplore.ieee.org "DAC 2023" "RTL" OR "physical design" OR "SoC"
```

**X-Ray via Google:**
```
site:ieeexplore.ieee.org "neural network accelerator" "ASIC" 2023 OR 2024
```

---

### 2.6 ACL Anthology (NLP / Computational Linguistics)

The ACL Anthology indexes every paper from ACL, EMNLP, NAACL, EACL, and related NLP venues.

**Search:**
```
aclanthology.org/?search=[TOPIC]
```

**Examples:**
```
aclanthology.org/?search=instruction+tuning
aclanthology.org/?search=retrieval+augmented+generation
aclanthology.org/?search=code+generation+LLM
```

**What to do:**
- Click paper → author names are linked → click author → see all their papers
- Check author affiliation in the paper PDF
- Cross-reference on LinkedIn and Google Scholar

---

### 2.7 OpenReview (ICLR & NeurIPS)

OpenReview hosts the submission and review process for ICLR and increasingly NeurIPS. It shows paper authors, reviewer identities (when public), and full review threads — giving you signal on who the *community* considers credible, not just who published.

**Search:**
```
openreview.net/search?term=[TOPIC]&group=ICLR.cc
openreview.net/search?term=[TOPIC]&group=NeurIPS.cc
```

**Examples:**
```
openreview.net/search?term=efficient+attention&group=ICLR.cc/2024
openreview.net/search?term=multimodal+learning&group=NeurIPS.cc/2023
```

**Why it matters:** Accepted papers at ICLR/NeurIPS are peer-reviewed. Spotlight and Oral papers = top 5% of submissions. Authors of these are among the strongest researchers globally.

---

## Part 3: Automated Pipeline Enrichment

### 3.1 Clearbit / People Data Labs (PDL)

For enriching a name + company into a full profile (email, LinkedIn URL, title, location):

**PDL API — find person by name + company:**
```json
POST https://api.peopledatalabs.com/v5/person/enrich
{
  "name": "Jane Smith",
  "company": "Anthropic",
  "location": "San Francisco"
}
```

Returns: email, LinkedIn URL, GitHub, Twitter, job history, education, skills.

**Use case:** You found a name on ArXiv or a conference paper. You don't have their contact. PDL can surface their professional email and LinkedIn in one API call.

---

### 3.2 Hunter.io (Email Finding)

For finding professional emails by name + domain:

```
hunter.io/find?domain=[company.com]&first_name=[First]&last_name=[Last]
```

**Bulk email pattern discovery:**
```
hunter.io/domain-search?domain=[company.com]
```
→ Shows the email pattern used by the company (e.g. first.last@company.com, first@company.com)
→ Apply pattern to names found via other channels

---

### 3.3 Prospeo / Skrapp / Snov.io

LinkedIn email extractors — find professional emails directly from LinkedIn profile URLs.

**Workflow:**
1. Build a list of LinkedIn profile URLs from X-Ray search
2. Run through Prospeo or Snov.io bulk finder
3. Get verified professional emails for direct outreach

**Snov.io URL finder:**
```
app.snov.io → Email Finder → LinkedIn URL input → returns verified email
```

---

### 3.4 GitHub API — Contributor Mining at Scale

GitHub's public API lets you pull contributor lists from any repo without manual browsing.

**Get contributors for a repo:**
```
https://api.github.com/repos/huggingface/transformers/contributors?per_page=100&page=1
```

**Get a user's profile:**
```
https://api.github.com/users/[USERNAME]
```
Returns: name, company, location, email (if public), blog URL, bio, followers, public repos.

**Get all repos a user contributes to:**
```
https://api.github.com/users/[USERNAME]/repos
```

**Practical workflow:**
```bash
# Pull top 100 contributors to vLLM
curl "https://api.github.com/repos/vllm-project/vllm/contributors?per_page=100" \
  | jq '.[].login' \
  | xargs -I {} curl "https://api.github.com/users/{}" \
  | jq '{name: .name, company: .company, location: .location, email: .email, blog: .blog}'
```

This gives you a structured list of top OSS contributors with company, location, and sometimes email — in minutes.

---

### 3.5 SeekOut Advanced Filters (Platform)

SeekOut crawls GitHub, ArXiv, patents, and publications and surfaces them inside a recruiter-friendly UI. Key filters most recruiters miss:

**Diversity sourcing filters:**
- `Diversity: Women in Tech` — surfaces female engineers from underrepresented backgrounds
- `Likely to move` — ML model predicting job change likelihood based on tenure and engagement signals

**Publication filters:**
- Filter by number of publications, citation count, h-index
- Filter by publication venue (NeurIPS, ICML, ICLR, CVPR, ACL)
- Filter by co-author at target companies

**Open source filters:**
- Filter by GitHub contributions > N commits
- Filter by programming language
- Filter by OSS project name

**Patent filters (semiconductor):**
- Filter by patent count
- Filter by patent topic (PCIe, ASIC, SerDes, machine learning accelerator)

---

## Part 4: Resume Board Mining

### 4.1 Indeed Resume Database

Indeed's resume database is publicly crawlable for basic search but full profiles require a paid account.

**X-Ray for resumes:**
```
site:indeed.com/r "machine learning engineer" "San Francisco" pytorch 2023
site:indeed.com/r "ASIC design engineer" "San Jose" "Synopsys" OR "Cadence"
```

### 4.2 Dice.com (Tech-Specific)

Dice has a deep database of tech professionals, particularly strong for infrastructure, DevOps, and systems engineers.

**X-Ray:**
```
site:dice.com "machine learning" "kubernetes" "MLOps" "San Francisco"
site:dice.com "firmware engineer" "embedded" "RTOS" "Austin" OR "San Jose"
```

### 4.3 Stack Overflow Careers / Developer Survey

Stack Overflow's Developer Survey publishes anonymized but searchable data on technology usage. The careers section has public profiles.

**X-Ray:**
```
site:stackoverflow.com/users "machine learning" "python" "pytorch" location:"United States"
```

### 4.4 Kaggle Profiles (Deep Mining)

Beyond browsing the leaderboard, Kaggle profiles are fully indexed.

**X-Ray:**
```
site:kaggle.com "grandmaster" "NLP" "San Francisco" OR "Bay Area"
site:kaggle.com "master" "computer vision" "pytorch" "United States"
```

**Kaggle Discussion Mining:**
Top Kagglers often post in discussion forums — their writing quality and domain knowledge is visible and searchable.

---

## Part 5: Patent Mining (Semiconductor & Hardware)

Patents are a goldmine for semiconductor and hardware sourcing. Inventors are named on every patent — and patent databases are fully public.

### 5.1 Google Patents

**Search by technology + company:**
```
patents.google.com/?q=PCIe+CXL+memory+controller&assignee=Broadcom
patents.google.com/?q=machine+learning+accelerator+ASIC&assignee=NVIDIA
patents.google.com/?q=SerDes+retimer&assignee=Astera+Labs
```

**Search by inventor name:**
```
patents.google.com/?inventor=LAST+FIRST&assignee=COMPANY
```

**What to look for:**
- Inventor names on recent patents = currently active engineers in that domain
- Company assignee = their current employer
- Co-inventors = their team members
- Patent filing date = when they were actively working on this problem

### 5.2 USPTO Patent Full-Text Database

```
patft.uspto.gov → Full-Text Search → Field: IN (inventor) → Search
```

**Example:**
```
IN/"Smith John" AND ABST/PCIe AND ISD/20220101->20241231
```

### 5.3 Patent X-Ray via Google

```
site:patents.google.com "PCIe" "CXL" "memory controller" inventor:"[NAME]"
site:patents.google.com "neural network accelerator" "ASIC" "machine learning" 2023 OR 2024
```

---

## Part 6: Social & Community Mining

### 6.1 Twitter / X (ML Research Community)

ML Twitter is an active community. Researchers announce papers, share ideas, and engage in technical debate — making them findable and warm.

**Search by topic:**
```
twitter.com/search?q="machine learning" "new paper" "arxiv" lang:en&src=typed_query&f=user
```

**Find researchers by keyword in bio:**
```
site:twitter.com "machine learning researcher" "PhD" "OpenAI" OR "DeepMind" OR "Anthropic"
site:twitter.com "ML engineer" "pytorch" "open to work" OR "looking for"
```

**Lists:** Many ML Twitter users maintain public lists of top researchers — these are curated candidate pools.

### 6.2 Hugging Face Community

Hugging Face has 500K+ model and dataset contributors with public profiles.

**Browse by contribution:**
```
huggingface.co/models?sort=downloads       # Most downloaded models — find top contributors
huggingface.co/datasets?sort=downloads     # Dataset authors
huggingface.co/spaces                      # App builders
```

**X-Ray:**
```
site:huggingface.co "machine learning engineer" "San Francisco" OR "Bay Area"
site:huggingface.co "research scientist" "LLM" OR "language model"
```

### 6.3 Discord & Slack Communities

Many niche technical communities are invite-only but have public member directories or searchable archives:

- **Eleuther AI Discord** — OSS LLM researchers
- **MLOps Community Slack** — ML platform/infra engineers
- **Hugging Face Discord** — Transformers contributors
- **LangChain Discord** — LLM application engineers
- **LAION Discord** — dataset and multimodal researchers

**Approach:** Join the community, participate authentically, identify active contributors by username, then cross-reference on GitHub/LinkedIn.

---

## Part 7: Full Workflow — End-to-End Example

**Scenario:** Hiring a Staff ML Engineer focused on LLM inference optimization at a Series B AI startup.

### Step 1 — Define the signal
LLM inference = vLLM, TensorRT-LLM, Triton, CUDA kernels, Flash Attention, speculative decoding, quantization (GPTQ, AWQ, INT8).

### Step 2 — GitHub contributor mining
```bash
# Pull vLLM contributors
curl "https://api.github.com/repos/vllm-project/vllm/contributors?per_page=100" | jq '.[].login'

# Pull Flash Attention contributors  
curl "https://api.github.com/repos/Dao-AILab/flash-attention/contributors?per_page=100" | jq '.[].login'
```
→ ~50–80 names with public GitHub profiles

### Step 3 — ArXiv paper search
```
arxiv.org/search/?searchtype=all&query=LLM+inference+optimization+speculative+decoding+2024
arxiv.org/search/?searchtype=all&query=flash+attention+efficient+transformer+2024
```
→ ~20–30 additional names with research background

### Step 4 — OpenReview mining
```
openreview.net/search?term=efficient+inference&group=ICLR.cc/2024
```
→ Cross-reference with Step 2 and 3 names; spotlight/oral paper authors = top priority

### Step 5 — LinkedIn X-Ray validation
```
site:linkedin.com/in ("LLM inference" OR "model serving" OR "vllm" OR "triton") ("staff engineer" OR "principal engineer") pytorch
```
→ Validate current role, tenure, location for names found above

### Step 6 — Email enrichment
- Run LinkedIn URLs through Prospeo/Snov.io
- Run names + companies through Hunter.io
- Check GitHub profiles for public email

### Step 7 — Outreach
By now you have 20–30 warm names with verified emails, GitHub profiles, and paper links. Your outreach references their specific work — the paper, the repo, the commit. Response rates on this kind of outreach are 3–5x higher than cold LinkedIn InMail.

---

## Appendix: Tool Stack Reference

| Tool | Use Case | Cost |
|---|---|---|
| Google X-Ray | Profile/resume mining across any indexed site | Free |
| GitHub API | Contributor lists at scale | Free (rate limited) |
| Semantic Scholar | Paper + author search with filtering | Free |
| ORCID | Researcher identity + employment | Free |
| ResearchGate | Researcher profiles + networks | Free |
| OpenReview | ICLR/NeurIPS paper + author search | Free |
| ACL Anthology | NLP paper + author search | Free |
| Google Patents | Patent inventor mining | Free |
| Hunter.io | Email finding by domain | Freemium |
| Snov.io / Prospeo | LinkedIn email extraction | Paid |
| People Data Labs | Person enrichment API | Paid |
| SeekOut | Unified sourcing with publication/patent filters | Paid |
| HireEZ | AI sourcing with diversity filters | Paid |

---

## Legal & Ethical Notes

- All methods here use **publicly available data** indexed by search engines or exposed via public APIs
- GitHub API: follow rate limits (60 req/hour unauthenticated, 5,000/hour authenticated)
- Resume mining: only contact people whose information is publicly posted
- Platform ToS: X-Ray search is legal — you're querying Google, not scraping the platform directly
- GDPR: for candidates in EU/UK, ensure outreach complies with legitimate interest basis
- Robots.txt: direct scraping (not covered here) must respect each site's robots.txt

---

*Part of the [recruiting-portfolio](https://github.com/marvelchandra/recruiting-portfolio) by Chandra Buduri*
