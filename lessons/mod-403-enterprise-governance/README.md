# MOD-403: Enterprise AI Governance

**Level**: Senior Architect (Strategic / Executive)
**Duration**: 35-50 hours
**Prerequisites**: Architect-level experience; mod-401 (Enterprise AI Strategy); mod-402 (Executive Leadership) recommended

## Module Overview

This module is part of the Senior AI Infrastructure Architect curriculum
(level 400). Focus: enterprise governance.

Senior-architect modules emphasize executive communication, strategic
thinking, and organizational influence — not hands-on implementation.
For hands-on technical material on related topics (model-card tooling,
evaluation pipelines, policy-as-code, lineage), see the engineer-level
and senior-engineer-level repos.

### Executive Summary

MOD-401 taught you to *build* an AI strategy and MOD-402 taught you to
*carry* it. MOD-403 is the governance half of the senior architect's
job — the standing structures, policies, and oversight mechanisms that
let the organization keep deploying AI without the board, the regulator,
or the general counsel pulling the plug.

At this level, governance is not a document. It is an operating system
with four parts that must all be in place simultaneously: a **mandate**
(who decides, with what authority), a **policy and standards hierarchy**
(what is required, recommended, prohibited), a **control and evidence
layer** (how you prove compliance when asked), and an **oversight
cadence** (how the board and C-suite see what is actually happening in
production). A governance program with three of the four looks fine on
paper and fails under audit.

By the end of this module, you will be able to:

- Design an enterprise AI governance operating model that ties board-
  level oversight to ground-truth production controls
- Map the current global AI regulatory and standards landscape (EU AI
  Act, NIST AI RMF, ISO/IEC 42001, sector rules) to a single internal
  control framework
- Build a three-lines-of-defense model for AI risk that is credible to
  internal audit, external audit, and the regulator
- Stand up model and data governance that scales past a handful of
  pilots to the hundreds-of-models state
- Govern third-party and foundation-model risk with the same rigor as
  internally built systems
- Communicate the state of AI governance to a board of directors
  without burying the lede

---

## Learning Objectives

### Governance Operating Model

1. **Mandate and authority**
   - Define the charter of an AI governance committee (membership,
     escalation thresholds, decision rights)
   - Place the committee correctly in the enterprise governance stack
     (board → risk committee → AI governance → model risk / data /
     security / privacy / ethics)
   - Distinguish advisory bodies from decision-making bodies and avoid
     the "everyone is accountable so no one is" failure mode

2. **Three lines of defense for AI**
   - 1st line: product, engineering, MLOps teams owning the risk they
     create
   - 2nd line: model risk, compliance, privacy, security as
     independent oversight
   - 3rd line: internal audit providing assurance to the board
   - Map this model to the organization's existing operational risk
     framework instead of running a parallel one

### Regulatory and Standards Landscape

3. **Horizontal AI regulation**
   - EU AI Act — risk tiers (prohibited, high-risk, limited-risk,
     minimal-risk), obligations by actor (provider / deployer /
     importer / distributor), and the general-purpose AI model
     regime
     <!-- needs-research: confirm current obligations timeline and
     thresholds against the latest consolidated AI Act text and any
     delegated/implementing acts -->
   - U.S. federal and state posture — NIST AI RMF 1.0 and the
     Generative AI Profile as the de facto U.S. control vocabulary;
     state-level laws (e.g., Colorado AI Act, NYC Local Law 144)
     and the direction of federal activity
     <!-- needs-research: refresh federal AI executive-order /
     agency-guidance posture current to the time of use -->
   - UK, Canada, Singapore, Japan, and other jurisdictional regimes
     — principles-based vs. prescriptive approaches and the
     consequences for a global rollout

4. **Sectoral overlays**
   - Financial services: SR 11-7 / OCC 2011-12 model risk management,
     Basel operational-risk expectations, consumer-protection rules
   - Healthcare: FDA guidance on AI/ML-enabled software as a medical
     device (predetermined change control plans), HIPAA interactions
   - Employment and HR: EEOC guidance on algorithmic hiring, NYC
     Local Law 144 bias-audit mandate
   - Critical infrastructure and public sector: OMB M-24-10 and
     successor memos, agency AI-use inventories
     <!-- needs-research: verify the current OMB memo numbers and
     agency inventory requirements -->

