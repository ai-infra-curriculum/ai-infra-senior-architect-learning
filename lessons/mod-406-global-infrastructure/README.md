# MOD-406: Global AI Infrastructure and Scaling

**Level**: Senior Architect (Strategic / Executive)
**Duration**: 35-50 hours
**Prerequisites**: Architect-level experience; mod-401 (Enterprise AI Strategy); mod-403 (Enterprise Governance) and mod-405 (Responsible AI) recommended

## Module Overview

This module is part of the Senior AI Infrastructure Architect curriculum
(level 400). Focus: global AI infrastructure and scaling.

Senior-architect modules emphasize executive communication, strategic
thinking, and organizational influence — not hands-on implementation.
For hands-on technical material on related topics (multi-region
Kubernetes, inference autoscaling, data-replication topologies, edge
deployment, GPU scheduling, cross-region observability), see the
engineer-level and senior-engineer-level repos.

### Executive Summary

MOD-401 taught you to *build* a strategy, MOD-402 to *carry* it,
MOD-403 to *govern* what you ship, MOD-404 to produce the *next*
generation, and MOD-405 to decide what the organization is willing to
deploy at all. MOD-406 asks the question the others defer: *where does
it physically run, under whose law, with whose electrons, on whose
silicon, and what happens when that answer stops being available?*

At enterprise scale, AI infrastructure is no longer a procurement
decision made inside IT. It is a set of decisions that touch
foreign policy, trade controls, energy policy, labor law, and the
privacy rights of residents in every country the organization
operates in. A single training run can draw the attention of an
export-control regulator, a grid operator, a water authority, a data-
protection commissioner, and a sovereign-cloud sales team — often in
the same week. The senior architect's job is to make these decisions
deliberately, with the trade-offs documented, rather than discovering
them in the form of an enforcement letter.

At this level, global infrastructure is a program with five parts
that must co-exist: a **compute supply posture** (chips, clouds,
sovereign alternatives, and the contingency plan when the primary
supplier is blocked), a **data sovereignty and cross-border posture**
(where data lives, how it moves, under which lawful-transfer
mechanism, and which workloads can never leave a jurisdiction), a
**regional regulatory alignment** (EU AI Act, US federal and state
rules, China's generative-AI measures, UK, Brazil, India, and the
sector overlays), a **siting and operations model** (power, water,
grid, latency, workforce distribution, local presence), and a
**resilience and contingency regime** (dual-region, dual-cloud, dual-
silicon, dual-jurisdiction playbooks for scenarios that were
hypothetical in 2020 and are quarterly news now). A program with
four of the five works until the fifth is tested, and then it does
not.

By the end of this module, you will be able to:

- Produce a defensible global AI infrastructure architecture that a
  CFO, General Counsel, and Chief Risk Officer can each sign
- Map the organization's workloads to a residency and cross-border
  transfer regime that survives GDPR, Schrems-era challenges,
  sector overlays, and emerging data-localization laws
- Translate chip export controls, foundation-model licensing terms,
  and sovereign-cloud offerings into a build / partner / regionalize
  / decline decision for each major workload
- Design a multi-region operating model (latency, availability,
  cost, carbon, sovereignty) with explicit, documented trade-offs
- Lead the organization through a geopolitical infrastructure
  disruption — a sudden export-control change, a cross-border
  transfer suspension, a regional cloud outage, or a nation-state
  compute embargo
- Communicate global infrastructure posture to a board, to a
  government customer, and to a regulator with authority in every
  jurisdiction the organization operates in

---

## Learning Objectives

### The Global AI Infrastructure Map

1. **The hyperscaler regional topology**
   - AWS, Microsoft Azure, Google Cloud regional footprints,
     Availability Zone construction, and the difference between a
     "region" (sovereign-law anchor) and an "edge location"
     (performance anchor)
   - The second-tier and specialty providers — Oracle Cloud,
     IBM Cloud, CoreWeave, Lambda, Crusoe, and the GPU-specialist
     clouds — and when they are the correct choice over a
     hyperscaler
   - Regional sovereign clouds (Alibaba Cloud, Tencent Cloud, Huawei
     Cloud, Yandex Cloud, OVHcloud, Bleu / S3NS / Delos, G42 /
     Core42, Nutanix sovereign, STC Cloud) and the jurisdictions in
     which they are the *only* defensible default

2. **The content-delivery and inference-edge map**
   - Cloudflare, Akamai, Fastly, and the hyperscaler CDN overlays
     as inference-edge substrates, not just static-content caches
   - Latency geography — the TeleGeography submarine-cable map, the
     Equinix / Digital Realty interconnection map, and the
     50-ms-to-population isocurves that decide where inference
     endpoints actually need to live
   - Edge inference on operator networks (AWS Wavelength, Azure
     Private MEC, GCP Distributed Cloud) and when 5G-adjacent
     deployment is architecture vs. marketing

3. **The sovereign-cloud and gov-cloud overlay**
   - AWS GovCloud, Azure Government, Google Cloud Public Sector,
     Oracle Government Cloud and their import of US federal
     authorization tiers (FedRAMP High, IL5, IL6)
   - EU-sovereign and member-state sovereign offerings — France
     (SecNumCloud, Bleu, S3NS), Germany (Delos), Italy (Polo
     Strategico Nazionale), Spain (SARA), and the "immune from
     non-EU law" claim's actual legal content
   - UK, Canada, Australia sovereign posture and the Five Eyes
     adjacency
   - China, UAE, Saudi Arabia, India, Brazil sovereign-AI programs
     as distinct categories, each with distinct access conditions

### Compute Supply Chain and Chip Geopolitics

4. **The silicon supply chain**
   - Design (NVIDIA, AMD, Intel, Apple, Google TPU, AWS Trainium,
     Cerebras, Graphcore, Groq, SambaNova) vs. fabrication (TSMC,
     Samsung, Intel Foundry, SMIC) vs. advanced packaging (CoWoS,
     HBM assembly) vs. lithography (ASML EUV monopoly)
   - Choke-point geography: Taiwan concentration in advanced nodes,
     Netherlands concentration in EUV, South Korea concentration
     in HBM, and the United States as the regulatory choke point
     via the Entity List and Foreign Direct Product Rule
   - HBM supply (SK Hynix, Samsung, Micron) as the actual
     bottleneck for current-generation accelerators, not GPU die
     fabrication alone

5. **US and allied export controls**
   - Bureau of Industry and Security (BIS) AI compute controls —
     performance-threshold and interconnect-bandwidth metrics,
     Entity List designations, Validated End User framework,
     and the evolving advanced-computing / AI-chips rule structure
     (the Biden-era AI Diffusion Rule was formally rescinded in
     November 2026 and the control regime continues to be revised
     through interim final rules)
   - Extraterritorial reach via the Foreign Direct Product Rule —
     why a non-US foundry still cannot ship to a listed party if
     US design IP or US-origin tools are involved
   - Allied coordination — Japan and the Netherlands joining US
     controls on advanced-node equipment, and the gap between what
     is coordinated and what is unilateral
   - Covered-nation and country-group taxonomies, and what
     "destination-neutral" controls (performance thresholds that
     apply everywhere) mean for a globally deployed enterprise

