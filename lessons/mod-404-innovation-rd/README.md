# MOD-404: Innovation and R&D Leadership

**Level**: Senior Architect (Strategic / Executive)
**Duration**: 35-50 hours
**Prerequisites**: Architect-level experience; mod-401 (Enterprise AI Strategy); mod-402 (Executive Leadership) and mod-403 (Enterprise Governance) recommended

## Module Overview

This module is part of the Senior AI Infrastructure Architect curriculum
(level 400). Focus: innovation and R&D.

Senior-architect modules emphasize executive communication, strategic
thinking, and organizational influence — not hands-on implementation.
For hands-on technical material on related topics (experiment tracking,
model evaluation harnesses, training infrastructure), see the
engineer-level and senior-engineer-level repos.

### Executive Summary

MOD-401 taught you to *build* a strategy, MOD-402 to *carry* it, and
MOD-403 to *govern* what you ship. MOD-404 is the other half of the
senior architect's job — building the engine that produces the *next*
generation of what you ship. Enterprise AI is defined less by what the
organization can do today than by whether its R&D pipeline can keep
pace with a field that resets every eighteen months.

At this level, innovation is not a lab, a hackathon, or a stage of the
funnel. It is a managed portfolio with four parts that must all exist
simultaneously: a **horizon-balanced portfolio** (near-term delivery
alongside multi-year bets), a **research-to-production pipeline** (how
a promising result crosses from a notebook to a regulated product), an
**intellectual-property and partnership posture** (what you own, what
you share, with whom), and an **innovation operating cadence** (how
leadership kills, continues, or scales a bet without turning the lab
into a product team or the product team into a lab). A program with
three of the four produces either demo-ware that never ships, or a
product organization that cannot renew itself.

By the end of this module, you will be able to:

- Design and defend an enterprise AI R&D portfolio across horizons
  (H1 extend, H2 build, H3 explore) tied to a CFO-credible funding
  model
- Apply disciplined selection frameworks (Heilmeier catechism,
  stage-gate, DARPA-style program construction) to AI research bets
- Stand up a research-to-production pipeline that moves promising
  results across the "valley of death" without destroying scientific
  rigor
- Govern IP, open-source contribution, publication, and research
  partnerships at enterprise scale
- Communicate innovation performance to a board and CFO using
  leading indicators, not vanity demos
- Build an innovation culture that survives after the founding sponsor
  moves on

---

## Learning Objectives

### Innovation Portfolio and Horizon Planning

1. **Three-horizon portfolio design**
   - Horizon 1 (H1): extend the current product — predictable return,
     short cycle, cost-of-not-doing-it logic
   - Horizon 2 (H2): build the next business — believable path,
     multi-year, measurable milestones
   - Horizon 3 (H3): explore the frontier — small, cheap, numerous
     bets with explicit kill criteria
   - Rebalance the mix annually; a portfolio drifting entirely to H1
     is a dying business, one drifting to H3 is a prospectus
     <!-- needs-research: cite Baghai, Coley, White (The Alchemy of
     Growth) and any current McKinsey R&D survey on realistic horizon
     mix percentages for established enterprises -->

2. **Selection and prioritization**
   - The Heilmeier Catechism (DARPA) as the project-pitch discipline:
     what are you trying to do, how is it done today, what is new,
     who cares, what are the risks, how much will it cost, how long
     will it take, what are the mid-term and final exams for success
     <!-- needs-research: cite the canonical DARPA / Heilmeier source
     for the catechism rather than secondary summaries -->
   - Expected-value framing for research bets (probability of success
     × value if successful × portfolio correlation discount)
   - Weighted shortest job first, bang-for-buck, and real-options
     thinking adapted for research spend

3. **Kill criteria and portfolio hygiene**
   - Pre-committed kill criteria at each stage — what would make us
     stop, decided *before* the result comes in
   - Sunk-cost audits and the "second compound-interest problem"
     (researchers who cannot be reassigned accumulate dead portfolio)
   - The difference between killing a project and killing a person's
     career, and why the second is the reason the first does not
     happen

### Research-to-Production Pipeline

4. **The valley of death**
   - Why research results die on the way to production — data
     plumbing, latency, cost, evaluation generality, operational
     ownership, regulatory classification
   - The handoff model that fails (toss over the wall) vs. the
     embedded model (research engineer rotates with the product team)
   - Dual-track delivery: discovery and delivery as parallel,
     coupled tracks rather than serial phases