5. **Standards as a common language**
   - ISO/IEC 42001 (AI management systems) as the ISMS-style
     backbone
   - ISO/IEC 23894 (AI risk management) and ISO/IEC 23053 (ML
     framework) for shared vocabulary
   - NIST AI RMF 1.0 (Govern / Map / Measure / Manage) and the
     Generative AI Profile
   - How to pick *one* internal control framework and crosswalk the
     rest to it rather than running five parallel programs

### Policy, Standards, and Controls Hierarchy

6. **The hierarchy**
   - **Policy** (board-approved, ~page) — what the organization
     stands for
   - **Standards** (CIO/CRO-approved, prescriptive) — what must be
     true for any AI system
   - **Procedures and controls** (operational) — how a team meets
     the standard
   - **Guidance and patterns** (optional) — how most teams *should*
     meet it
   - Each layer must point up to the next; a control with no standard
     is theater and a standard with no control is a wish

7. **Making policy enforceable**
   - Prefer paved roads to prohibitions — the easiest path must be
     the compliant path
   - Encode controls in platform (policy-as-code, CI/CD gates,
     registry-level enforcement) rather than in slide decks
   - Keep a small number of truly binding rules and a larger number
     of defaults; collapsing the two produces either over-restriction
     or widespread exception-granting

### Model and Data Governance

8. **Model lifecycle governance**
   - Model inventory as the single source of truth (every model in
     production, its owner, its purpose, its risk tier)
   - Tiered review — low-risk models self-certify, high-risk models
     go through model risk committee
   - Evaluation evidence (accuracy, fairness, robustness, safety,
     cost) retained as audit artifacts, not screenshots
   - Change control: what triggers re-approval (data drift, model
     retraining, prompt changes, system-prompt changes for GenAI)

9. **Data governance in service of AI**
   - Lineage from source → feature → training set → model → decision
   - Purpose-of-use and consent tracking for training data
   - Sensitive-data handling (PII, PHI, PCI, trade secrets,
     regulated attributes)
   - Synthetic data, data minimization, and retention policy as
     active controls, not aspirations

### Third-Party, Foundation Model, and Vendor Governance

