# AWS Leadership Principles — STAR Format Responses
### Patrick Diamitani | Candidate: AWS Solutions Architect, Startups

---

## 1. CUSTOMER OBSESSION

**Principle:** Leaders start with the customer and work backwards. They work vigorously to earn and keep customer trust.

**SITUATION:**  
Our sales reps needed a customized pre-call brief to review before every client meeting. They already had access to raw datapoints—web activity, HubSpot engagement, past meeting notes—but that data lived in silos and required manual digging. What they actually needed was synthesized insight, not another dashboard of numbers.

**TASK:**  
I was asked to build a workflow automation that combined company and prospect research, lead intelligence, and HubSpot activity signals into a single, actionable brief for reps ahead of every call.

**ACTION:**  
I mapped every data source: HubSpot contact/company activity, prior meeting history, Factors.ai intent data, and our product catalog. Built an n8n workflow that pulled scheduled meetings daily and enriched each with contact/company-level data. Engineered the AI node prompt to move beyond surface-level summaries—training it to map page view spikes to relevant Atlas products.

**RESULT:**  
Auto-generates a 5-bullet action brief for every prospect/MQL, mapped to relevant products. Embedded on every HubSpot contact record—reducing manual research time reps previously spent per call.

---

## 2. OWNERSHIP

**Principle:** Leaders are owners. They think long term and act on behalf of the entire company.

**SITUATION:**  
RevOps receives lead lists with mismatched headers, inconsistent casing, and invalid data that slow down imports or create bad HubSpot records.

**TASK:**  
Solve at the system level—make any lead list format and import automatically with no manual cleanup.

**ACTION:**  
Built a Claude Coworkers skill that handles file uploads with specific formatting instructions. Validates headers, standardizes casing, removes duplicates, maps fields to HubSpot schema, and returns a clean file ready for import.

**RESULT:**  
Now the team drops any CSV into the tool and gets back a validated, formatted file in seconds. Removes human error and ensures standardized structure—keeping HubSpot clean.

---

## 3. INVENT AND SIMPLIFY

**Principle:** Leaders expect innovation and always find ways to simplify.

**SITUATION:**  
Manual prospecting doesn't scale and creates uneven coverage across reps.

**TASK:**  
Build an end-to-end system sourcing leads, enriching/scoring them, generating personalized outreach, and delivering to reps' tools—automatically on a schedule.

**ACTION:**  
Full-stack pipeline: SerpAPI for lead lists → Clay for data enrichment (cleaning, contact finding, fit scoring) → Custom Claude Coworkers AI agent generating 3–5 message variations per lead → Amplemarket for sequencing/deliverability → Calendly integration for booked meetings.

**RESULT:**  
Pipeline runs every morning at 7am with zero manual input. Reps start their day with enriched leads and pre-written sequences—focusing on conversations instead of list building.

---

## 4. LEARN & BE CURIOUS

**Principle:** Leaders are never done learning and always seek to improve themselves.

**SITUATION:**  
Staying current with AI requires daily ingestion—not weekly newsletters.

**TASK:**  
Create an automated system curating and synthesizing the most significant AI/ML developments daily.

**ACTION:**  
Built an automated news aggregation using n8n. Pulls fresh AI/ML and tech stories from Reddit, Hacker News, newsletters, and RSS feeds. Claude Coworkers skill analyzes each for novelty and relevance, generates a structured digest, surfaces top 5 with synthesized explanations.

**RESULT:**  
Generated "LiveBuildAI" LinkedIn newsletter scaling to 992+ subscribers and producing inbound inquiries for consulting and product development.

---

## 5. INSIST ON THE HIGHEST STANDARDS

**Principle:** Leaders have relentlessly high standards and continually raise the bar.

**SITUATION:**  
Single-model prompts for all tasks introduce unnecessary error and cost. Different tasks need different minds—planning vs. writing vs. debugging.

**TASK:**  
Design a framework routing tasks to optimal LLMs by phase, with benchmarks validating the decision logic.

**ACTION:**  
Built ROSTR Framework—classifies tasks by 5D Phase (PreD, Design, Dev, Deploy, Debug) and routes to best-fit model via PAL compilation layer. PreD research → DeepSeek; UI prototyping → Claude. Benchmarked 20 real tasks:

| Category        | Baseline | ROSTR  | Improvement |
|-----------------|----------|--------|-------------|
| Task Completion | 64.7%    | 79.9%  | +15.2 pp    |
| Code Quality    | 70.6%    | 79.4%  | +8.8 pp     |
| Coherence       | 65.3%    | 82.4%  | +19.7 pp    |
| Creativity      | 56.3%    | 67.3%  | +11.0 pp    |
| Overall         | 64.2%    | 77.2%  | +13.0 pp    |

**RESULT:**  
ROSTR demonstrated materially improved output quality. Published with Zenodo DOI (citable) as foundation for all builds.

---

## 6. BIAS FOR ACTION

**Principle:** Leaders know speed matters. Many decisions are reversible—value calculated risk-taking.

**SITUATION:**  
n8n instance runs dozens of workflows with no centralized health tracking. Silent failures could stall lead routing or HubSpot syncs for days.

**TASK:**  
Ship lightweight monitoring auditing all daily executions, surfacing failures with root-cause tagging, pushing reports to VP of Growth—fast.

**ACTION:**  
Skipped "right" architecture. Built Claude Coworkers skill (n8n-execution-analyst) querying n8n Postgres directly, pulling execution records, flagging unfinished runs, categorizing root causes, generating markdown reports, emailing via SMTP to VP.

**RESULT:**  
Daily audit surfaces failures within 24 hours. Caught and repaired 8 unknown workflow issues in first month—preventing lead routing delays, sync failures, downstream pipeline impact. VP starts every day with visible proof of system health.

---

## CONTACT

**Patrick Diamitani**  
📧 patrick.diamitani@gmail.com  
📱 319.930.0290  
🔗 linkedin.com/in/Diamitani
