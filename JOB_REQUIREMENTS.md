# Senior AI Infrastructure Architect — Job Requirements (2026-11)

Research window: **2026-08-14 → 2026-11-12** (90 days). Sample: **35 postings** across **30 employers** (FAANG, hyperscaler, Fortune 500 FS, healthcare, enterprise consulting, federal, AI-native). Raw records: [`.aicg/job-requirements.json`](.aicg/job-requirements.json).

## Executive summary

The 2026-H2 market for Senior AI Infrastructure Architect / Principal / Chief AI Architect / VP AI Platform roles is **structurally unchanged** relative to the shape of the existing curriculum:

- The dominant postings still cluster around enterprise AI strategy, executive/board communication, enterprise architecture governance, responsible-AI regulatory programs, global/sovereign deployment, and strategic partnerships — all covered by MOD-401…MOD-410.
- What is new in 2026 (MCP gateways, agentic runtime stacks, CAIO operating models, sovereign-AI deployment patterns) resolves at this level into **strategy / standards / governance** work that the existing modules already frame; the technical patterns themselves belong to lower-level roles (Level 45 Architect, Level 50 Principal Engineer, Level 30 ML Platform / MLOps).

**Recommendation: zero net-new modules, zero net-new projects, zero net-new exercises for this cycle.** No requirement cleared the continuity-bias thresholds (≥3 distinct ≤90-day postings AND ≥0.30 frequency AND cannot be incrementally extended). See [`.aicg/curriculum-plan-delta.json`](.aicg/curriculum-plan-delta.json) — empty arrays.

## Requirement → curriculum mapping

Requirements are ordered by posting frequency. "Owner level" per the role hierarchy; higher-level roles link to the lowest level that owns primary coverage.

