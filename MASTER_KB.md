# Patrick Diamitani — Master Knowledge Base

> Auto-generated from all source files, resumes, portfolios, skills, and session history.
> Last updated: July 15, 2026

---

## Table of Contents

1. [Bio & Summary](#1-bio--summary)
2. [Professional Experience](#2-professional-experience)
3. [Enterprise Production Work (Atlas HXM)](#3-enterprise-production-work-atlas-hxm)
4. [Agent Skills & Library (30+)](#4-agent-skills--library-30)
5. [Products & Ventures](#5-products--ventures)
6. [Published Papers & Research](#6-published-papers--research)
7. [Precinct Captain Work (Your48)](#7-precinct-captain-work-your48)
8. [Education & Certifications](#8-education--certifications)
9. [Technical Skills Matrix](#9-technical-skills-matrix)
10. [Impact Metrics](#10-impact-metrics)
11. [Contact & Links](#11-contact--links)

---

## 1. Bio & Summary

**Patrick Diamitani**
Chicago, IL · Open to relocation
872.240.2830 · Patrick.Diamitani@gmail.com
[linkedin.com/in/Diamitani](https://linkedin.com/in/Diamitani) · [diamitani.me](https://www.diamitani.me) · [gptpat.co](https://www.gptpat.co)

**Target roles:** Forward Deployed Engineer · GTM / Applied AI Engineer · AI Solutions Engineer
(Google, Meta, OpenAI, Anthropic, Palantir-style)

Production AI systems builder who embeds with GTM and revenue teams, turns messy business rules into reliable workflows, and ships LLM + deterministic systems that operators actually use. Currently lead AI & Automation for a 50+ person GTM org at Atlas HXM: 8+ production automations live, ~242 pipeline deals auto-screened with auditable verdicts, and a post-sales AI pipeline recovered from 84% failure to stable end-to-end delivery. Combines enterprise sales DNA (Uber, Upwork, Techstars) with hands-on engineering (n8n, Azure OpenAI, HubSpot/Clay APIs, Claude Agent SDK, JavaScript rules engines, AWS).

---

## 2. Professional Experience

### Atlas HXM · GTM AI & Automation Manager
*Chicago, IL · 2025 – Present*

AI & Automation lead for a 50+ person GTM organization at a global Employer-of-Record (EOR) platform. Own production AI systems across sales, partnerships, compliance, and enablement — from problem framing with VP Growth through architecture, build, reliability, and operator adoption.

### GPTPAT · AI Engineer & Founder
*2024 – Present*

Build and deploy production AI solutions for SMB and mid-market clients — chatbots, workflow automation, and full-stack web apps grounded in client data.

### Scalytics.io · GTM Engineer (Consulting)
*Apr 2025 – Present (part-time)*

GTM systems for private-AI / federated-data startup — ICP, outbound tooling, Make.com ↔ Zoho/HubSpot automations, custom CRM tooling with founding PhDs.

### RevEnabled · Founder · Sales Systems & GTM Consulting
*Apr 2023 – Dec 2024*

Revenue operations and GTM systems consulting — CRM setup, outbound infrastructure, playbooks, and automation.

### Uber · Enterprise BDR (Uber for Business)
*Aug 2022 – Jan 2023*

$947K+ gross bookings; 2,000+ emails / 250 dials/week to C-suite/VP; led hiring cohort in quota.

### Upwork · Senior Enterprise BDR
*Oct 2019 – Dec 2021*

Top 10% quota performance on 60+ team; #1 connection rate (100+ dials/day); Fortune 500 strategic use cases.

### Earlier Roles

- **Techstars Chicago · Portfolio Associate — Sales (2018):** Sales infra for 2ndKitchen (acquired), Clyde (acquired), Rheaply ($40M).
- **DreamItReel · Founding Account Executive (2016–2018):** $2M+ revenue, 40% YoY; team of 5.
- **Omicon Entertainment · Founding Partner:** 150+ events, 80K+ attendees, $3M+ revenue.

---

## 3. Enterprise Production Work (Atlas HXM)

### 01 — EOR Compliance Checker (v5)
**Flagship · Live in Production**

Auto-screens every sales-pipeline deal against a 30-sector compliance worksheet.

- **46-node n8n production workflow** (real-time webhook + hourly safety-net sweep + on-demand batch re-screen)
- **Hybrid engine**: LLM maps messy CRM text to 30 canonical sectors; deterministic JS matrix issues verdicts
- **Three-axis compliance framework** (viability tier + advisory flags + hard screen-outs)
- **Dry-run harness** tests any future rule change against entire pipeline with zero writes
- **Live across ~242 open deals**; corrected 103 mis-tagged deals; 16 unit tests; 238/238 clean writes before go-live

### 02 — Post-Sales Call Automation
**Live · Major Reliability Turnaround**

After every sales call, auto-generates rep-ready follow-up package: consultative email, missed-questions analysis, competitor research, LinkedIn draft, CRM note.

- Recovered from 21/25 failing → stable end-to-end
- Replaced dead Azure AI Search with deterministic Blob lookups across 250+ country files
- Cut context from 882KB → 295KB per call with higher groundedness
- Four AI agents grounded in real country data

### 03 — Pre-Sales Call Automation
**Built · Requested by VP Growth**

Sends reps concise pre-call prep note the moment a meeting is booked. Uses event trigger (not scheduled sweep) to defeat time-zone failure. Enriches from Factors.ai Journey API + HubSpot.

### 04 — Chatbot MQL Automation + Attribution
**Live · Recovered a Whole Channel**

AI classifies website chat → MQL vs. non-MQL → routes follow-up → stamps attribution. Recovered 364 historical contacts into reporting. Idempotency checkpoint prevents double-processing.

### 05 — Partner PQL Workflow
**Deploy-Ready**

Classifies inbound partner-form submissions, drafts partner-specific email, routes to partnerships owner. Fixed HubSpot v3-API association bug (id vs. vid).

### 06 — Entity Readiness Change Report
**Build-Ready · Approval-Gated**

Weekly diff of country hire-readiness. Only reports countries that flipped — locked two-column table. Baseline writes gated behind successful non-empty pulls.

### 07 — SDR-Agency Prospecting Enablement (AGS)
**Ongoing · Owns the Pipeline**

Full prospecting supply chain: intake → normalize → dedupe → enrich → suppress → activate. 5,398-contact master with CRM-safe screening. Competitive-takeaway play: 188 verified HR contacts.

### 08 — Outbound Signals & Intent Engine
**Strategy + Build**

Eight signal categories (expansion, funding, hiring, leadership, competitor/tech, compliance, first-party engagement, suppression), each weighted and mapped to data source, persona, and query logic. 0–100 account scoring model.

### 09 — Clay Credit Governance & Cost Control
**Shipped · Cost + Governance Win**

Traced 515K credit spike to root cause. Full-year forensic audit (seven-sheet master dataset). Standard Enrichment Table Template with ICP-fit gate. Three build profiles replacing undisciplined ~50-credit average.

### 10 — New Project Automation System (Center of Excellence)
**Meta-System · Framework**

Turns raw input → complete project package: knowledge base, PRD, architecture diagram, reporting framework, phased build plan. Idea → fully-scoped project: 4–8 hrs → <30 min.

### 11 — GTM Skill & Agent Library (30+)
**Platform · Built for 50+ Reps**

Reusable AI skills and agents for non-technical reps via plain-English commands:
- **Prospecting & enrichment**: Clay engine, credit estimator, CSV enrichers, HubSpot import formatter, list routers
- **Workflow & ops**: n8n workflow architect, execution analyst, GTM architect, project intake & handoff
- **Revenue & enablement**: HubSpot data/revenue analysts, RFP knowledge-base builder, Factors.ai signal operator, case-study builder
- **Content at scale**: Full branded content suite + agent-factory

---

## 4. Agent Skills & Library (30+)

### Prospecting & Enrichment
| Skill | Function |
|-------|----------|
| `clay-prospecting-engine` | Build and execute Clay prospecting tables |
| `clay-credit-estimator` | Estimate credit usage before enrichment runs |
| `clay-csv-enricher` | Enrich CSV lists via Clay API |
| `hubspot-data-analyst` | Analyze HubSpot CRM data, pipelines, revenue |
| `hubspot-import-formatter` | Format CSVs for HubSpot imports |

### Workflow & Operations
| Skill | Function |
|-------|----------|
| `n8n-engineer` | Build, debug, and deploy n8n workflows |
| `n8n-workflow-architect` | Design workflow architecture from requirements |
| `n8n-execution-analyst` | Analyze n8n execution failures and errors |
| `n8n-csv-router` | Route CSV data through n8n workflows |
| `gtm-architect` | Design GTM systems and automation architecture |
| `saas-architect` | Architecture design for SaaS platforms |
| `dashboard-builder` | Build dashboards and reporting interfaces |
| `workflow-builder` | General workflow construction |

### Project Management
| Skill | Function |
|-------|----------|
| `new-project-system` | Intake engine: idea → full project package |
| `project-instructions-builder` | Build project briefs and instructions |
| `project-closeout-report` | Generate project closeout documentation |
| `project-handoff` | Handoff projects between teams/agents |
| `context-engine` | Maintain project context across sessions |
| `file-organizer` | Organize project files and directories |

### Atlas-Specific
| Skill | Function |
|-------|----------|
| `atlas-proposal-builder` | Build Atlas proposals and decks |
| `atlas-use-case-builder` | Generate use cases from industry/scenario |
| `atlas-agent-factory` | Build new Atlas agents from descriptions |
| `atlas-gtm-insider` | Atlas GTM domain knowledge and context |
| `atlas-video-studio` | Video production for Atlas content |
| `atlas-video-hyperframes` | HyperFrames video generation |
| `atlas-video-render` | Render Atlas video projects |
| `atlas-prospect-video-builder` | Build prospect-specific videos |

### Content & Enablement
| Skill | Function |
|-------|----------|
| `case-study-builder` | Build case studies from project data |
| `jtbd-builder` | Jobs-to-be-Done framework construction |
| `prompt-rewriter` | Optimize and rewrite prompts |
| `token-spend-analyst` | Analyze AI token spending |
| `pal` | Prompt Abstraction Layer compiler |

### Productivity
| Skill | Function |
|-------|----------|
| `exec-assistant` | Executive assistant workflows |
| `asana-organizer` | Asana task management |
| `daily-session-recap` | End-of-day session summaries |
| `video-editor` | Video editing workflows |
| `rostr-builder` | ROSTR framework implementation |

---

## 5. Products & Ventures

### GPTPAT (gptpat.co)
Production AI solutions for SMB and mid-market:
- **Coach Angie Chatbot** — Recruiting agency chatbot (Voiceflow + OpenAI)
- **Email Automation Platform** — CSV-driven outreach (Make.com, v0, Vercel, Supabase)
- **Yo Hablo** — Ed-tech web app (v0, Vercel, Gemini API, TTS)
- YouTube moderation automation, blog rewriter (RSS + LLM), Shopify workflows

### RevEnabled (revenabled.com)
GTM systems consulting:
- **Dark Roast Media**: Outbound ops, 60K leads, 500 emails/day @ 40% open / 12% reply, $1M → $3M ARR
- **Rand McNally (Rand Fleet)**: 2,000% engagement lift, 200K+ emails @ 50% open, ~$5M pipeline

### Scalytics.io
GTM engineer for private-AI / federated-data startup: ICP, outbound tooling, Make.com ↔ Zoho/HubSpot automations.

### Your48 (your48.vercel.app)
Civic intelligence platform for Chicago's 48th Ward:
- Precinct directory with interactive map
- Business license database (1,500+ businesses)
- Constituent intake forms
- Ward dashboard

### Atlas HXM Agent Ecosystem
30+ Claude skills/agents deployed across 50+ person GTM org. Center of Excellence project system. ROSTR framework implementation.

---

## 6. Published Papers & Research

### ROSTR Framework
**"ROSTR: A Unified Architecture for Production-Grade Multi-Agent Systems with Phase-Aware Orchestration and Persistent Knowledge Compounding"**
Patrick Diamitani, April 2026

DOI: [10.5281/zenodo.19550414](https://doi.org/10.5281/zenodo.19550414)

Components:
- **PAL** (Prompt Abstraction Layer) — Intent Compiler: transforms loose NL into strict agent manifests
- **RAG DAL** (Dynamic Acquisition Layer) — Multi-pass retrieval with source credibility stratification
- **NPAO** (Navigate, Prioritize, Allocate, Orchestrate) — 5D phase taxonomy + 4D priority scoring
- **Rostr Hub** — Agent Operating System with persistent reference architecture

The paper formalizes the agentic framework used to build the Atlas HXM automation ecosystem.

---

## 7. Precinct Captain Work (Your48)

### Your48 V2.0 — Civic Intelligence Platform

**Role:** Precinct Captain, 48th Ward Chicago + Platform Architect/Builder

**What I built:**

Your48 is a civic intelligence platform for Chicago's 48th Ward (Edgewater, Uptown, Andersonville), serving Alderman Leni Manaa-Hoppenworth's office and constituents.

**V1.0 (Live at your48.vercel.app):**
- Civic homepage with ward directory, city services, community resources
- Events calendar, newsletter integration (Mailchimp)
- AI chat widget for ward questions
- Mobile-first responsive design

**V2.0 (In development):**
- **Precinct Directory**: Interactive ward map with precinct boundaries, "Find My Precinct" address lookup, captain profiles with bio/photo/territory
- **Business License Database**: 1,500+ licensed businesses searchable by name, address, category, license status
- **Constituent Intake System**: Digital forms for service requests (potholes, graffiti, tree trimming) with photo upload and precinct auto-detection
- **Ward Dashboard**: Public metrics on service requests, business licenses, ward initiatives

**Tech Stack:**
- React 18 + Vite + TypeScript
- Tailwind CSS design system
- Mapbox GL JS (ward/precinct boundaries)
- Fuse.js (client-side search)
- Chicago Data Portal API (business licenses, 311)
- Airtable (forms + staff data)
- Vercel (deployment, free tier)

**Data managed:**
- ~1,562 business licenses (Chicago Data Portal)
- ~42 religious institutions
- ~27 CPS schools in the ward
- 39 precincts with captain contacts
- Community anchors and resources

**ROSTR Framework application:**
The ROSTR data sync pipeline handles daily business license ingestion from Chicago Data Portal, normalization, precinct tagging, and JSON generation — all running as Vercel cron jobs at $0 cost.

---

## 8. Education & Certifications

- **Per Scholas — AWS re/Start · Chicago, IL**
  - AWS Certified AI Practitioner (May–Jul 2025)
  - AWS Certified Cloud Practitioner (Dec 2024–Apr 2025)
  - Hands-on: VPC/EC2, Lambda/API Gateway, Bedrock/Polly/Lex, RDS/DynamoDB

- **St. John's University, Tobin College of Business · Queens, NY**
  - B.S. Economics (2009–2014)
  - Co-founded Entrepreneurial Society; Student Government ($1M budget); G.L.O.B.E. Microfinance Program

---

## 9. Technical Skills Matrix

### AI / LLM Systems
- Azure OpenAI (GPT-4o / GPT-5-chat)
- Claude + Claude Skills / Agent SDK
- OpenAI Assistants API & Custom GPTs
- Google Gemini
- AWS Bedrock
- Retrieval & grounding, prompt + eval harnesses
- Hybrid LLM + deterministic decision engines

### Orchestration & APIs
- n8n (production workflows, webhooks, idempotency, dry-run gates)
- Custom JavaScript rules engines
- MCP tool connectors
- REST APIs, Make.com, Zapier

### GTM Data Stack
- HubSpot API (CRM properties, workflows, attribution)
- Clay (+ credit governance)
- Amplemarket, ZoomInfo, Avoma, Factors.ai, Salesforce, Apollo.io

### Cloud & Delivery
- AWS (EC2, S3, IAM, Lambda, VPC, Bedrock)
- Azure Blob Storage
- Vercel, Supabase, Docker, Microsoft 365

### Languages & Web
- JavaScript / TypeScript
- Python
- React, Node.js
- SQL, HTML/CSS

---

## 10. Impact Metrics

| Metric | Result |
|--------|--------|
| Production GTM automations live | 8+ |
| Pipeline deals auto-screened (auditable) | ~242 |
| Post-sales AI reliability turnarond | 21/25 failing → stable E2E |
| Idea → scoped project package | 4–8 hrs → <30 min |
| Reusable GTM Claude skills/agents | 30+ |
| Enterprise bookings (Uber) | $947K+ |
| Consulting pipeline (Rand Fleet) | ~$5M |
| Clay credit spend spike governed | 515K traced to root cause |
| Historical chatbot contacts recovered | 364 |
| Ward precincts managed | 39 |
| Ward businesses catalogued | ~1,562 |
| SDR-agency contact master | 5,398 |

---

## 11. Contact & Links

- **Email:** Patrick.Diamitani@gmail.com
- **Phone:** 872.240.2830
- **LinkedIn:** [linkedin.com/in/Diamitani](https://linkedin.com/in/Diamitani)
- **Portfolio:** [diamitani.me](https://www.diamitani.me)
- **GPTPAT:** [gptpat.co](https://www.gptpat.co)
- **Civic:** [your48.vercel.app](https://your48.vercel.app)
- **ROSTR Paper:** [zenodo.org/records/19550414](https://zenodo.org/records/19550414)
- **Location:** Chicago, IL · Open to relocation

---

*This knowledge base is the single source of truth for Patrick Diamitani's professional history, projects, skills, and impact. Generated from all available source files, resumes, portfolios, and session history.*