5. **Stage gates for AI R&D**
   - Stage-Gate (Robert Cooper) adapted for AI/ML: idea → feasibility
     → prototype → pilot → productionization → scale
     <!-- needs-research: confirm whether Cooper has published an
     AI-specific adaptation and cite if so -->
   - Evidence required at each gate (benchmark, ablation, offline
     eval, online eval, shadow deployment, cost-per-unit, safety
     signoff)
   - Gate decisions as portfolio decisions, not just individual
     project decisions — the budget freed by killing one bet is
     already pre-committed to the next

6. **Measuring research throughput**
   - Lead time from idea to validated production impact
   - Experiment velocity and experiment "coverage" (the fraction of
     hypothesized improvements actually tested)
   - Reproducibility rate (fraction of positive internal results
     that replicate in a different team's hands)
   - Research-to-ship ratio (what proportion of funded bets ship
     and survive six months post-launch)

### Open vs. Closed Innovation

7. **Open innovation strategy**
   - Chesbrough's open-innovation thesis: valuable ideas enter and
     leave the firm through many channels; the boundary is permeable
     by design
     <!-- needs-research: anchor citations to Chesbrough's original
     book / HBR article rather than paraphrased summaries -->
   - The spectrum: internal-only research, consortia, joint ventures,
     academic collaborations, open-source contribution, standards
     participation, external challenges and prizes

8. **Research partnerships**
   - Academic partnerships — university labs, endowed chairs, visiting
     researcher programs, sponsored PhD programs
   - National-lab and government partnerships (DOE labs, DARPA
     programs, EU Horizon Europe, UKRI)
     <!-- needs-research: refresh the list of currently active major
     AI-relevant public programs at time of use -->
   - Industry consortia (MLCommons, LF AI & Data, Partnership on AI)
     and when a consortium is a genuine force-multiplier vs. a logo
     wall

9. **Open-source and publication posture**
   - Contributing to and consuming from open-source AI ecosystems as
     a deliberate strategy, not a side effect
   - Publication policy — what the research team may publish, what
     reviews are required, how publication interacts with patent and
     trade-secret strategy
   - Weight-release decisions (open weights, gated weights,
     API-only) as a product and risk decision as much as a
     research decision

### Intellectual Property and Competitive Moat

10. **IP strategy for AI**
    - What is actually patentable in AI (methods, architectures,
      training techniques, inference systems) vs. what is better
      kept as trade secret
      <!-- needs-research: confirm current USPTO, EPO, and UK IPO
      guidance on AI-invention patentability and inventorship -->
    - Data as a moat — proprietary training data, feedback loops,
      and the "data flywheel" as the real competitive asset for most
      enterprises
    - Model weights, prompts, and system prompts as protectable
      assets — what works as trade secret, what travels when people
      do
    - Freedom-to-operate analysis for AI (training data provenance,
      model lineage, third-party model terms)

11. **Foundation-model era IP questions**
    - Training-data copyright exposure and the state of litigation
      <!-- needs-research: assemble a current reading list of the
      major foundation-model training-data lawsuits, their stage,
      and any decided holdings -->
    - Output ownership and the user-content question
    - IP indemnification from model vendors (what it actually covers,
      what the caps are, and when it is worth the premium)
    - Patent landscaping as a defensive discipline

### Innovation Operating Model and Culture

12. **Where the lab sits**
    - Central corporate research lab (Bell Labs, PARC, IBM Research,
      Microsoft Research) — pros, failure modes
    - Embedded research inside product lines — faster, narrower,
      harder to compound
    - Hybrid models: central platform research + embedded applied
      research with rotation
    - Skunkworks and "garage" structures — when they work and when
      they signal that the main organization is broken
    - "Google X" and other moonshot factories — the economics of
      graduation and shutdown as the product

13. **Talent and incentives**
    - Dual career ladders (researcher track vs. engineer track vs.
      manager track) and compensation design that lets a principal
      researcher earn at the level of a senior director
    - Publication and conference policy as a recruiting tool
    - Rotation programs between research and product as talent
      development *and* technology transfer
    - The "research director's dilemma" — hiring for breakthroughs
      while delivering a quarterly roadmap

14. **Innovation metrics the board will actually read**
    - Leading indicators: idea pipeline volume, stage-gate
      throughput, experiment velocity, reproducibility rate
    - Lagging indicators: revenue from products <3 years old,
      competitive patents cited, external recognition
    - Cost indicators: R&D intensity, cost per published advance,
      research compute efficiency
    - Vanity metrics to avoid: raw patent counts, paper counts,
      demo counts, hackathon counts

---

## Module Structure

```
mod-404-innovation-rd/
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

### Week 1: Portfolio and Horizon Design (6 hours)

**Topics:**
- The three-horizon model and why the "right" mix is organization-
  specific, not a template
- Framing an AI R&D portfolio as managed risk, not managed demos
- The Heilmeier Catechism as the standing pitch discipline for every
  new research initiative
- Expected-value, real-options, and weighted-shortest-job-first
  framings for R&D prioritization
- Failure modes: the H1-only trap, the H3-only trap, and the "all
  H2, no graduation" trap

**Readings:**
- Baghai, Coley, White — *The Alchemy of Growth* (horizon framework,
  selected chapters)
  <!-- needs-research: confirm a specific edition / chapter citation -->
- The Heilmeier Catechism — DARPA primary source
- Clayton Christensen — *The Innovator's Dilemma* (selected chapters
  on disruption and resource allocation)
- Geoffrey Moore — *Zone to Win* (managing innovation across the
  performance, productivity, incubation, and transformation zones)

**Exercise:** Classify your organization's current AI initiatives into
H1/H2/H3 and compute the actual spend mix. Is the mix defensible to
the CFO? See `exercises/exercise-01-case-study.md` for a structured
version.

---

### Week 2: Selecting, Funding, and Killing Research Bets (8 hours)

**Topics:**
- Running the Heilmeier Catechism as a chartering ritual, not a
  one-time filter
- Pre-committed kill criteria — why they are the only reliable
  antidote to sunk-cost portfolio drift
- Stage-gate design for AI/ML: what evidence crosses each gate,
  who is the decision-maker, who has the veto
- Funding models: central R&D budget, internal venture fund,
  business-unit cross-charges, and the trade-offs of each
- Research compute as a budget line — how capacity planning for
  training clusters differs from production capacity planning
  <!-- needs-research: cite public sources on frontier-training
  compute costs and implied R&D-intensity benchmarks -->

**Readings:**
- Robert G. Cooper — *Winning at New Products* (Stage-Gate)
  <!-- needs-research: confirm current edition -->
- Steve Blank — *The Four Steps to the Epiphany* (customer
  discovery as a research discipline)
- Rita McGrath — *Discovery-Driven Planning* (HBR, 1995)
- Gary Klein, HBR: "Performing a Project Premortem" (also appears
  in MOD-402; here used for research-bet pre-mortems)

**Case Study:** A 50-researcher AI R&D org spends $80M/year and
ships two products in three years. You are asked to triple
research-to-ship ratio without growing headcount. What do you keep,
kill, or re-charter? Design the stage-gate review, the kill criteria,
and the first quarterly portfolio review. See
`exercises/exercise-02-strategy-memo.md`.

**Deliverable:** A one-page portfolio memo: current mix (H1/H2/H3),
proposed mix, three specific stop/start/continue decisions with
defended reasoning, and the leading indicators you will show the CFO
in 90 days.

---

### Week 3: The Research-to-Production Pipeline (8 hours)

**Topics:**
- The "valley of death" in AI specifically — what causes most
  promising results to never ship (data plumbing, eval generality,
  latency, cost-per-call, operational ownership, regulatory
  classification)
- Dual-track delivery: discovery track and delivery track running
  in parallel with explicit coupling, not a research-then-engineering
  waterfall
- The handoff anti-pattern vs. embedded-researcher and
  researcher-rotation models
- Platform as the compound-interest instrument: shared training
  infrastructure, evaluation harnesses, feature stores, and model
  registries that make the Nth bet cheaper than the first
- The interaction with governance (MOD-403) — how research artifacts
  become audit-ready model-inventory entries at productionization

**Readings:**
- Marty Cagan — *Inspired* and *Empowered* (product discovery and
  dual-track delivery)
- Jeff Patton — *User Story Mapping* (dual-track discovery origin)
- *Accelerate* — Forsgren, Humble, Kim (flow, lead time, batch size
  — read as applied to research throughput, not just delivery)
- Published research-to-production retrospectives from large AI labs
  <!-- needs-research: select 2-3 primary-source engineering-blog
  posts (DeepMind, Google Research, Meta AI, etc.) documenting a
  specific research-to-production transition -->

**Exercise:** Draft a one-page memo to the CTO proposing a
research-to-production pipeline for the organization. Include the
coupling points to the governance program from MOD-403 and the
funding model from Week 2. See `exercises/exercise-02-strategy-memo.md`.

**Deliverable:** A two-artifact set on the *same* R&D program:
- 1-page research-to-production charter (CEO/CTO-readable)
- 3-5 page operating spec (platform + process, engineering-leadership-
  readable)

Each must trace to the other. A reviewer should be able to walk from
charter commitment → operating-spec control without jumping gaps.

---

### Week 4: Open Innovation, Partnerships, and the IP Posture (10 hours)

**Topics:**
- Chesbrough's open-innovation model and the firm as a permeable
  boundary, not a fortress
- Academic partnerships: endowed chairs, sponsored research
  agreements, visiting-faculty programs, PhD sponsorships, and
  what each actually buys
- National-lab and government partnerships — the funding leverage
  and the strings attached (export control, security clearance,
  publication delay)
- Industry consortia (MLCommons, LF AI & Data, Partnership on AI,
  standards bodies) as force multipliers and political venues
- Open-source and publication strategy as recruiting, as technology
  transfer, and as competitive signaling — all three at once
- IP strategy: what to patent, what to keep as trade secret, what
  to publish, and how those three decisions interact

**Readings:**
- Henry Chesbrough — *Open Innovation: The New Imperative for
  Creating and Profiting from Technology*
- Jon Gertner — *The Idea Factory: Bell Labs and the Great Age of
  American Innovation* (the canonical central-research-lab case)
- Douglas Smith & Robert Alexander — *Fumbling the Future: How
  Xerox Invented, Then Ignored, the First Personal Computer* (PARC
  as the canonical graduation-failure case)
- WIPO — selected materials on AI and intellectual property
  <!-- needs-research: cite the current WIPO AI-and-IP resource
  page or policy brief -->
- Primary-source AI training-data litigation trackers
  <!-- needs-research: identify a credible, continuously updated
  tracker and cite it rather than news summaries -->

**Case Study:** Your organization is asked to co-found a pre-
competitive industry consortium on AI evaluation standards with four
direct competitors. General Counsel is nervous about antitrust
exposure; the CTO is worried about giving away the eval playbook;
the CEO sees a PR win. Draft the decision memo. See
`exercises/exercise-03-stakeholder-mapping.md`.

**Deliverable:** Stakeholder map + 90-day engagement plan for one
real or realistic external-partnership decision (consortium,
foundation-model alliance, academic lab, government program, or
open-source stewardship).

---

### Week 5: Innovation Operating Model, Talent, and Culture (10 hours)

**Topics:**
- The operating-model choice: central lab, embedded applied
  research, hybrid with rotation, skunkworks, standalone moonshot
  venture — each has a historical track record and a known failure
  mode
- Bell Labs, PARC, IBM Research, Microsoft Research, DeepMind,
  OpenAI, Anthropic, Meta AI as operating-model case studies
  <!-- needs-research: verify current lab structures and recent
  reorganizations before relying on these as live examples -->
- Dual career ladders and compensation design — making the
  researcher-track distinguished engineer a credible career
  destination
- Rotation programs between research and product as *both* talent
  development *and* the main technology-transfer mechanism
- Publication policy, conference attendance, external talks, and
  sabbatical programs as recruiting tools and as retention tools
- The "founder's lab" problem — innovation culture that depends on
  one executive sponsor and collapses when that sponsor leaves

**Readings:**
- Jon Gertner — *The Idea Factory*
- Safi Bahcall — *Loonshots: How to Nurture the Crazy Ideas That
  Win Wars, Cure Diseases, and Transform Industries*
- Ed Catmull — *Creativity, Inc.* (Pixar's approach to sustained
  creative output inside a disciplined operation)
- Peter Sims — *Little Bets* (small, numerous, cheap experiments)
- Will Larson — *Staff Engineer* (dual-ladder and research-engineer
  archetype)

**Exercise:** 3-year innovation roadmap: pick an operating-model
target (central lab, hybrid, embedded + platform, moonshot shop) and
sequence quarterly milestones to reach it from wherever the
organization is today. See `exercises/exercise-04-roadmap.md`.

**Deliverable:** Innovation roadmap (15-20 pages) covering:
- Current-state assessment (headcount, spend, horizon mix, recent
  research-to-ship ratio, stage-gate throughput, external profile)
- Target end-state tied to a chosen operating model
- Quarterly milestones with leading indicators
- Talent and compensation plan
- Risk register for innovation-program-specific risks (brain drain,
  sponsor loss, portfolio drift, graduation failure)

---

### Week 6: Communicating Innovation to the Board (6 hours)

**Topics:**
- What the board actually needs on innovation — leading indicators
  over demo reels; cost discipline over paper counts; graduation
  outcomes over launch volume
- The one-page innovation portfolio view — horizons, bets, stage,
  kill/continue/scale decisions in the quarter
- Separating the *science* story (what we learned) from the
  *product* story (what we shipped) from the *finance* story (what
  we spent to get there)
- Communicating a visible research failure — how to kill a public
  bet without poisoning the next one
- The board AI committee and where innovation reporting fits

**Readings:**
- Gary Pisano — HBR: "You Need an Innovation Strategy"
- *The Pyramid Principle* — Barbara Minto (reinforced from MOD-402
  for the board-facing format)
- Published board-level innovation disclosures from public AI-
  heavy companies (10-K R&D sections, investor-day decks)
  <!-- needs-research: assemble a short reading list of current
  public disclosures to study as examples -->

**Scenario:** The organization's most visible H2 bet — a
foundation-model-powered product your CEO personally championed —
has missed its second stage-gate and is burning $40M/year with no
line of sight to revenue. You have 90 minutes before a board
innovation-committee call. Draft:
- 1-page board briefing (what we learned, what we are asking the
  board to approve: kill, pivot, or re-charter)
- Internal all-hands note (framing for the team)
- 30/60/90-day plan under each of the three options
- Decision log template for the committee discussion

**Exercise:** Board-level presentation on the state of AI
innovation and R&D. See `exercises/exercise-05-presentation.md`.

**Deliverable:** Board-ready deck (10-15 slides) on the current
state of the organization's AI innovation portfolio, reviewed with
a peer using the "so what?" test at every slide.

---

## Case Studies

### Case Study 1: Portfolio Reset at a Mature Enterprise

**Background:**
- Fortune 200 organization with a 15-year-old AI/ML research group
- Historical output: strong academic publication record, modest
  product impact
- Board and new CEO ask: "what have we gotten for the $600M we have
  spent?"
- Three horizons are present on paper; actual spend is >85% H1
  maintenance work rebranded as research
- No stage-gate, no kill criteria, no research-to-ship metric

**Your Role:** Senior AI infrastructure architect, newly appointed
to chair an R&D operating-committee alongside the Chief Scientist
and Chief Product Officer.

**Assignment:**
1. Produce a defensible current-state assessment (headcount, spend,
   actual horizon mix, research-to-ship ratio over the last 36
   months)
2. Propose a target mix and the stage-gate / kill-criteria
   discipline required to reach it
3. Design a 12-month transition plan that re-charters existing
   projects into H1/H2/H3 buckets and sunsets or graduates the
   portfolio tail
4. Protect the organization from an obvious failure mode: an
   indiscriminate layoff dressed as "portfolio hygiene"

**Deliverables:**
- Current-state assessment (10 pages)
- Target-state portfolio memo (3-5 pages)
- 12-month transition plan with quarterly milestones
- Communications plan (internal + board)

**Success Criteria:**
- Current-state assessment is reproducible from primary data
- Portfolio target survives a CFO's five-year-cost projection
- Transition plan preserves core scientific talent and signals a
  credible research future

---

### Case Study 2: Standing Up a Foundation-Model Research Program

**Background:**
- Global software company competing with three vendors that have
  public foundation-model programs
- Existing applied-ML organization is strong; frontier-model
  capability is absent
- Options on the table: (a) build an internal frontier-training
  program, (b) deepen a foundation-model-vendor alliance, (c) found
  a jointly funded research consortium, (d) acquire a research
  lab
  <!-- needs-research: refresh the list of recent large AI-lab
  acquisitions / acqui-hires with publicly disclosed structures -->
- Board is willing to commit a multi-year R&D investment but wants
  a defensible answer on "build vs. partner vs. buy"

**Your Role:** Senior AI infrastructure architect, chartered with
delivering the board recommendation jointly with the Chief
Scientist and the Head of Corporate Development.

**Assignment:**
1. Frame the decision in Heilmeier-catechism form for each of the
   four options
2. Build the expected-value / real-options analysis — including
   graduation and shutdown economics
3. Lay out the IP, compute, data, talent, and partnership
   dependencies for the recommended option
4. Design the operating model and board-level oversight cadence
   that would accompany the chosen path

**Deliverables:**
- Four Heilmeier-form pitches (one per option, 2 pages each)
- Comparative expected-value analysis
- Board recommendation memo (6 pages, Amazon-narrative style)
- Operating-model and oversight charter for the chosen path

**Success Criteria:**
- Recommendation is defensible under a CFO challenge on multi-year
  TCO and under a General-Counsel challenge on IP and partnership
  structure
- The shutdown / exit path for the recommended option is specified
  up front
- The recommendation survives at least one organizational-leadership
  change before its first stage gate

---

### Case Study 3: The Visible Failure

**Background:**
- 3-year-old moonshot inside a well-known enterprise
- Deep public commitment by the CEO; press coverage at launch
- Two missed stage gates; a third would normally trigger kill
  criteria that were agreed to (in writing) at chartering
- Project lead is a tenured principal researcher with a strong
  external profile and a loyal team
- Killing the project triggers press coverage and risks a visible
  retention event; continuing triggers a CFO escalation and
  undermines the stage-gate discipline you have spent two years
  building

**Your Role:** Senior architect chairing the R&D operating
committee. The CEO has delegated the call to the committee.

**Assignment:**
1. Apply the pre-committed kill criteria honestly — document the
   evidence and the gap
2. Design three decision options (kill, pivot, re-charter) with
   30/60/90-day plans under each
3. Pre-wire the decision across the CEO, CFO, Chief Scientist,
   General Counsel, and the project lead before the committee
   meets
4. Produce the board communication under the chosen option

**Deliverables:**
- Evidence memo against the stage-gate criteria
- Three-option decision brief (3 pages)
- Stakeholder pre-wiring plan with sequenced conversations
- Board-facing communication under the chosen option
- Internal all-hands framing

**Success Criteria:**
- The decision is defensible against the pre-committed criteria,
  not against ex-post rationalization
- The stage-gate discipline survives the decision intact
- The project lead and core team remain credible contributors to
  the next bet, whatever the call is

---

## Exercises and Activities

The five exercises in `exercises/` are structured so each one feeds
the next. Treat them as a sequence, not a menu.

### Exercise 1: Case Study Analysis (3 hours)
Find a published case (HBR, Harvard, Stanford, MIT, or a primary-
source research-lab retrospective) on enterprise AI innovation or on
a historical corporate research lab. Summarize, critique trade-offs,
and apply three lessons to your own organization.
See `exercises/exercise-01-case-study.md`.

### Exercise 2: 1-Page Strategy Memo (3 hours)
Write a 1-page memo to your CEO, CTO, or board chair on a specific
innovation investment — e.g., stand up a frontier-model research
program, kill the AI moonshot, adopt a stage-gate for all R&D above
a threshold, open-source the evaluation harness. TL;DR, current state,
recommendation, ask, risks.
See `exercises/exercise-02-strategy-memo.md`.

### Exercise 3: Stakeholder Map + Influence Plan (4 hours)
Map sponsors, supporters, neutrals, and blockers across CEO, CFO,
Chief Scientist / CTO, General Counsel, Chief Product Officer,
business-unit leaders, and the external academic / partner
community. Convert to a 90-day engagement plan with sequenced
conversations.
See `exercises/exercise-03-stakeholder-mapping.md`.

### Exercise 4: 3-Year Innovation Roadmap (5 hours)
Draft a 3-year roadmap for the enterprise AI innovation program,
broken into quarterly milestones. Each phase: success metrics,
investment, portfolio-mix target, stage-gate throughput target, and
graduation outcomes.
See `exercises/exercise-04-roadmap.md`.

### Exercise 5: Board-Level Presentation (5 hours)
A 10-slide deck for a board innovation committee on the current state
and forward plan of the AI R&D portfolio, reviewed with a peer using
the "so what?" test at every slide.
See `exercises/exercise-05-presentation.md`.

---

## Assessment

### Module Quiz

Short strategic-thinking questions — no crisp right answers, defend
your position. See `quiz.md` for the full prompt list.

### Strategic Innovation Portfolio (8-10 hours)

A single coherent artifact set built around *one* innovation program
you would design for a real (or realistic composite) organization:

1. **1-page innovation strategy memo** (board-approvable)
2. **Portfolio design** (H1/H2/H3 with bets, spend, and kill
   criteria)
3. **Research-to-production operating spec** (3-5 pages,
   engineering-leadership-consumable)
4. **Partnership and IP posture memo** (what we build, what we
   partner on, what we publish)
5. **Stakeholder map + 90-day engagement plan**
6. **Board-level status deck** (10-12 slides)

All six artifacts must describe the *same* innovation program and
must be internally consistent. A reviewer should be able to spot-
check any two and find the same horizons, the same bets, and the
same operating-model assumptions.

**Evaluation Criteria:**
- **Internal coherence** (25%) — memo, portfolio, operating spec,
  and board deck tell the same story at every altitude
- **Portfolio discipline** (20%) — horizons, kill criteria, and
  stage gates are credible, not decorative
- **Research-to-ship realism** (15%) — the pipeline survives first
  contact with data, latency, cost, and governance constraints
- **Executive communication** (15%) — board deck is answer-first
- **Stakeholder strategy** (15%) — pre-wiring plan is credible,
  especially for the inevitable kill decisions
- **Right-sizing** (10%) — the program fits the organization,
  neither a cargo-culted Bell Labs nor a demo factory

---

## Resources

### Required Reading

1. **Books**
   - Baghai, Coley, White — *The Alchemy of Growth*
   - Henry Chesbrough — *Open Innovation*
   - Clayton Christensen — *The Innovator's Dilemma*
   - Robert G. Cooper — *Winning at New Products*
   - Jon Gertner — *The Idea Factory*
   - Safi Bahcall — *Loonshots*
   - Marty Cagan — *Inspired* and *Empowered*
   - Geoffrey Moore — *Zone to Win* (and *Crossing the Chasm* for
     adjacent framing)

2. **Foundational articles and primary sources**
   - George H. Heilmeier — the Catechism (DARPA primary source)
   - Rita McGrath, HBR: "Discovery-Driven Planning" (1995)
   - Gary Pisano, HBR: "You Need an Innovation Strategy"
   - Primary-source AI-lab engineering retrospectives on research-
     to-production transitions
     <!-- needs-research: select 3-5 current primary-source blog
     posts or papers -->

### Supplementary Resources

- Ed Catmull — *Creativity, Inc.*
- Steve Blank — *The Four Steps to the Epiphany*
- Peter Sims — *Little Bets*
- Will Larson — *Staff Engineer* (dual-ladder design)
- WIPO — AI and intellectual property policy materials
  <!-- needs-research: confirm current WIPO publication -->
- MLCommons, LF AI & Data, Partnership on AI — consortium materials
  as primary sources on current industry collaboration shape
- OECD and G7 Hiroshima AI Process outputs — for the international
  R&D policy framing

See also `resources.md` in this module for the running reading list.

---

## Next Steps

Upon completing MOD-404, you will be prepared to:

1. **Design and defend** a horizon-balanced AI R&D portfolio with
   credible kill criteria
2. **Charter and operate** a research-to-production pipeline tied
   to the governance program from MOD-403
3. **Decide** the organization's open-innovation, partnership, and
   IP posture with trade-offs made explicit
4. **Lead** an innovation operating model that survives sponsor
   turnover
5. **Brief** a board on innovation performance using leading
   indicators, not vanity demos
6. **Progress to MOD-405**: Responsible AI and Ethical Leadership

---

**Ready to begin?** Start with Week 1: Portfolio and Horizon Design.

## Cross-references
- Engineering-level prerequisite: see ai-infra-engineer-learning + ai-infra-senior-engineer-learning
- Solutions repo: ai-infra-senior-architect-solutions/modules/mod-404-innovation-rd