6. **The deployer's compute options under constraint**
   - Reserved capacity with a hyperscaler vs. long-term cluster
     leases from a GPU-specialist cloud vs. self-operated colo
     with purchased silicon
   - The multi-year foundation-model-vendor compute commitment as
     a de facto supply-chain play (hyperscaler ↔ model-lab equity
     and compute-credit arrangements — Microsoft-OpenAI,
     Amazon-Anthropic, Google-Anthropic, Oracle-OpenAI and
     successor deals, publicly disclosed in the tens-to-hundreds
     of billions of dollars range)
   - Sovereign compute programs (France INRIA / Jean Zay, UK Isambard-AI
     and AI Research Resource, EuroHPC JUPITER / LUMI / Leonardo,
     US NAIRR, Japan ABCI, UAE Falcon / G42, India AI Mission
     compute) as subsidized access under conditions
   - The "build the fab" option (TSMC Arizona, Samsung Texas,
     Intel Ohio, TSMC Dresden, Rapidus Hokkaido) as a 2030-horizon
     bet, not a 2026-horizon supply fix — Intel Ohio has slipped
     to 2030, Samsung Taylor to 2028, and TSMC's second Arizona
     fab deferred past its original target

### Data Sovereignty and Cross-Border Flows

7. **Residency, localization, and sovereignty as distinct claims**
   - *Residency* (data physically stored in a jurisdiction) vs.
     *localization* (data stored, processed, *and* operated under
     that jurisdiction's personnel and tooling) vs. *sovereignty*
     (immune to foreign legal process such as US CLOUD Act or
     Chinese national-security data demands)
   - Why "data stays in-region" is a necessary but not sufficient
     claim; the supporting evidence is personnel location,
     administrative access, key management, and legal opinion
   - The sovereign-cloud offer's actual legal content: who answers
     a subpoena, who holds the keys, who can run an operator
     script after hours

8. **GDPR, Schrems, and the EU transfer regime**
   - GDPR Chapter V transfer mechanisms — adequacy decisions
     (including the EU-US Data Privacy Framework, in force but
     under pending CJEU challenge), Standard Contractual Clauses,
     Binding Corporate Rules, derogations — and their
     post-*Schrems II* evidence burden under EDPB Recommendations
     01/2020 on supplementary measures
   - The Data Protection Impact Assessment (DPIA) and Transfer
     Impact Assessment (TIA) as the enterprise-level residency
     audit artifacts
   - Interaction with the EU AI Act (Regulation (EU) 2024/1689) —
     training-data lawfulness, high-risk-system data governance
     (Article 10), and cross-system data-flow implications

9. **Non-EU data regimes that constrain training and inference**
   - UK Data Protection Act and UK GDPR, and the divergence watch
   - China's Personal Information Protection Law (PIPL), Data
     Security Law, Cybersecurity Law, and the CAC's
     generative-AI-specific *Interim Measures for the Management
     of Generative Artificial Intelligence Services* (effective
     15 August 2023), with filing and security-assessment
     obligations for public-facing services
   - India's Digital Personal Data Protection Act (2023) and its
     implementing Rules (notified November 2025, substantive
     obligations phasing in through 2027), Brazil's LGPD, South
     Korea's PIPA, Japan's APPI, Australia's Privacy Act reform,
     and the India / Russia / Vietnam / Indonesia data-localization
     overlays
   - US sectoral rules that dominate residency even without a
     federal privacy law — HIPAA for health, GLBA for finance,
     FERPA for education, ITAR / EAR for defense and dual-use
   - Executive-order and state-level overlays that affect AI
     data flows: US Executive Order on bulk data to countries
     of concern, California CCPA/CPRA, Colorado AI Act (as
     revised by SB 189), Texas TRAIGA, New York Local Law 144,
     Illinois BIPA — a fast-moving layer that must be refreshed
     before any cross-jurisdictional architecture decision

10. **The output-side residency problem**
    - Membership-inference, training-data extraction, and the
      possibility that a model deployed in-region exposes data
      trained out-of-region — residency of *weights* vs. residency
      of *training corpus*
    - Model-weight residency and the growing practice of
      weight-locking to a region as an infrastructure control
    - RAG, embeddings, and vector-store residency — where the
      hidden data flows actually occur
    - Logs, prompts, and user-reply retention as the most-missed
      residency surface

### The Regional Regulatory Landscape

11. **The EU AI Act as the global template**
    - Scope, extraterritorial reach ("placing on the market in the
      Union," "output used in the Union"), and the role mapping
      (provider, deployer, importer, distributor, authorised
      representative)
    - Prohibited practices (Article 5), high-risk systems (Annex III
      and sectoral), general-purpose AI model obligations
      (Articles 51-55), transparency obligations (Article 50),
      Fundamental Rights Impact Assessment
    - Application-date table — prohibitions (from 2 February 2025),
      GPAI obligations (from 2 August 2025), general applicability
      (2 August 2026), and high-risk timelines (Annex III high-risk
      deferred to 2 December 2027 under the Digital Omnibus on AI)
      as the planning calendar for compliance investment
    - Codes of Practice, harmonised standards, and the AI Office /
      AI Board governance stack
    - Fines — percentage-of-global-turnover tiers, which must be
      framed to a board in actual-dollar terms

12. **US, UK, and allied frameworks**
    - US federal: NIST AI RMF 1.0 and the Generative AI Profile
      (NIST AI 600-1), OMB M-25-21 (agency AI use, rescinding and
      replacing M-24-10) and M-25-22 (AI acquisition), sector
      regulators (FTC, SEC, CFPB, EEOC, HHS, FDA) and their
      enforcement posture
    - US state activity: Texas TRAIGA (effective January 2026),
      Colorado AI Act as revised by SB 189 (effective January 2027),
      California SB 53 and AB 2013 (effective January 2026) and
      the broader CAITA series, Utah AI amendments, Illinois, New
      York — a 50-state map that materially shifts each quarter
    - UK pro-innovation framework, the AI Safety Institute, and
      the regulator-led sectoral approach
    - Canada's proposed AIDA (Bill C-27, lapsed on prorogation in
      January 2025, with the "AI for All" strategy launched in its
      place), Australia AI safety standards (with a comprehensive
      AI Act anticipated from 2027), Singapore Model AI Governance
      Framework and AI Verify, Japan AI Promotion and Guidelines,
      South Korea AI Basic Act (effective 22 January 2026)

13. **China and jurisdictions with structurally different regimes**
    - CAC *Interim Measures for the Management of Generative
      Artificial Intelligence Services*, deep-synthesis provisions,
      algorithmic recommendation rules, and filing requirements
    - PIPL cross-border transfer regime — Standard Contract,
      Security Assessment, Certification — and the *de facto*
      data-localization effect
    - MLPS 2.0 (Multi-Level Protection Scheme), CII (Critical
      Information Infrastructure) designation, and their collision
      with multinational-vendor normal operations
    - Indonesia, Vietnam, Russia, Nigeria, Saudi Arabia, UAE
      localization patterns — each with its own enforcement
      flavor and acceptable mitigations

14. **International standards as the shared vocabulary**
    - ISO/IEC 42001:2023 (AI management system), ISO/IEC 23894:2023
      (AI risk management), ISO/IEC 5338:2023 (AI lifecycle),
      ISO/IEC 42005:2025 (AI impact assessment), and the
      ISO/IEC 5259 series (data quality for AI, with parts
      published on a rolling basis)
    - Interaction with the EU AI Act's harmonised-standards
      pathway (CEN-CENELEC JTC 21) and the US accreditation
      ecosystem
    - Why a global organization is operating at least three
      control-framework translations at once — AI Act, NIST AI
      RMF, and ISO/IEC 42001 as the usual trio

### Siting, Power, and Grid Constraints

15. **Energy, water, and grid as first-class design constraints**
    - Training-cluster site selection — power availability on the
      1-GW-to-1-TWh/year envelope, interconnection queue timelines,
      and power-purchase-agreement (PPA) design, against IEA
      projections that global data-center electricity demand will
      roughly double by 2030 with AI driving the majority of the
      increase
    - Water for evaporative cooling — the hot-humid/hot-dry
      trade-off, closed-loop and air-cooled alternatives, and the
      permits that make or break a greenfield site
    - Carbon intensity of local grid as a disclosed metric, grid
      mix sensitivity by region, and the growing audit scrutiny
      of "net zero via unbundled RECs" claims
    - Lifecycle emissions and embodied carbon in the fab and the
      data center shell as the next audit frontier

16. **Site-selection geography**
    - US clusters — Northern Virginia, Columbus, Phoenix, Dallas,
      Reno, Iowa, Oregon — and their 2026-era constraints (grid,
      transformer lead times, water, community opposition,
      including the 12-month data-center moratorium adopted in
      Loudoun County in September 2026)
    - EMEA clusters — Ireland, Netherlands, Germany (Frankfurt),
      Nordics (Stockholm, Oslo, Helsinki) for renewable-rich
      operation, Spain, Portugal, Italy for south-Europe anchor
    - APAC clusters — Singapore (constrained by moratorium
      history), Sydney, Tokyo, Osaka, Mumbai, Jakarta, Seoul
    - Emerging clusters — Saudi Arabia (HUMAIN's multi-GW
      build-out and NEOM), UAE (Abu Dhabi, including Stargate UAE),
      Malaysia (Johor as the primary Singapore spillover corridor,
      with multi-GW of announced capacity), and sovereign-compute
      siting
    - Latency geography that forces inference siting independent
      of training siting

17. **Edge and distributed AI architectures**
    - The inference-at-the-edge pattern — CDN-adjacent small-model
      inference for latency, with the frontier model called from
      a central region
    - On-device inference (phone, laptop, IoT, automotive) as a
      *sovereignty* choice, not just a latency choice — data never
      leaves the device, which collapses the transfer-impact-
      assessment problem
    - The operator / telco MEC overlay and when it is appropriate
    - Industrial and automotive edge — safety-critical ML with
      dual-site operation, ISO 26262, IEC 61508 overlay
    - The honest edge taxonomy — "edge" means at least five
      different things in current vendor literature; name which
      one in architecture documents

### Sovereign AI, National Programs, and Public-Private Partnerships

18. **National AI compute and model programs**
    - US — National AI Research Resource (NAIRR), Department of
      Energy exascale programs (Frontier, Aurora, El Capitan),
      and the AI Safety Institute network
    - EU — EuroHPC (JUPITER, LUMI, Leonardo, MareNostrum 5),
      AI Factories initiative, and the AI Gigafactories tender
      launched in July 2026 (up to seven sites, targeted combined
      EU-plus-private investment of over €30 billion, selection
      expected in early 2027)
    - UK — AI Research Resource, Isambard-AI, Dawn, and the AI
      Safety Institute as an anchor tenant
    - France — Jean Zay, CMA-CGM/Mistral, "Choose France" and
      the Paris AI Action Summit outputs
    - Germany, Italy, Spain — national HPC and AI programs under
      the EuroHPC umbrella
    - Japan ABCI, South Korea KISTI / NIA, Singapore SingHealth
      and AI Singapore
    - UAE G42 / Core42 / Falcon (with the 2024 Microsoft
      investment and associated US-coordinated technology-stack
      alignment), Saudi HUMAIN (launched 2024 with announced
      multi-GW compute commitments), India AI Mission and the
      IndiaAI compute marketplace (expanded in 2026), Indonesia
      and Vietnam sovereign programs
    - China — the national AI compute network and the provincial
      compute alliances; "East Data West Compute" (东数西算)
      interconnect strategy as a case study in national
      compute-topology planning

19. **Partnership patterns with governments**
    - Preferred-vendor and framework-agreement tenders (G-Cloud UK,
      GSA federal schedule, EU DEP, ANAC Italy) as the formal
      channel
    - Sovereign-cloud joint ventures as the high-trust structure —
      French / German / Italian examples, and the Gulf / APAC
      analogs that are structurally different
    - Direct bilateral deals with national AI authorities and the
      governance implications (sovereign weight custody, red-line
      commitments, technology-transfer clauses)
    - The export-control dimension — US BIS sign-off on sovereign-
      compute deals involving advanced accelerators as a de facto
      third party to the commercial contract

20. **What a sovereign customer actually buys**
    - The "sovereign AI" bundle varies: compute capacity, data
      residency, locally trained foundation model, local-language
      performance, local-regulatory alignment, local-workforce
      commitment, and technology-transfer access
    - Pricing, SLAs, and governance arrangements are routinely
      *more* stringent than commercial — this is a demanding
      customer segment
    - The reputational and influence trade-offs — being the
      sovereign provider for jurisdiction X affects the
      organization's posture in jurisdictions Y and Z

### Multi-Region Operations and the Global Operating Model

21. **The multi-region topology decision**
    - Single-region with disaster-recovery vs. multi-region
      active-active vs. follow-the-sun vs. per-tenant pinned —
      each has a cost and complexity profile and each solves a
      different problem
    - Data-replication and consistency choices (strong, bounded-
      staleness, eventual) as they touch AI workloads
      specifically — feature stores, vector stores, model registries,
      inference caches
    - The *real* cost of multi-region — not egress alone, but the
      operational overhead of running a change in six regions and
      the reconciliation cost when one lags
    - The failure mode: "global" as an aspiration enforced by a
      single ops team in one time zone

22. **Global operations and support**
    - Follow-the-sun support with handoff rituals — not a staffing
      model, an operations discipline
    - Regional incident command and escalation when the incident
      straddles jurisdictions (a GDPR notification clock and a
      CCPA breach notice have different rules)
    - Multi-region observability — the metrics, traces, and model
      performance dashboards that are *themselves* residency-
      constrained
    - Change management under 24-hour clock — code and model
      updates that cannot simply "go to production on a Friday"
      in a multi-region operation

23. **Cultural and language dimensions**
    - Model quality in non-English languages as an infrastructure
      decision (regional fine-tunes, local evaluation sets,
      locally sourced instruction data)
    - Cultural, legal, and content-policy variance by region —
      the same output may be lawful, borderline, and prohibited
      in three different markets
    - Local-presence requirements — in-country Data Protection
      Officer, in-country legal representative (EU AI Act Article
      22 authorised representative for non-EU providers of
      high-risk AI systems, alongside the parallel GDPR Article
      27 representative for non-EU controllers and processors
      caught by Article 3(2)), in-country incident-response team
    - Regional product variance — same model, different operating
      envelope by market — as a governance artifact, not an
      implementation detail

### Resilience, Scenarios, and Geopolitical Contingency

24. **Scenario planning for infrastructure disruption**
    - Export-control expansion — a new rule removes a current
      accelerator from the organization's authorized supply
    - Cross-border transfer suspension — a *Schrems III*-style
      decision invalidates a current transfer mechanism and the
      replacement is not immediately available
    - Sovereign cloud mandate — a jurisdiction requires AI
      services for regulated sectors to run on an in-country
      sovereign operator
    - Regional cloud outage spanning a cascading failure (Azure
      2024, AWS 2017, GCP 2020 as teaching cases)
      <!-- needs-research: refresh the list of significant
      multi-hour multi-region hyperscaler incidents with
      published post-mortems -->
    - Nation-state-level disruption — regional conflict, physical
      cable cut, embargo

25. **Resilience design under geopolitical stress**
    - Dual-cloud (not dual-region on the same cloud) as the
      honest bar for sovereignty-grade resilience
    - Dual-silicon — training and inference portable across NVIDIA /
      AMD / TPU / Trainium with evaluated performance deltas, not
      claimed portability
    - Dual-jurisdiction for the most sensitive workloads — the
      ability to re-home a workload across borders inside a
      regulatory clock
    - Weight custody and escrow arrangements with sovereign
      customers, including the "vendor goes dark" clause
    - The documented downgrade path — what the service looks like
      when a tier of infrastructure is removed, not simply
      "undefined"

26. **Business-continuity artifacts the board will want**
    - The infrastructure risk register — named scenarios, named
      owners, named mitigations, named leading indicators
    - The exit plan from each critical vendor (hyperscaler, model
      vendor, GPU vendor) with cost and time-to-cutover documented
    - The regulatory-escalation playbook — who the organization
      calls at each key regulator on day one of a crisis, and
      what has been pre-wired
    - Tabletop exercise cadence — at least annual, cross-functional,
      with named observers and documented findings

### Communicating a Global Posture

27. **Five audiences, five stories**
    - **Board**: fiduciary-grade framing of concentration risk,
      geopolitical exposure, and the capital commitments the
      answer requires
    - **Regulator (home jurisdiction)**: control evidence,
      jurisdiction-specific artifacts (DPIA, FRIA, TIA, AI Act
      technical documentation)
    - **Regulator (host jurisdiction)**: local-presence, local-
      language support, data-residency evidence
    - **Government customer**: sovereignty bundle, red lines,
      weight custody, technology-transfer commitments
    - **Workforce**: the honest account of what moves, what
      doesn't, which roles are regional, which are global

28. **The global infrastructure narrative**
    - The quarterly board update — concentration, residency
      posture, sovereign exposure, scenario readiness
    - The customer-facing transparency note — where your data
      runs, under which law, with which supplementary measures
    - The regulator-facing disclosure — same facts, different
      altitude, same vocabulary
    - The internal operating-review deck — leading indicators,
      not vanity capacity numbers

---

## Module Structure

```
mod-406-global-infrastructure/
├── README.md (you are here)
├── lecture-notes/
│   └── 01-overview.md  (one strategic-level lecture)
├── exercises/
│   ├── exercise-01-case-study.md
│   ├── exercise-02-strategy-memo.md
│   ├── exercise-03-stakeholder-mapping.md
│   ├── exercise-04-roadmap.md
│   └── exercise-05-presentation.md
├── quiz.md
└── resources.md
```

### Week 1: The Global AI Infrastructure Map and Compute Supply Chain (6 hours)

**Topics:**
- The hyperscaler, GPU-specialist, and sovereign-cloud topology —
  what each tier is actually for, and which workloads belong where
- The silicon supply chain as a map — design, fabrication,
  packaging, HBM, lithography — and the choke points that make
  "diversify our GPU supplier" a harder sentence than it reads
- US export controls as the ambient constraint on every global
  AI deployment plan — BIS performance thresholds, Entity List
  mechanics, Foreign Direct Product Rule, Validated End User
  <!-- needs-research: cite the current BIS final rule text and
  any pending or proposed updates at time of use -->
- Reading an organization's current compute posture as a
  concentration-risk disclosure — supplier, region, silicon,
  model-vendor, and the single-point-of-failure that each one
  hides

**Readings:**
- US Bureau of Industry and Security — AI diffusion / AI compute
  export-control rules (consolidated Federal Register text)
  <!-- needs-research: pin to the specific final-rule citation at
  time of use; this is the most volatile input in the module -->
- Chris Miller — *Chip War: The Fight for the World's Most
  Critical Technology*
- CSIS Wadhwani AI Center — published reports on compute
  governance and the chip supply chain
  <!-- needs-research: refresh the current report list from CSIS
  and from CNAS / Georgetown CSET -->
- Primary-source hyperscaler regional-infrastructure pages
  (AWS Global Infrastructure, Azure global infrastructure, Google
  Cloud locations)
- TeleGeography submarine-cable map as a working reference

**Exercise:** Audit your organization's current AI compute posture.
Draw the supplier map (design → fab → cloud → region → workload)
and identify the top three concentration risks. A one-page memo to
the CTO on what the map actually shows. See
`exercises/exercise-01-case-study.md` for a structured version.

---

### Week 2: Data Sovereignty, Residency, and Cross-Border Transfers (8 hours)

**Topics:**
- Residency vs. localization vs. sovereignty as distinct legal
  claims — and the evidence each claim actually requires
- GDPR Chapter V and the Schrems-era transfer regime — SCCs,
  BCRs, adequacy, supplementary measures, and the live state
  of the EU-US Data Privacy Framework
  <!-- needs-research: confirm current DPF status and any pending
  CJEU challenge -->
- PIPL, India DPDP, Brazil LGPD, South Korea PIPA, Japan APPI,
  and the residency / cross-border pattern each one actually
  produces
- The output-side residency problem — weights, embeddings, logs,
  prompts, RAG stores — and why "data stays in-region" is a
  partial answer at best
- Sector overlays (HIPAA, GLBA, FERPA, ITAR/EAR, PCI-DSS) as
  the real residency constraint for regulated-industry workloads

**Readings:**
- EU Regulation 2016/679 (GDPR) Chapter V (consolidated OJ text)
- European Data Protection Board — Recommendations 01/2020 on
  supplementary measures and subsequent guidance
  <!-- needs-research: pin to the current EDPB publication list -->
- CJEU *Schrems II* judgment (Case C-311/18) — read the
  operative paragraphs on supplementary-measure obligations
- CAC — *Interim Measures for the Management of Generative
  Artificial Intelligence Services* (2023) and the PIPL
  cross-border transfer standard-contract measures
  <!-- needs-research: cite current CAC Generative AI measures
  text and most recent amendments -->
- NIST AI 600-1 — *Generative AI Profile*, with emphasis on data
  and IP risk categories

**Case Study:** A multinational health-insurance company wants to
deploy a GenAI customer-service agent in the US, EU, UK, Canada,
and Japan. The underlying foundation model is hosted on a
hyperscaler API. Training data includes US clinical records;
inference logs would, by default, return to the vendor. Design
the residency and cross-border posture for the deployment, with
jurisdiction-by-jurisdiction defensibility. See
`exercises/exercise-02-strategy-memo.md`.

**Deliverable:** A data-sovereignty compliance framework covering:
- Residency classification by data class and jurisdiction
- Lawful-transfer mechanism and supplementary measures per route
- Weight / embedding / log / prompt residency positions
- Named audit artifacts (DPIA, TIA, FRIA entries)

---

### Week 3: Regional Regulation and the Compliance Matrix (6 hours)

**Topics:**
- The EU AI Act as the globally reaching template — scope,
  extraterritoriality, role mapping, application-date table
- The US patchwork — NIST AI RMF, federal executive orders,
  sector-regulator enforcement, state AI laws (Colorado, New
  York, Texas, Utah, California), New York Local Law 144 as a
  precedent for employment screening
  <!-- needs-research: refresh the state-AI-law inventory at time
  of use; this changes on roughly a quarterly cadence -->
- UK, Canada, Australia, Singapore, Japan, South Korea — the
  pro-innovation / sector-led axis and where it produces a
  different compliance artifact than the EU rules-led axis
- China and jurisdictions with structurally different regimes
  — PIPL, generative-AI measures, deep-synthesis rules, CII
  designation, filing and security-assessment obligations
- ISO/IEC 42001, 23894, 5338, 42005, 5259 as the common
  vocabulary that makes the multi-regime map tractable
  <!-- needs-research: verify current publication status of each
  ISO AI-series standard -->

**Readings:**
- Regulation (EU) 2024/1689 (EU AI Act) — Articles 1-6, 50-55,
  85-99 (prohibited, GPAI, transparency, enforcement, fines)
  <!-- needs-research: lock the citation to the final OJ text -->
- NIST AI 100-1 — *AI Risk Management Framework (AI RMF 1.0)*
  core document
- OECD AI Policy Observatory — ongoing jurisdictional updates
- Published cross-jurisdictional AI-law trackers (academic and
  reputable law-firm / policy-think-tank trackers)
  <!-- needs-research: identify two or three continuously updated
  trackers and cite directly rather than via press summaries -->

**Exercise:** 1-page strategy memo recommending a specific
regional-compliance posture — e.g., "Operate the EU and UK
estate as the control surface; adopt the EU AI Act technical
documentation and FRIA as the enterprise baseline and apply
deltas to US sector and state overlays rather than maintaining
three parallel frameworks." See `exercises/exercise-02-strategy-memo.md`.

**Deliverable:** A regional compliance matrix: for each major
jurisdiction the organization operates in, the applicable AI
rules, data-protection rules, sector overlays, residency
expectations, and the specific evidence artifacts shipped under
each. Rows = jurisdictions; columns = control surfaces; cells =
named artifact + owner + review cadence.

---

### Week 4: Siting, Energy, and the Multi-Region Architecture (8 hours)

**Topics:**
- Power, grid, and water as the first-order constraints on
  training-cluster site selection — PPAs, interconnection
  queues, transformer lead times, water permits, community
  consent
  <!-- needs-research: cite current IEA / EPRI / LBNL data on
  data-center electricity demand, and the regional-grid stress
  reports from ERCOT, PJM, Ireland CRU, Virginia SCC, etc. -->
- The global siting map — US, EMEA, APAC, emerging clusters —
  with the 2026-era constraints that each one is actually under
- Carbon, embodied emissions, and the audit frontier beyond
  "100% renewable via unbundled RECs"
- The multi-region topology decision — single-region-with-DR vs.
  active-active vs. follow-the-sun vs. per-tenant pinned, with
  the trade-offs stated explicitly
- Edge and distributed inference — CDN-adjacent small-model
  inference, on-device inference as sovereignty, MEC and
  industrial-edge when they are appropriate
- The replication and consistency choices that touch AI
  workloads specifically — feature stores, vector stores, model
  registries, inference caches

**Readings:**
- International Energy Agency — most recent *Electricity* / data-
  center demand report
  <!-- needs-research: pin to the most recent IEA publication at
  time of use (the "Electricity 2024" and successor reports
  update annually) -->
- Lawrence Berkeley National Laboratory — U.S. data-center energy
  usage reports (2024 and later)
- Uptime Institute — Global Data Center Survey (current year)
- Google *Carbon-Free Energy* and 24/7 CFE methodology primary
  documents, as an example of audit-grade carbon claims
- Published post-mortems from significant multi-region cloud
  outages (AWS, Azure, GCP) as applied reliability case material
  <!-- needs-research: refresh the list of significant published
  post-mortems within the last 24 months -->

**Case Study:** Your organization is planning a 500-MW training
campus. The business requires it operational within 36 months.
Three candidate sites are on the table: Northern Virginia (grid-
constrained, strong interconnection), Nordic (renewable-rich,
cooler-climate, longer latency to US customers), and a Gulf-state
sovereign-cluster partnership (power-cheap, geopolitically
exposed, data-residency implications). Design the decision
framework, including a defensible comparative total-cost picture,
risk register, and a stakeholder pre-wiring plan for CFO, CRO,
General Counsel, Chief Trust Officer, and board.

**Deliverable:** Global AI infrastructure architecture (15-20
pages) covering:
- Target regional topology for training and inference
- Siting rationale (power, water, latency, carbon, sovereignty,
  cost)
- Replication / residency / weight-custody posture by workload
  class
- Edge and on-device strategy
- The three concentration risks the architecture *does not*
  mitigate and the explicit rationale for accepting them

---

### Week 5: Sovereign AI, National Programs, and the Operating Model (10 hours)

**Topics:**
- The sovereign-AI product category — what a sovereign customer
  actually buys (compute, residency, local model, local
  language, local workforce, technology transfer) and how it
  differs from a commercial contract
- National AI compute and model programs (US NAIRR, EuroHPC and
  AI Factories, UK AI Research Resource, France Jean Zay, Japan
  ABCI, UAE / Saudi programs, India AI Mission, China provincial
  alliances and "East Data West Compute") as subsidized access
  under conditions
  <!-- needs-research: refresh the current list of major
  sovereign AI compute programs, their stated capacity, and
  their access-eligibility rules -->
- Partnership patterns with governments — framework-agreement
  tenders, sovereign-cloud joint ventures, direct bilateral
  deals, export-control sign-off as a de facto third party
- The multi-region operating model — follow-the-sun support,
  regional incident command, multi-region observability under
  residency constraint, change management under a 24-hour clock
- Cultural, language, and local-presence requirements — DPO,
  authorised representative, in-country IR, regional product
  variance as a governance artifact
- The Alibaba Cloud and Tencent Cloud regional-compliance
  playbook (where multinational-vendor normal operations
  collide with CII designation and MLPS 2.0) as a case study
  <!-- needs-research: verify current CII designation scope and
  any recent enforcement examples -->

**Readings:**
- EuroHPC Joint Undertaking — public program documents on JUPITER,
  LUMI, Leonardo, MareNostrum 5, and the AI Factories / AI
  Gigafactories initiative
  <!-- needs-research: confirm current AI Factory and Gigafactory
  site selections and funding scale -->
- UK AI Safety Institute and UK AI Research Resource — published
  program materials
- US NSF — NAIRR pilot documents
- Published sovereign-AI deal structures (publicly disclosed
  Microsoft-G42, AWS-NAIRR-equivalent arrangements, Oracle gov
  cloud regions)
  <!-- needs-research: refresh the list of major publicly
  disclosed sovereign-AI partnerships and deal structures -->
- OECD AI Policy Observatory — national AI strategies database

**Case Study:** Your organization — a US-headquartered AI platform
vendor — is invited to co-found a sovereign-AI partnership with
a Gulf-state government. The deal includes a 2-GW compute
commitment, locally hosted weights, a local-language foundation-
model program, and a workforce-development commitment in-country.
The US Department of Commerce has signaled that export-control
sign-off on advanced accelerators is possible under a Validated
End User-style structure with specific security and end-use
conditions. General Counsel is concerned about Article 5 EU AI
Act prohibitions in the model's downstream reach. The CEO sees a
strategic positioning win. Draft the decision memo and the
build / partner / regionalize / decline recommendation. See
`exercises/exercise-03-stakeholder-mapping.md`.

**Deliverable:** Global operations model proposal (10-15 pages)
covering:
- Regional ownership and local-presence structure
- Follow-the-sun incident model and jurisdictional escalation
- Observability and change-management under residency constraint
- Sovereign-customer engagement playbook (if applicable)
- Named failure modes and documented mitigations

---

### Week 6: Resilience, Contingency, and Board Communication (6 hours)

**Topics:**
- Scenario planning for infrastructure disruption — export-
  control expansion, cross-border transfer suspension, sovereign-
  cloud mandate, regional cloud outage, nation-state-level
  disruption
- Resilience design under geopolitical stress — dual-cloud, dual-
  silicon, dual-jurisdiction, weight custody and escrow, a
  documented downgrade path
- Business-continuity artifacts the board will want — the
  infrastructure risk register, exit plans from each critical
  vendor, the regulatory-escalation playbook, tabletop cadence
- Board-level global-infrastructure reporting — concentration,
  residency posture, sovereign exposure, scenario readiness —
  as a quarterly standing agenda item
- The global narrative externally — customer-facing transparency,
  regulator-facing disclosure, government-customer commitments
- The "visible infrastructure incident" scenario — regional
  outage with cross-border customer impact, during a residency-
  sensitive workload — as the stress test for the entire
  operating model

**Readings:**
- Gary Klein, HBR — "Performing a Project Premortem" (applied to
  global-infrastructure contingency, as in MOD-402 and MOD-404)
- Barbara Minto — *The Pyramid Principle* (reinforced from
  MOD-402 for board-facing communication)
- NIST SP 800-34 (Contingency Planning) applied to AI workloads
  <!-- needs-research: confirm current revision of SP 800-34 and
  any AI-specific contingency guidance from NIST -->
- Published global-infrastructure board disclosures from AI-heavy
  public companies (10-K risk factors on compute concentration,
  geopolitical exposure, data-residency litigation)
  <!-- needs-research: assemble a short list of current 10-K and
  equivalent disclosures that treat AI infrastructure as a
  material risk factor -->
- AI Incident Database and Partnership on AI — infrastructure-
  adjacent incident patterns

**Scenario:** The US BIS issues an emergency order on a Friday
restricting the export of your current primary accelerator
generation to one of your production regions. Your largest
training run has eight weeks remaining and a $40M committed
cluster lease on now-restricted silicon. Your board calls a
special session Monday morning. Draft:
- 1-page board briefing (what is contained, what is not, options
  with 30/60/90-day impact, what you are asking the board to
  approve)
- Internal all-hands note (workforce framing, including the
  teams that would move or pause under each option)
- Regulator communications under each option (including the
  home-jurisdiction and host-jurisdiction regulators)
- 30/60/90-day plan under the chosen option with named owners
- Decision log template for the next 72 hours

**Exercise:** Board-level presentation on the current state of the
organization's global AI infrastructure posture. See
`exercises/exercise-05-presentation.md`.

**Deliverable:** Board-ready deck (10-15 slides) on the state of
the organization's global AI infrastructure program, reviewed
with a peer using the "so what?" test at every slide.

---

## Case Studies

### Case Study 1: Google Cloud's Global Infrastructure as a Deployer Reference

**Background:**
- One of three hyperscalers with a globally reaching AI platform,
  operating a regional topology that spans the Americas, EMEA,
  and APAC, with a parallel sovereign-adjacent footprint
  (GovCloud-class offerings, EU-sovereign initiatives, and
  regional partnerships)
- Public commitments on carbon-free energy, water replenishment,
  and operational transparency are themselves an audit artifact
  that enterprise buyers are asked to consume and translate
  <!-- needs-research: confirm current Google Cloud regional
  footprint, sovereign-cloud offerings, and most recent
  environmental report -->
- Serves as a *reference architecture* that senior architects at
  deployer organizations are expected to read as a design
  document, not just a supplier catalog

**Your Role:** Senior AI infrastructure architect at a
multinational deployer evaluating whether to standardize AI
workloads on a single hyperscaler's global topology or to pursue
a dual-cloud posture with sovereignty-grade segregation.

**Assignment:**
1. Produce a current-state assessment of the hyperscaler's
   global AI topology as it applies to your organization's
   workload mix — which regions are usable for which workloads,
   which are usable with supplementary measures, which are not
2. Compare the single-hyperscaler-global posture against a
   dual-cloud posture across TCO, operational complexity,
   resilience, residency defensibility, and vendor concentration
3. Identify the three workloads where the single-hyperscaler
   posture is *clearly* correct and the three where it is
   *clearly* insufficient
4. Pre-wire the posture with CFO, CTO, CRO, General Counsel,
   Chief Trust Officer, and the board

**Deliverables:**
- Current-state assessment (10 pages)
- Comparative posture memo (5-7 pages)
- Three-option decision brief (concentrate / split / segregate)
- Stakeholder pre-wiring plan
- Board-facing recommendation memo

**Success Criteria:**
- Assessment is defensible under an external audit on
  concentration risk and residency posture
- Decision survives a CFO challenge on multi-year TCO and a
  CRO challenge on geopolitical scenario coverage
- Workload-level recommendations are specific and testable, not
  "mostly cloud A with some cloud B"

---

### Case Study 2: Alibaba Cloud and Regional Compliance for a Multinational Operating in China

**Background:**
- Multinational organization with a significant business in
  mainland China, operating AI workloads that would, by default,
  run on a global hyperscaler
- Chinese regulatory regime — PIPL, Data Security Law,
  Cybersecurity Law, CAC Generative AI Interim Measures,
  deep-synthesis rules, algorithmic recommendation filing, CII
  designation for the sector — collides with that default
  <!-- needs-research: verify current filing / security-
  assessment regime applicable to foreign and domestic
  generative-AI service providers in China -->
- Local sovereign-cloud alternatives (Alibaba Cloud, Tencent
  Cloud, Huawei Cloud) are the de facto in-China deployment
  path for regulated workloads
- US export-control overlay affects which accelerators and which
  foundation-model weights can be deployed in-region at all

**Your Role:** Senior architect responsible for the global AI
platform, chartered with defining the in-China operating model
alongside the China general manager, the Global General Counsel,
and the Chief Trust Officer.

**Assignment:**
1. Classify the organization's AI workloads against Chinese
   regulatory categories — generative, deep-synthesis,
   algorithmic recommendation, CII-sector, non-regulated
2. Produce a defensible in-China deployment architecture —
   which workloads run on a local sovereign cloud, which run
   on a cross-border transfer path with evidence, which cannot
   run at all
3. Reconcile the in-China posture with the global posture —
   avoid the "two parallel programs" failure mode while
   accepting that convergence is structurally impossible on
   several control surfaces
4. Design the escalation path for a regulator inquiry — CAC,
   local Public Security Bureau, sector regulator — including
   named local counsel and named local executive accountability

**Deliverables:**
- Workload-classification matrix against Chinese AI regulation
- In-China deployment architecture (10-15 pages)
- Cross-border-transfer evidence pack for workloads that remain
  cross-border
- Regulator-engagement playbook for the China entity
- Board communication on the in-China posture

**Success Criteria:**
- Architecture is defensible to Chinese regulators under the
  current regime and under a near-term tightening scenario
- Posture does not create a compliance deficit in other
  jurisdictions (EU AI Act, US export controls, sectoral rules
  in home market)
- The organization retains a defensible exit from any
  individual Chinese vendor without losing continuity of
  service to Chinese customers

---

### Case Study 3: HSBC-Style Global AI Platform Across Six Regulatory Regimes

**Background:**
- Global financial-services organization operating in the UK,
  EU, US, Hong Kong, Singapore, UAE, and roughly thirty other
  jurisdictions, with a shared AI platform ambition
- Financial-sector regulators (PRA/FCA in the UK, EBA/ECB in the
  EU, Fed/OCC/FDIC/CFPB in the US, HKMA, MAS, CMA KSA, DFSA /
  FSRA in the UAE) each have their own AI / model-risk
  expectations layered on top of general AI law
  <!-- needs-research: cite current PRA SS1/23 model-risk
  supervisory statement, OCC/Fed/FDIC SR 11-7 and any AI-specific
  updates, HKMA GenAI principles, MAS FEAT and AI guidelines -->
- Workloads span credit decisioning (high-risk under EU AI Act),
  customer service (lower-risk but transparency-obligated),
  financial-crime screening (sector-overlay-heavy), and
  internal productivity (lightest-touch)
- Residency expectations in some jurisdictions (UAE, India,
  China, Saudi Arabia) require in-country processing for
  regulated-customer data

**Your Role:** Senior AI infrastructure architect, newly
chartered to produce the enterprise global-AI-platform
architecture and operating model, reporting to the Group CIO
with a dotted line to the Chief Risk Officer and the Chief
Compliance Officer.

**Assignment:**
1. Produce a defensible global AI infrastructure architecture
   — regional topology, workload siting, residency positions,
   edge and on-device choices — grounded in the organization's
   actual regulatory footprint
2. Produce a regional compliance matrix covering the top ten
   jurisdictions, with named control surfaces, named artifacts,
   and named owners
3. Design the global operating model — follow-the-sun support,
   regional incident command, multi-region observability under
   residency constraint, change management under a 24-hour
   clock — including the authorised representative and
   DPO-equivalent appointments required
4. Design the contingency regime — dual-cloud, dual-silicon,
   dual-jurisdiction — with the specific workloads that each
   contingency actually protects, and the ones it does not
5. Pre-wire with CFO, CRO, CCO, Chief Trust Officer, General
   Counsel, business-unit CEOs, and the board risk committee

**Deliverables:**
- Global AI infrastructure architecture (20-25 pages)
- Regional compliance matrix (tabular, with a narrative overlay)
- Global operations model
- Contingency and resilience plan with named scenarios
- Board-risk-committee communication pack
- Workforce and local-presence plan

**Success Criteria:**
- Architecture is defensible under the PRA / FCA model-risk
  framework, under the EU AI Act high-risk regime, and under
  US federal and state AI rules simultaneously
- Residency posture holds up to a parallel inquiry by at least
  three data-protection authorities
- Contingency plan has been tabletop-exercised across at least
  two of the named scenarios before go-live
- The platform survives a leadership change, a visible incident,
  and a regulatory enforcement action without the architecture
  being re-drawn

---

## Exercises and Activities

The five exercises in `exercises/` are structured so each one feeds
the next. Treat them as a sequence, not a menu.

### Exercise 1: Case Study Analysis (3 hours)
Find a published global-infrastructure case (HBR, Stanford, MIT,
primary-source engineering-blog post from a hyperscaler or large
deployer, or a published regulator enforcement action or data-
protection authority decision). Summarize, critique trade-offs,
and apply three lessons to your own organization.
See `exercises/exercise-01-case-study.md`.

### Exercise 2: 1-Page Strategy Memo (3 hours)
Write a 1-page memo to your CEO, CTO, CRO, Chief Trust Officer,
or board chair on a specific global-infrastructure investment —
e.g., "Adopt a dual-cloud posture across EU and US for
sovereignty-grade workloads before any customer-facing GenAI
launch in the EU," or "Enter a sovereign-cloud partnership in
jurisdiction X with specific red lines on export control, weight
custody, and technology transfer." TL;DR, current state,
recommendation, ask, risks, red-line commitments.
See `exercises/exercise-02-strategy-memo.md`.

### Exercise 3: Stakeholder Map + Influence Plan (4 hours)
Map sponsors, supporters, neutrals, and blockers across CEO, CFO,
CTO, CRO, CISO, CPO, General Counsel, Chief Trust Officer, Chief
Communications Officer, business-unit leaders, worker
representation, and at least one external stakeholder (regulator,
government customer, sovereign-cloud partner, hyperscaler account
team). Convert to a 90-day engagement plan with sequenced
conversations.
See `exercises/exercise-03-stakeholder-mapping.md`.

### Exercise 4: 3-Year Global Infrastructure Roadmap (5 hours)
Draft a 3-year roadmap for the enterprise global AI infrastructure
program, broken into quarterly milestones. Each phase: success
metrics (regional coverage, residency-posture defensibility,
concentration-risk delta, scenario-readiness coverage), investment,
key deliverables, and the specific control coverage delta over
the prior quarter.
See `exercises/exercise-04-roadmap.md`.

### Exercise 5: Board-Level Presentation (5 hours)
A 10-slide deck for a board (or board risk / technology committee)
on the current state and forward plan of the global AI
infrastructure program, reviewed with a peer using the "so what?"
test at every slide.
See `exercises/exercise-05-presentation.md`.

---

## Assessment

### Module Quiz

Short strategic-thinking questions — no crisp right answers, defend
your position. See `quiz.md` for the full prompt list.

### Strategic Global Infrastructure Portfolio (8-10 hours)

A single coherent artifact set built around *one* global AI
infrastructure program you would design for a real (or realistic
composite) organization:

1. **Global AI infrastructure architecture** (15-20 pages,
   CFO- and CRO-approvable)
2. **Data sovereignty compliance framework** (residency
   classification, transfer mechanisms, weight / embedding / log
   positions, named audit artifacts)
3. **Regional compliance matrix** (top ten jurisdictions, with
   named control surfaces, named artifacts, and named owners)
4. **Global operations model** (regional ownership, follow-the-
   sun, incident command, observability, change management,
   local presence)
5. **Contingency and resilience plan** (named scenarios, dual-
   cloud / dual-silicon / dual-jurisdiction positions, exit
   plans, tabletop cadence)
6. **Board-level status deck** (10-12 slides)

All six artifacts must describe the *same* global AI
infrastructure program and must be internally consistent. A
reviewer should be able to spot-check any two and find the same
regional topology, the same residency positions, the same
sovereign exposure, and the same contingency vocabulary.

**Evaluation Criteria:**
- **Internal coherence** (25%) — architecture, compliance
  framework, matrix, operating model, and board deck tell the
  same story at every altitude
- **Residency defensibility** (20%) — positions survive a
  jurisdiction-by-jurisdiction audit, not just a summary-level
  claim
- **Geopolitical realism** (15%) — contingency plan addresses
  actual recent and plausible disruption scenarios, not
  abstract risks
- **Operational realism** (15%) — operating model is something
  a real support team can run across time zones, not an org
  chart
- **Executive communication** (15%) — board deck is answer-first,
  concentration and scenario readiness over vanity capacity
- **Right-sizing** (10%) — the program fits the organization,
  neither sovereignty-theater nor a single-region monolith

---

## Resources

### Required Reading

1. **Primary frameworks, standards, and law**
   - EU Regulation 2024/1689 (AI Act) — Articles 1-6, 50-55,
     85-99 and the application-date table
     <!-- needs-research: lock the citation to the published
     Official Journal reference -->
   - EU Regulation 2016/679 (GDPR) Chapter V and the EDPB
     Recommendations 01/2020 on supplementary measures
   - CJEU *Schrems II* judgment (Case C-311/18)
   - NIST AI 100-1 — *AI Risk Management Framework (AI RMF 1.0)*
   - NIST AI 600-1 — *Generative AI Profile*
   - US BIS — AI diffusion / AI compute export-control rules
     (consolidated Federal Register text)
     <!-- needs-research: pin to the specific final-rule citation
     at time of use; the AI-chip rule set updates several times
     per year -->
   - CAC — *Interim Measures for the Management of Generative
     Artificial Intelligence Services* (2023) and the PIPL
     cross-border transfer standard-contract measures
   - ISO/IEC 42001 (AI management system), ISO/IEC 23894 (AI risk
     management), ISO/IEC 5338 (AI lifecycle), ISO/IEC 42005
     (AI impact assessment)
     <!-- needs-research: confirm the current publication status
     of each standard -->

2. **Books and long-form references**
   - Chris Miller — *Chip War: The Fight for the World's Most
     Critical Technology*
   - Anu Bradford — *The Brussels Effect* (background on EU
     regulatory globalization that underlies the AI Act)
   - Anu Bradford — *Digital Empires: The Global Battle to
     Regulate Technology*
   - Thomas Wright — *All Measures Short of War* (background
     on the geopolitical frame)
   - Daniel Yergin — *The New Map* (energy-and-geopolitics
     background that increasingly rhymes with AI compute siting)

3. **Policy and technical reports**
   - International Energy Agency — most recent *Electricity* /
     data-center-demand report
     <!-- needs-research: pin to the most recent IEA publication
     at time of use -->
   - Lawrence Berkeley National Laboratory — U.S. data-center
     energy usage reports (2024 and later)
   - Uptime Institute — Global Data Center Survey (current year)
   - Georgetown CSET, CNAS, CSIS Wadhwani AI Center — published
     reports on compute governance, export controls, and
     sovereign AI
     <!-- needs-research: refresh the current report lists from
     each institution at time of use -->
   - OECD AI Policy Observatory — ongoing jurisdictional and
     implementation updates

### Supplementary Resources

- Hyperscaler primary-source infrastructure and sustainability
  reports (AWS, Azure, GCP, Oracle, IBM, Alibaba Cloud,
  Tencent Cloud, Huawei Cloud)
- EuroHPC Joint Undertaking — public program documents on
  JUPITER, LUMI, Leonardo, MareNostrum 5, and the AI Factories /
  Gigafactories initiative
  <!-- needs-research: refresh program state at time of use -->
- UK AI Safety Institute, US AI Safety Institute, AISI network
  publications
- NSF NAIRR pilot documents; US DOE exascale program
  documentation (Frontier, Aurora, El Capitan)
- TeleGeography submarine-cable and interconnection maps
- Published post-mortems from significant multi-region cloud
  outages (AWS, Azure, GCP)
  <!-- needs-research: assemble a current list within the last
  24 months -->
- 10-K risk factors on compute concentration, geopolitical
  exposure, and AI-regulatory risk from AI-heavy public companies
  <!-- needs-research: assemble a current short list -->

See also `resources.md` in this module for the running reading list.

---

## Next Steps

Upon completing MOD-406, you will be prepared to:

1. **Produce and defend** a global AI infrastructure
   architecture across hyperscaler, GPU-specialist, and
   sovereign-cloud layers
2. **Classify** workloads against a residency and cross-border
   transfer regime that survives GDPR, Schrems-era challenges,
   sector overlays, and emerging data-localization laws
3. **Translate** chip export controls, foundation-model
   licensing terms, and sovereign-cloud offerings into a build /
   partner / regionalize / decline decision
4. **Design** a multi-region operating model with explicit,
   documented trade-offs across latency, availability, cost,
   carbon, and sovereignty
5. **Lead** the organization through a geopolitical
   infrastructure disruption, including the regulator, workforce,
   and board communications under time pressure
6. **Progress to MOD-407**: Strategic Partnerships and Vendor
   Management

---

**Ready to begin?** Start with Week 1: The Global AI
Infrastructure Map and Compute Supply Chain.

## Cross-references
- Engineering-level prerequisite: see ai-infra-engineer-learning + ai-infra-senior-engineer-learning
- Solutions repo: ai-infra-senior-architect-solutions/modules/mod-406-global-infrastructure