| # | Requirement | Freq | Owner | Primary coverage | Status |
|---|---|---:|---|---|---|
| 1 | Enterprise AI strategy, multi-year roadmaps, $50M+ investment cases | 0.80 | **senior-architect (L55)** | [MOD-401 Enterprise AI Strategy and Vision](lessons/mod-401-enterprise-ai-strategy/README.md) + [Project-401 AI Transformation Strategy](projects/project-401-ai-transformation-strategy/) | ✅ covered |
| 2 | AI governance, model risk management, ARB leadership, standards | 0.71 | **senior-architect (L55)** | [MOD-403 Enterprise Governance](lessons/mod-403-enterprise-governance/README.md) + [Project-406 Enterprise Governance Model](projects/project-406-enterprise-governance-model/) | ✅ covered |
| 3 | C-suite/board executive communication; influence CTOs, CIOs, CISOs, Directors | 0.65 | **senior-architect (L55)** | [MOD-402 Executive Leadership](lessons/mod-402-executive-leadership/README.md) | ✅ covered |
| 4 | Responsible AI, EU AI Act, NIST AI RMF, ISO 42001 regulatory programs | 0.49 | **senior-architect (L55)** | [MOD-405 Responsible AI](lessons/mod-405-responsible-ai/README.md) + [Project-403 Responsible AI Framework](projects/project-403-responsible-ai-framework/) | ✅ covered |
| 5 | Enterprise GenAI/Agentic reference architecture: AI gateways, MCP, model routing, agent runtime, control plane | 0.46 | architect (L45) | **Primary:** `ai-infra-architect-learning` (Level-45). **Senior-architect strategic framing:** [MOD-401](lessons/mod-401-enterprise-ai-strategy/) (portfolio positioning), [MOD-403](lessons/mod-403-enterprise-governance/) (standards/ARB), [MOD-405](lessons/mod-405-responsible-ai/) (guardrails) | ✅ owned at lower level, strategic layer covered |
| 6 | Global/multi-cloud architecture, data sovereignty, sovereign AI deployment | 0.43 | **senior-architect (L55)** | [MOD-406 Global Infrastructure](lessons/mod-406-global-infrastructure/README.md) + [Project-402 Global AI Platform Architecture](projects/project-402-global-ai-platform-architecture/) | ✅ covered |
| 7 | LLMOps, LLM observability, prompt management, eval frameworks | 0.40 | ml-platform (L30) | **Primary:** `ai-infra-ml-platform-learning`. **Senior-architect framing:** standards-setting via MOD-403 | ✅ owned at lower level |
| 8 | Strategic partnerships and multi-vendor AI platform management (ChatGPT Enterprise, Claude Enterprise, hyperscaler AI surfaces) | 0.37 | **senior-architect (L55)** | [MOD-407 Strategic Partnerships](lessons/mod-407-strategic-partnerships/README.md) | ✅ covered |
| 9 | AI FinOps, token economics, GPU TCO modeling | 0.34 | architect (L45) | **Primary:** `ai-infra-architect-learning`. **Senior-architect strategic layer** (build-vs-buy TCO at the portfolio level): already in [MOD-401](lessons/mod-401-enterprise-ai-strategy/) | ✅ owned at lower level |
| 10 | AI-specific security controls (guardrails, workload identity, policy-as-code, sandboxing) | 0.31 | architect (L45) | **Primary:** `ai-infra-architect-learning`. **Senior-architect framing:** standards through [MOD-403](lessons/mod-403-enterprise-governance/) and [MOD-405](lessons/mod-405-responsible-ai/) | ✅ owned at lower level |
| 11 | CAIO/Chief AI Architect operating models and decision rights | 0.29 | **senior-architect (L55)** | [MOD-402 Executive Leadership](lessons/mod-402-executive-leadership/README.md) + [MOD-403 Enterprise Governance](lessons/mod-403-enterprise-governance/README.md) | ✅ covered (below 0.30 threshold anyway) |
| 12 | Innovation program leadership; emerging tech (quantum, agentic, physical AI) | 0.26 | **senior-architect (L55)** | [MOD-404 Innovation & R&D](lessons/mod-404-innovation-rd/README.md) + [Project-404 Innovation Program Design](projects/project-404-innovation-program-design/) | ✅ covered |
| 13 | Future-of-AI strategy (post-GenAI, physical AI, AGI readiness) | 0.23 | **senior-architect (L55)** | [MOD-410 Future of AI Infrastructure](lessons/mod-410-future-of-ai-infra/README.md) | ✅ covered |
| 14 | GPU cluster design, NCCL/InfiniBand fabrics, distributed-training collectives | 0.20 | performance/principal-engineer (L35/L50) | **Primary:** `ai-infra-performance-learning` + `ai-infra-principal-engineer-learning`. Senior-architect view: vendor/portfolio strategy in [MOD-407](lessons/mod-407-strategic-partnerships/) | ✅ owned at lower level |
| 15 | Thought leadership, standards contribution, industry influence | 0.17 | **senior-architect (L55)** | [MOD-409 Thought Leadership](lessons/mod-409-thought-leadership/README.md) + [Project-405 Industry Thought Leadership](projects/project-405-industry-thought-leadership/) | ✅ covered |
| 16 | M&A technical due diligence and post-merger AI integration | 0.14 | **senior-architect (L55)** | [MOD-408 M&A Due Diligence](lessons/mod-408-ma-due-diligence/README.md) | ✅ covered |

## Posting evidence (abbreviated)

Full normalized records live in [`.aicg/job-requirements.json`](.aicg/job-requirements.json). Representative recent postings used to validate each dominant theme:

- **Enterprise AI strategy & roadmaps:** Zuora *VP of AI Platform*; Schonfeld *Head of AI Platform*; New York Life *CVP — Head of Enterprise AI Platform*; Priceline *Principal Enterprise Architect, AI Platform*; Medline *Head of Data & AI Platforms*; Bullish Group *Head of AI Platform & Enablement*.
- **Governance / ARB / model risk:** BMO *Principal Architect AI Platform* (2026-11-10, Chicago); Vuori *Principal AI Architect & Governance*; Sedgwick *Principal Architect — AI*; HealthEquity *AI Governance and Controls Architect*; Salesforce *Principal/Distinguished Applied AI Architect — FS Regulated*; Charles Schwab *Senior Manager, Model Risk Oversight — AI*; Citi *Senior AI Engineer — Wholesale Credit Risk (SVP)*.
- **Executive/board communication:** OpenAI *Manager, Applied AI Architects*; Aimpoint Digital *Lead AI Security Architect 2026*; NVIDIA *AI Infrastructure Global Architect*; Verizon *Principal Engineer — AI Platform Architect*.
- **Responsible AI / regulatory:** Vuori; Rush University Medical Center; Beth Israel Lahey Health; HealthEquity; Sedgwick.
- **GenAI/Agentic reference arch (owned at L45 Architect):** Wells Fargo *Principal Architect — GenAI and Agentic AI*; Verizon *5-layer stack*; BMO; Capgemini *Principal AI Enterprise Architect*; Huron *Senior AI Infrastructure Architect*; HMG Technology *AI Architect (LLMs | MCP | Text-to-SQL)*.
- **Global / sovereign AI / data residency:** NTT DATA *Senior Principal AI Infrastructure Architect* (Dublin); NTT DATA *AI Architect Sr. Advisor*; Oracle *AI Infrastructure Architect*; NVIDIA *AI Infrastructure Global Architect*; Microsoft *Senior Cloud & AI Infrastructure CSA (CTJ — Poly)*.
- **Strategic partnerships / multi-vendor:** Aimpoint Digital *Director of AI Platforms and Infrastructure* (ChatGPT Enterprise + Claude Enterprise ownership); Accenture *AI Infrastructure Architect*.
- **CAIO / decision rights:** Scotiabank *Chief AI Architect*; the Fortune-500 CAIO trend (76% of CEOs hiring one per Kanungo / Fortune 500 tracker; 54 F500 firms with enterprise-wide CAIO as of Sep 2026 per Rework).

## Why no additions this cycle

Per continuity-bias rules the bar for new content is: ≥3 distinct ≤90-day postings AND ≥0.30 frequency AND no existing module/exercise can be incrementally extended. Every requirement at or above 0.30 either (a) is already owned by an existing senior-architect module, or (b) is owned by a lower-level role per the hierarchy — in which case this repo links to that owner rather than duplicating.

Candidate gaps considered and rejected:

- **"5-layer enterprise agentic stack reference architecture" (Verizon-style)** — detailed reference architecture is a Level-45 Architect responsibility. At senior-architect level it surfaces as portfolio strategy (already MOD-401) and ARB standards (already MOD-403). No net-new senior-architect content warranted.
- **CAIO operating model / decision rights** — 0.29 frequency (below threshold), and the content is cleanly covered by MOD-402 (C-level operating relationships) and MOD-403 (governance forums and decision rights).
- **EU AI Act 2026 enforcement specifics** — already in scope of MOD-405 and Project-403; the 2026 enforcement milestones update at the resource/case-study level, not as a curriculum change.
- **Sovereign AI deployment patterns (on-prem, air-gapped, VPC, hybrid)** — the senior-architect framing (regulatory drivers, regional strategy, vendor economics) is already in MOD-406 + Project-402; detailed deployment patterns belong at L45.

## External resources for out-of-scope depth

Learners who need the Level-45 or lower implementation depth should consult the sibling curricula:

- `ai-infra-architect-learning` — GenAI reference architecture, MCP/AI gateway patterns, LLM platform engineering
- `ai-infra-ml-platform-learning` — LLMOps, observability, model-gateway implementation
- `ai-infra-performance-learning` — GPU cluster design, distributed-training collectives, NCCL/InfiniBand
- `ai-infra-principal-engineer-learning` — deep platform-engineering authority
- `ai-infra-sre-learning` — AI reliability, incident response for AI systems

## Research methodology notes

- Postings were sourced via WebSearch across ZipRecruiter, Indeed, Dice, LinkedIn-indexed boards, company career pages, and specialist aggregators (freehire.me, virtualvocations, zapply.jobs, aiengineerjobs).
- For postings where the full job description could not be retrieved via WebFetch (e.g. HTTP 403 from gated aggregators, closed roles), responsibilities were captured from the public search snippet and employer-titled role description only. These are tagged by the absence of a verbatim quote in the raw JSON.
- No posting was double-counted across employers; two postings from the same employer are listed only when the roles are materially distinct (e.g. Aimpoint Digital's Director of AI Platforms vs. Lead AI Security Architect).

## Change log

- **2026-11-12** — initial research packet. Zero proposed additions.