10. **Supply-chain AI risk**
    - Foundation-model procurement — model cards, usage terms, data
      handling, output ownership, indemnification
    - Vendor AI features bolted onto non-AI products (the "AI arrived
      in your CRM last Tuesday" problem)
    - Open-weights vs. API-hosted models — the shift in where the
      risk accumulates
    - Shadow AI inventory and sanctioned-use lists

11. **Contracting and liability**
    - Clauses that actually move risk (training-data warranties,
      IP indemnification, model-update notification, data-residency)
    - When a procurement decision is really a governance decision
      and should go to the AI governance committee, not to sourcing

### Board and Executive Oversight

12. **What a board actually needs**
    - A one-page AI risk heat map by business unit and use case
    - Leading indicators (coverage of the model inventory, time-to-
      detect-drift, critical-issue backlog) over lagging ones
      (incidents counted after they hit the press)
    - Independent assurance (internal audit, external auditor, or a
      third-party assessor against ISO 42001 / NIST AI RMF)
    - A standing escalation path for AI incidents separate from
      general cyber

13. **Operating cadence**
    - Quarterly AI governance committee → semiannual risk committee
      → annual board
    - Integrating AI into the existing enterprise risk management
      (ERM) cycle instead of bolting on a parallel one
    - When to stand up a standalone board AI committee and when that
      is governance theater

---

## Module Structure

```
mod-403-enterprise-governance/
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

### Week 1: Governance Operating Model (6 hours)

**Topics:**
- The four-part operating system: mandate, policy/standards, controls,
  oversight cadence
- Three lines of defense applied to AI
- Committee charter design (membership, quorum, escalation thresholds,
  decision rights)
- Where AI governance sits relative to data governance, model risk,
  privacy, security, and ethics councils
- Failure modes: the advisory-committee trap, the shadow-committee
  trap, the compliance-theater trap

**Readings:**
- NIST AI RMF 1.0 — *Govern* function (NIST AI 100-1)
- ISO/IEC 42001:2023 — AI management systems (clauses 4-6)
  <!-- needs-research: confirm clause references against the current
  published edition -->
- *Governance of AI* — Center for the Governance of AI / academic
  surveys (selected chapters)
  <!-- needs-research: pick a canonical survey article and cite
  directly -->

**Exercise:** Draft a one-page AI governance committee charter for an
organization you know. See `exercises/exercise-01-case-study.md` for a
structured version.

---

### Week 2: Regulatory and Standards Landscape (8 hours)

**Topics:**
- EU AI Act — risk tiers, roles, obligations, timelines, GPAI model
  regime
- NIST AI RMF 1.0 and the Generative AI Profile (NIST AI 600-1)
- ISO/IEC 42001 as an audit-ready management-system standard
- Sectoral rules: SR 11-7 (financial), FDA AI/ML SaMD guidance
  (healthcare), EEOC / NYC LL144 (employment), OMB memos (U.S.
  federal use)
- Building a single internal control framework and crosswalking
  every external regime to it

**Readings:**
- NIST AI 100-1 (AI RMF 1.0) and NIST AI 600-1 (Generative AI
  Profile) — primary texts
- Consolidated text of the EU AI Act (official Journal version)
  <!-- needs-research: cite the final published Official Journal
  reference, not a pre-vote draft -->
- SR 11-7 "Guidance on Model Risk Management" (Federal Reserve /
  OCC 2011-12) — the pre-AI foundation that most model risk teams
  will extend to GenAI
- FDA: "Artificial Intelligence/Machine Learning (AI/ML)-Based
  Software as a Medical Device (SaMD) Action Plan" and the
  predetermined change control plan guidance
  <!-- needs-research: refresh against the most recent FDA
  publication at time of use -->

**Case Study:** A global financial services firm must comply with EU
AI Act (deployer + GPAI model provider obligations), SR 11-7, GDPR,
state insurance regulators, and an internal ISO 42001 program — all
on the same model inventory. Build the crosswalk and the "single
source of control" mapping that prevents five parallel audits of the
same system.

**Deliverable:** Regulatory crosswalk (one row per internal control,
columns for each external regime it satisfies, gaps flagged).

---

### Week 3: Policy, Standards, and the Enforceable Control Layer (8 hours)

**Topics:**
- The policy → standards → procedures → guidance hierarchy and why
  collapsing layers kills enforceability
- Writing a board-approvable AI policy that survives contact with
  product teams (prohibitions, risk tiering, roles, escalation)
- Standards that are testable: how a control engineer reads your
  standard and knows whether a system passes
- Paved roads and policy-as-code — moving controls from slide deck
  into platform
- Exception management: how exceptions are requested, approved,
  time-boxed, and reviewed

**Readings:**
- *The Phoenix Project* / *The DevOps Handbook* — on controls as
  flow, not friction (selected chapters)
- Google SRE book — error budgets as a governance pattern
- OPA / Rego and policy-as-code primers (not for implementation —
  for understanding the shape of enforceable policy)
  <!-- needs-research: pick a canonical OPA whitepaper or docs page
  to cite -->

**Exercise:** 1-page strategy memo recommending a specific governance
investment — e.g., "stand up a model inventory + tiered review before
we scale GenAI pilots." See `exercises/exercise-02-strategy-memo.md`.

**Deliverable:** A three-layer artifact set on the *same* governance
domain (say, GenAI use):
- 1-page policy (board-approvable)
- 3-5 page standard (CIO/CRO-approvable)
- 1 implementation pattern (engineering-consumable)

Each must trace to the next. A reviewer should be able to walk from
policy clause → standard requirement → implementation control without
jumping gaps.

---

### Week 4: Stakeholder Alignment and the Governance Coalition (8 hours)

**Topics:**
- The standing stakeholders of AI governance — General Counsel, CRO,
  CISO, CPO, Head of Compliance, Chief Data Officer, business-unit
  leaders, internal audit, external auditor, board risk committee
- Stated vs. underlying concerns (General Counsel wants defensibility,
  not purity; CFO wants predictability, not minimization; CISO wants
  blast-radius clarity, not model accuracy)
- Pre-wiring a governance proposal across the second line *before*
  the first line hears about it
- Running the room when the business wants speed and the second line
  wants pause

**Readings:**
- *Crucial Conversations* — Patterson et al.
- HBR: "A Survival Guide for Leaders" — Heifetz & Linsky (adaptive
  vs. technical change)
- IIA (Institute of Internal Auditors): The Three Lines Model (2020
  update)

**Case Study:** The General Counsel wants a prohibition on all GenAI
until an EU AI Act compliance program is in place. The CEO wants
every function to have a GenAI pilot by end of quarter. You chair
the AI governance committee. Draft the 90-day plan that converts
both into sponsors of the same roadmap.
See `exercises/exercise-03-stakeholder-mapping.md`.

**Deliverable:** Stakeholder map + 90-day engagement plan for standing
up (or reforming) an AI governance program.

---

### Week 5: Model, Data, and Third-Party Governance in Practice (10 hours)

**Topics:**
- Model inventory as the governance keystone — what fields, who owns
  it, how it stays current, what breaks when it doesn't
- Tiered review: criteria for low / medium / high / unacceptable
  risk, who signs off at each tier, what evidence is required
- Evaluation as evidence (not as benchmark theater) — fairness,
  robustness, safety, cost, drift
- Data governance for AI — lineage, purpose-of-use, consent,
  sensitive-data handling, retention, synthetic data
- Foundation-model and vendor-AI procurement — model cards, usage
  terms, indemnification, data residency, update notification
- Shadow AI: discovery, sanctioning, and the "AI arrived in your
  CRM last Tuesday" problem

**Readings:**
- NIST AI RMF 1.0 — *Map*, *Measure*, and *Manage* functions
- Mitchell et al., "Model Cards for Model Reporting" (FAT* 2019)
- Gebru et al., "Datasheets for Datasets"
- SR 11-7 — model inventory and ongoing-monitoring expectations
- EU AI Act — provider / deployer / GPAI obligations as applied to
  third-party foundation models
  <!-- needs-research: verify the current articles governing GPAI
  model providers and downstream deployers -->

**Exercise:** 3-year governance roadmap moving the organization from
"spreadsheet inventory + ad-hoc review" to "registry-backed inventory
+ tiered review + continuous evaluation + audit-grade evidence."
Quarterly milestones. See `exercises/exercise-04-roadmap.md`.

**Deliverable:** Governance roadmap (15-20 pages) covering:
- Current-state assessment (inventory coverage, review coverage,
  evidence coverage, regulatory posture)
- Target end-state tied to a chosen framework (NIST AI RMF or
  ISO/IEC 42001, not both)
- Quarterly milestones with leading indicators
- Coalition and sponsor map
- Risk register for governance-program-specific risks (not model
  risks — program execution risks)

---

### Week 6: Board Oversight, Assurance, and Incident Governance (6 hours)

**Topics:**
- What the board actually needs to see — the one-page heat map, the
  leading indicators, the independent assurance line
- Fitting AI into existing enterprise risk management (ERM) cadence
  instead of running a parallel track
- Internal audit's role: assurance over control design and operating
  effectiveness, not model correctness
- External attestation options (ISO 42001 certification, SOC 2
  mapped to AI controls, third-party AI assessments) and when each
  is worth the cost
- Incident governance: how an AI-specific incident (hallucination,
  disparate impact, prompt injection, data leakage, autonomous-agent
  action) flows through the same incident response you already have

**Readings:**
- IIA: The Three Lines Model (2020)
- COSO: *Enterprise Risk Management — Integrating with Strategy and
  Performance* (selected chapters)
  <!-- needs-research: confirm the current COSO ERM framework edition
  and the AI-specific COSO supplement if available -->
- NIST AI RMF Playbook — governance and oversight examples
- Published board-level AI-incident post-mortems (public filings,
  regulator enforcement actions)
  <!-- needs-research: assemble a current reading list of 3-5
  publicly documented AI incidents with board-level fallout -->

**Scenario:** A production AI system makes a visibly biased decision
that reaches a regulator *and* the press. You have 90 minutes before
a board call. Draft:
- 1-page board briefing (what happened, what is contained, what is
  not, what you are asking the board to approve)
- Internal all-hands note
- 30/60/90-day remediation plan with named owners
- Decision log template for the next 72 hours

**Exercise:** Board-level presentation on the state of AI governance.
See `exercises/exercise-05-presentation.md`.

**Deliverable:** Board-ready deck (10-15 slides) on the current state
of the organization's AI governance program, reviewed with a peer
using the "so what?" test at every slide.

---

## Case Studies

### Case Study 1: EU AI Act Operationalization at a Global Enterprise

**Background:**
- Global organization (financial services, retail, or industrial —
  choose) operating in all EU member states
- Mixed AI portfolio: in-house traditional ML, in-house GenAI
  applications, embedded vendor AI, foundation-model APIs
- Existing operational-risk, model-risk, privacy, and security
  programs — none built for AI
- EU AI Act phased obligations coming into force on a known schedule
  <!-- needs-research: cite the current phased-entry-into-application
  dates for EU AI Act obligations -->

**Your Role:** Senior AI infrastructure architect, chairing (or
co-chairing with General Counsel) the AI governance committee.

**Assignment:**
1. Classify the existing AI portfolio into AI Act risk tiers; defend
   the classifications
2. Identify where the organization is acting as provider, deployer,
   importer, or distributor — and show why these roles co-exist for
   the same model in different contexts
3. Map AI Act obligations onto an existing control framework (NIST
   AI RMF or ISO 42001) rather than building a parallel one
4. Design the operating model (committee, 2nd-line team structure,
   assurance line) for ongoing compliance

**Deliverables:**
- Portfolio classification memo with rationale (10 pages)
- Role-mapping matrix (provider / deployer / importer / distributor
  × model × jurisdiction)
- Controls crosswalk (AI Act articles → internal controls)
- Operating-model proposal (committee charter, roles, cadence)

**Success Criteria:**
- Classifications defensible to external counsel
- No controls counted twice (same obligation satisfied by one
  control, evidence reused across audits)
- Operating model can survive a leadership change

---

### Case Study 2: SR 11-7 Extended to Generative AI

**Background:**
- U.S. bank with a mature SR 11-7 model risk management program
- Business lines deploying GenAI for customer-facing use (contact
  center summarization, draft credit-decision explanations,
  marketing personalization)
- Model Risk Management (MRM) team argues GenAI is "out of scope"
  of SR 11-7; the regulator disagrees
  <!-- needs-research: cite public supervisory communications from
  Federal Reserve / OCC on GenAI and SR 11-7 scope -->

**Your Role:** Senior architect partnering with the Chief Model Risk
Officer to extend MRM to GenAI.

**Assignment:**
1. Map SR 11-7 pillars (model development, model implementation,
   model use, model validation, ongoing monitoring, governance)
   onto a GenAI use case
2. Identify where the existing MRM process fits and where it breaks
   (non-deterministic outputs, prompt sensitivity, system-prompt
   changes as model changes, retrieval context as model input)
3. Propose a GenAI-specific validation protocol as an *extension*
   of SR 11-7, not a replacement

**Deliverables:**
- SR 11-7 gap analysis for GenAI (10 pages)
- Proposed GenAI validation protocol
- Transition plan for existing GenAI pilots

**Success Criteria:**
- Credible to the bank's primary federal regulator
- Credible to an external auditor
- Does not stall business delivery that was already approved under
  existing frameworks

---

### Case Study 3: Standing Up Governance in a GenAI-First Company

**Background:**
- 400-person company whose entire product is a foundation-model-
  powered application
- No existing ERM, MRM, or privacy program at enterprise maturity
- Investors and prospective enterprise customers are asking for an
  ISO 42001 roadmap, SOC 2 report with AI controls, and written
  responsible-AI documentation
- Engineering leadership views governance as a growth tax

**Your Role:** Senior architect reporting to the CTO, with a dotted
line to a newly hired Chief Trust Officer.

**Assignment:**
1. Design a governance program sized for a 400-person company
   (the enterprise-scale version will kill velocity and credibility)
2. Pick one anchor framework (NIST AI RMF or ISO 42001) and defend
   the choice given customer and investor pressure
3. Build the minimum viable committee, policy, standard, and
   evidence structure
4. Sequence the program so the first six months produce artifacts
   that actually close enterprise deals

**Deliverables:**
- Right-sized operating-model memo (5 pages)
- Minimum viable policy + standard + implementation pattern
- 12-month roadmap tied to specific customer-facing outcomes
- Objection-handling playbook for engineering leadership

**Success Criteria:**
- Program is defensible in a customer security review
- Engineering sees the program as enabling, not blocking
- Path to ISO 42001 or SOC 2 + AI is clear without pre-committing
  to an expensive audit before it would pay off

---

## Exercises and Activities

The five exercises in `exercises/` are structured so each one feeds
the next. Treat them as a sequence, not a menu.

### Exercise 1: Case Study Analysis (3 hours)
Find a published case (HBR, Harvard, Stanford, NIST, ISO, regulator
enforcement action) on enterprise AI governance. Summarize, critique
trade-offs, and apply three lessons to your own organization.
See `exercises/exercise-01-case-study.md`.

### Exercise 2: 1-Page Strategy Memo (3 hours)
Write a 1-page memo to your CEO, CRO, or board chair on a specific
governance investment — e.g., stand up a model inventory, extend MRM
to GenAI, adopt ISO 42001 as the anchor framework, create a Chief AI
Risk Officer role. TL;DR, current state, recommendation, ask, risks.
See `exercises/exercise-02-strategy-memo.md`.

### Exercise 3: Stakeholder Map + Influence Plan (4 hours)
Map sponsors, supporters, neutrals, and blockers across General
Counsel, CRO, CISO, CPO, Head of Compliance, Chief Data Officer,
business-unit leaders, and internal audit. Convert to a 90-day
engagement plan with sequenced conversations.
See `exercises/exercise-03-stakeholder-mapping.md`.

### Exercise 4: 3-Year Governance Roadmap (5 hours)
Draft a 3-year roadmap for the enterprise AI governance program,
broken into quarterly milestones. Each phase: success metrics,
investment, key deliverables, and the specific control coverage
delta over the prior quarter.
See `exercises/exercise-04-roadmap.md`.

### Exercise 5: Board-Level Presentation (5 hours)
A 10-slide deck for a board risk committee on the current state and
forward plan of the AI governance program, reviewed with a peer
using the "so what?" test at every slide.
See `exercises/exercise-05-presentation.md`.

---

## Assessment

### Module Quiz

Short strategic-thinking questions — no crisp right answers, defend
your position. See `quiz.md` for the full prompt list.

### Strategic Governance Portfolio (8-10 hours)

A single coherent artifact set built around *one* governance program
you would design for a real (or realistic composite) organization:

1. **1-page AI policy** (board-approvable)
2. **3-5 page AI standard** (CIO/CRO-approvable, testable)
3. **1 implementation pattern or control specification** (engineering-
   consumable)
4. **Regulatory crosswalk** (internal controls × external regimes)
5. **Stakeholder map + 90-day engagement plan**
6. **Board-level status deck** (10-12 slides)

All six artifacts must describe the *same* governance program and
must be internally consistent. A reviewer should be able to spot-
check any two and find the same core framework, the same risk
tiering, and the same control vocabulary.

**Evaluation Criteria:**
- **Internal coherence** (25%) — policy, standard, and control
  speak the same vocabulary
- **Regulatory fit** (20%) — crosswalk shows real coverage, not
  marketing crosswalks
- **Audit-ready evidence posture** (15%) — a reviewer can see how
  compliance would be proven
- **Executive communication** (15%) — board deck is answer-first
- **Stakeholder strategy** (15%) — pre-wiring plan is credible
- **Right-sizing** (10%) — the program fits the organization,
  neither theater nor overreach

---

## Resources

### Required Reading

1. **Primary standards and frameworks**
   - NIST AI 100-1 — *Artificial Intelligence Risk Management
     Framework (AI RMF 1.0)*
   - NIST AI 600-1 — *Generative AI Profile*
   - ISO/IEC 42001:2023 — *Information technology — Artificial
     intelligence — Management system*
   - EU AI Act (consolidated text, Official Journal)
     <!-- needs-research: lock the citation to the published OJ
     reference -->

2. **Foundational articles and guidance**
   - SR 11-7 / OCC 2011-12 — "Guidance on Model Risk Management"
   - IIA: *The Three Lines Model* (2020 update)
   - Mitchell et al., "Model Cards for Model Reporting" (FAT* 2019)
   - Gebru et al., "Datasheets for Datasets"

### Supplementary Resources

- COSO: *Enterprise Risk Management — Integrating with Strategy
  and Performance*
  <!-- needs-research: confirm current edition and any AI
  supplement -->
- FDA — AI/ML-enabled SaMD action plan and PCCP guidance
- EEOC — guidance on algorithmic hiring tools
- NYC Local Law 144 — automated employment decision tools
- Partnership on AI, OECD AI Principles, G7 Hiroshima AI Process
  outputs — for international framing

See also `resources.md` in this module for the running reading
list.

---

## Next Steps

Upon completing MOD-403, you will be prepared to:

1. **Charter and chair** an enterprise AI governance committee
2. **Translate** EU AI Act, NIST AI RMF, ISO 42001, and sectoral
   rules into a single internal control framework
3. **Design and defend** a three-lines-of-defense model for AI risk
4. **Govern** model, data, and third-party AI with audit-grade
   evidence
5. **Brief** a board on AI governance posture without burying the
   lede
6. **Progress to MOD-404**: Innovation and R&D Leadership

---

**Ready to begin?** Start with Week 1: Governance Operating Model.

## Cross-references
- Engineering-level prerequisite: see ai-infra-engineer-learning + ai-infra-senior-engineer-learning
- Solutions repo: ai-infra-senior-architect-solutions/modules/mod-403-enterprise-governance
