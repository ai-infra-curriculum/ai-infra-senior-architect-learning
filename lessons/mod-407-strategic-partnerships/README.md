# MOD-407: Strategic Partnerships and Vendor Management

**Level**: Senior Architect (Strategic / Executive)
**Duration**: 35-50 hours
**Prerequisites**: Architect-level experience; mod-401 (Enterprise AI Strategy); mod-403 (Enterprise Governance) and mod-406 (Global Infrastructure) recommended

## Module Overview

This module is part of the Senior AI Infrastructure Architect curriculum
(level 400). Focus: strategic partnerships and vendor management.

Senior-architect modules emphasize executive communication, strategic
thinking, and organizational influence — not hands-on implementation.
For hands-on technical material on related topics (API integration,
SDK evaluation, benchmarking across vendors, cost tracking, egress
engineering), see the engineer-level and senior-engineer-level repos.

### Executive Summary

MOD-401 taught you to *build* a strategy, MOD-402 to *carry* it,
MOD-403 to *govern* what you ship, MOD-404 to produce the *next*
generation, MOD-405 to decide what the organization is willing to
deploy at all, and MOD-406 to place it on the physical and
jurisdictional map. MOD-407 asks the question the others have
treated as a given: *whose technology is in the stack, under what
terms, with what kill switches on either side, and what happens
when the counterparty's interests diverge from yours?*

At enterprise scale, an AI platform is not something an organization
builds — it is something an organization *assembles*, from a stack
of vendor relationships that each have their own economics, their
own regulatory exposure, their own concentration profile, and their
own answer to the question "who else do you sell this to?" A
production AI system in 2026 typically has at least four load-
bearing counterparties (a foundation-model vendor, a cloud and
compute vendor, a data vendor, and a systems-integration partner),
and often another three to five less visible ones (evaluation
providers, safety classifiers, embedding and retrieval vendors,
observability vendors, specialist agents). The senior architect's
job is to understand each of these as a *partnership* — not a
purchase — and to design the ecosystem so that the loss, abuse,
pricing shift, or regulatory capture of any single counterparty is
survivable.

At this level, strategic partnerships are a program with five parts
that must co-exist: a **partnership portfolio** (who the
organization is in business with, in what role, for what term, at
what depth), a **vendor evaluation and due-diligence discipline**
(how new counterparties are vetted before they become load-
bearing), a **contract architecture** (the standard clauses the
organization refuses to deploy an AI workload without, and the
negotiated-exception process for the ones it accepts), a
**partnership governance regime** (joint steering, escalation,
dispute resolution, review, renegotiation, exit), and an
**ecosystem posture** (whether the organization is primarily a
builder, a channel, a platform, or a marketplace for other
people's AI). A program with four of the five works until the
fifth is tested, and then it does not.

By the end of this module, you will be able to:

- Produce a defensible enterprise partnership portfolio that a
  CFO, CRO, Chief Trust Officer, and General Counsel can each sign
- Classify every load-bearing AI vendor relationship by role,
  substitutability, counterparty risk, and contractual posture
- Translate foundation-model licensing terms, hyperscaler
  enterprise agreements, and systems-integrator master-service
  terms into a build / partner / resell / decline decision for
  each capability area
- Negotiate the AI-specific clauses — model-input and model-
  output rights, training-data use, evaluation and red-team
  access, indemnification for third-party IP claims, residency
  and operator-access commitments, exit and transition rights —
  as a standing enterprise position rather than a per-deal
  invention
- Design a partnership governance model (joint steering,
  escalation, review cadence, renegotiation and exit triggers)
  that survives leadership change on either side
- Lead the organization through a partnership crisis — a vendor
  pricing shift, a strategic pivot, a security or trust incident,
  an acquisition of a critical supplier by a competitor, or a
  regulatory enforcement action against a counterparty
- Communicate partnership posture to a board, to a regulator,
  to a government customer, and to the organization's own
  workforce with the same vocabulary and the same numbers

---

## Learning Objectives

### The Partnership Ecosystem Map

1. **The AI-vendor stack as a layered dependency**
   - The foundation-model layer (frontier labs: OpenAI, Anthropic,
     Google DeepMind, Meta, Mistral, Cohere, xAI, DeepSeek,
     Alibaba Qwen, Baidu ERNIE; open-weights providers; vertical-
     specialist labs) and the way each layer participates in
     different partnership shapes (API, hosted, VPC-isolated,
     licensed-weights, custom-trained)
     <!-- needs-research: refresh the current frontier-lab list,
     their publicly disclosed hyperscaler affiliations, and their
     model-access and deployment-option matrices at time of use -->
   - The compute and cloud layer (hyperscalers, GPU-specialist
     clouds, sovereign-cloud operators) as covered in MOD-406,
     now read as *partnerships* rather than as infrastructure
   - The data layer (licensed corpus providers, synthetic-data
     vendors, evaluation-set providers, labeling and RLHF
     vendors) as the most under-governed partnership tier in
     most organizations
   - The platform and application layer (vector databases,
     retrieval and RAG platforms, agent frameworks, workflow
     orchestration, prompt-ops and evaluation vendors)
   - The systems-integration and services layer (large SIs,
     boutique AI implementation partners, specialist consultancies)

2. **Partnership roles and archetypes**
   - **Supplier** — a counterparty the organization buys from on
     standard commercial terms; low integration, replaceable with
     effort, governed by procurement
   - **Strategic vendor** — a counterparty with a multi-year
     commitment and a *named* joint working relationship; limited
     substitutability without migration cost
   - **Strategic partner** — a counterparty with a formal joint
     program, co-selling or co-development scope, and reputational
     linkage
   - **Alliance** — a formal, often publicly announced relationship
     with shared investment or equity, governance, and strategic
     direction
   - **Joint venture or co-founded entity** — a separate legal
     entity for a specific market, jurisdiction, or capability
   - The practical difference between these tiers is usually
     captured in three things: contractual commitment length,
     governance intensity, and whether leadership on either side
     is personally identified with the relationship

3. **The ecosystem role the organization plays**
   - **Builder** — the organization builds its own AI capabilities
     and buys only commodity inputs; partnerships are narrow and
     primarily procurement-managed
   - **Assembler** — the organization composes a product from
     partner components; partnerships are load-bearing and
     governed as such
   - **Channel** — the organization resells, implements, or
     white-labels partner AI; partner economics dominate
   - **Platform** — the organization hosts other people's AI
     capabilities on its own surface (marketplaces, agent stores,
     app galleries)
   - **Marketplace operator** — the organization is the economic
     intermediary between AI buyers and sellers, with governance
     and trust obligations to both sides
   - Most organizations are two of these at once; the failure
     mode is being three without having decided which

### Vendor Evaluation and Due Diligence at Enterprise Scale

4. **The AI-vendor due-diligence framework**
   - *Technical fit* — capability vs. requirement, benchmark and
     own-evaluation performance, roadmap alignment, integration
     surface, deployment-model options (API / dedicated /
     VPC / on-prem / licensed-weights)
   - *Financial* — funding stage and runway, revenue concentration,
     burn rate against commercial terms, acquisition exposure,
     insurance and indemnification capacity — AI vendors in 2026
     range from pre-revenue to trillion-dollar-market-cap, and
     the counterparty profile is the first filter
     <!-- needs-research: refresh the public funding and revenue
     disclosures for major frontier labs and AI-platform vendors
     at time of use -->
   - *Legal and regulatory* — IP posture on training data and
     model outputs, data-use and residency commitments, EU AI Act
     role (provider, deployer, authorised representative),
     sector-regulator exposure, pending litigation, open
     regulator investigations
   - *Security and trust* — SOC 2 Type II, ISO/IEC 27001,
     ISO/IEC 42001, FedRAMP tier, HIPAA readiness, penetration-
     test history, incident history, responsible-disclosure track
     record, operator-access controls
     <!-- needs-research: confirm current ISO/IEC 42001 certified
     AI vendors at time of use; the certified-population is
     growing but still small -->
   - *Operational* — uptime and incident history, documented RPO
     and RTO, change-management discipline, model-version
     policy, deprecation and sunset posture
   - *Strategic* — alignment of the vendor's own strategy with
     the organization's, overlap with competitors in the
     vendor's customer base, equity entanglements that affect
     neutrality, foreign-ownership and export-control exposure

5. **Model-vendor-specific diligence**
   - *Model provenance* — training-data sources, licensing
     posture, opt-out handling, removal-request handling, and
     the audit trail available to an enterprise buyer under
     GDPR, the EU AI Act Article 10 and Article 53, and emerging
     US state transparency obligations
     <!-- needs-research: refresh the EU AI Act GPAI training-
     data transparency template status (Code of Practice,
     implementing acts, AI Office guidance) at time of use -->
   - *Evaluation posture* — standardized benchmarks (MMLU, HELM,
     HumanEval, SWE-bench, MMMU, and successor suites), the
     vendor's own hazard and safety evaluations, third-party
     evaluation relationships, red-team program maturity, and
     the *vendor's willingness to let the buyer evaluate on
     buyer-provided data*
     <!-- needs-research: current state of leading public
     benchmarks and the frontier-model hazard-evaluation
     landscape (UK AISI, US AISI, METR, Apollo, Anthropic
     RSP-style disclosures, OpenAI preparedness reports,
     Google Frontier Safety Framework reports) -->
   - *Safety and trust & safety* — classifiers, usage policies,
     enforcement history, allowlist / blocklist semantics,
     region- and tenant-level policy options, incident
     notification commitments
   - *Fine-tuning and customization terms* — whether the model
     can be fine-tuned, on whose data, on whose hardware, with
     which rights on the resulting adapter / checkpoint, and
     whether those rights survive contract termination
   - *Deployment options* — public API, dedicated capacity,
     private deployment (hyperscaler VPC, on-prem, air-gapped),
     and the pricing / isolation / audit trade-offs across them
   - *Model-lifecycle commitments* — version freshness, backward-
     compatibility, deprecation notice period, long-lived
     endpoint availability, re-evaluation on version change

6. **Hyperscaler and compute-vendor-specific diligence**
   - Enterprise discount program structure (EDP for AWS, MACC
     for Azure, Google CUD / commits) and the way AI-specific
     consumption nests inside these umbrella commitments
     <!-- needs-research: refresh current EDP/MACC/CUD discount
     mechanics and AI-service-specific commit instruments at
     time of use -->
   - Reserved vs. on-demand vs. spot for accelerator inventory,
     and the way reserved commitments calcify a partnership
   - Capacity commitments — the de facto compute-reservation
     negotiation that now dominates AI-platform economics —
     including the question of *what capacity actually means*
     when the vendor cannot deliver silicon on the committed date
   - Data egress and inter-region transfer economics as a
     switching-cost lever, and the public and negotiated
     carve-outs available in 2026
   - Service-portability commitments (data egress waivers,
     model-portability clauses, inference-API-equivalence
     clauses) as the modern expression of "no lock-in"
   - Marketplace and co-sell participation — AWS Marketplace,
     Azure Marketplace, Google Cloud Marketplace — as both a
     distribution channel and a partnership instrument

7. **Systems-integrator and services-partner diligence**
   - The AI-services-partner market (large SIs with AI
     practices; boutique AI-native implementation firms;
     specialist consultancies with vertical depth) and the
     differences in operating model, pricing, and skin-in-the-
     game
   - Partner certification tiers across hyperscalers and model
     vendors — what "Premier Partner" or "Expert" actually
     means operationally, and the gap between the badge and
     the delivery team
   - Delivery-risk evaluation — reference calls, prior-project
     postmortems, on-site talent vs. offshore delivery, and the
     hidden-subcontractor problem
   - IP and deliverables — who owns the code, prompts,
     evaluations, and fine-tuned models produced in an
     engagement, and the standard clauses that contain the
     answer

### Contract Architecture for AI Partnerships

8. **The AI-specific clause set that distinguishes an AI vendor contract from a generic SaaS contract**
   - *Input rights* — what the vendor may do with customer
     prompts, documents, embeddings, and files; the
     "no training on customer inputs by default" baseline that
     is now table stakes; the opt-in and opt-out mechanics; the
     retention window and deletion commitments
   - *Output rights* — who owns the model output, whether it
     may be used commercially, whether the vendor can reuse
     outputs from the customer's workloads to train other
     customers' models (the "no cross-customer training" clause)
   - *Training-data warranties* — the vendor's representation
     that training data was lawfully sourced, licensed, and
     where applicable removed on opt-out; the specific
     limitations and carve-outs the vendor still insists on
   - *IP indemnification for third-party claims* — the "copyright
     shield" clauses that vendors now offer, their caps, their
     conditions (acceptable-use compliance, no-opt-out from
     safety mitigations), and what they exclude
     <!-- needs-research: confirm current scope and caps of
     publicly announced copyright-indemnity programs from major
     model vendors and hyperscalers at time of use -->
   - *Evaluation and audit rights* — the buyer's right to
     evaluate on buyer-provided data, to run red-team exercises,
     to access model cards and system cards, and to inspect the
     vendor's own evaluation results
   - *Change-of-control, assignment, and sub-contracting* — who
     ends up operating the service if the counterparty is
     acquired, spun out, or restructured
   - *Service-level objectives for AI* — latency, throughput,
     availability, *and* model-behavior-equivalence under
     version upgrades; the SLO dimensions that are specific to
     AI and that generic cloud-contract templates do not cover
   - *Deprecation and version policy* — notice period, parallel-
     endpoint duration, equivalence testing, forced-migration
     commitments
   - *Residency and operator-access* — data region, operator
     location, administrative access, key custody — the clauses
     that make a residency position defensible rather than
     aspirational (MOD-406 overlap)
   - *Exit and transition* — cooperation on migration, data
     return in a documented format, model-output return, prompt
     and evaluation-set return, run-off licensing for cached
     outputs

9. **Commercial and pricing structures**
   - Per-token, per-request, per-image, per-minute,
     per-megabyte-of-embeddings, per-GPU-hour, per-seat,
     per-named-user, platform-fee, and committed-use pricing
     models — and the way these combine inside a single
     agreement
   - The *rate card vs. enterprise rate* distinction, and the
     negotiation surface where volume, commit, co-marketing,
     reference-ability, and strategic value are converted into
     discount
   - *Price-protection* clauses — ceiling, most-favored-nation,
     lookback — and the standard limits
   - *Budget-governor and alerting* commitments, and the
     organization's ability to cap consumption at the API
     boundary without having to re-architect the application
   - *Credits, migration incentives, and funding programs* — the
     hyperscaler and model-vendor migration programs that fund
     a buyer's switching cost, and the way these should be
     treated in TCO and lock-in analysis
     <!-- needs-research: refresh current major vendor
     migration-funding programs and their public eligibility
     terms at time of use -->

10. **Data-partner and training-data licensing specifics**
    - *Content-license* structures for text, image, audio,
      and video training data — the "license for model
      training" category that emerged after 2023 and is still
      consolidating
      <!-- needs-research: refresh the landscape of major
      content-licensing deals (news publishers with OpenAI /
      Anthropic / Google, Reddit, Stack Overflow, Shutterstock,
      Getty, music catalog deals) and the standard clause
      patterns -->
    - *Opt-out, right-to-be-forgotten, and TDM-exception*
      mechanics across jurisdictions (EU DSM Directive Article
      4, UK TDM exception, US fair-use posture under current
      litigation, Japan Article 30-4 copyright exception),
      and the way a data vendor's pipeline must express these
      <!-- needs-research: refresh pending and decided AI
      training-data litigation at time of use (NYT v. OpenAI,
      multiple class actions, Getty v. Stability, etc.) and
      the way major settlements and rulings shift the
      contractual baseline -->
    - *Labeling and RLHF* vendor terms — worker-welfare
      commitments, provenance of labelers, contested-
      jurisdiction labor exposure, and quality-governance clauses
    - *Synthetic-data* contracts — provenance of the generator,
      downstream-use restrictions, and the "distilled from a
      larger model" clause the originating vendor increasingly
      includes

11. **The clause positions the organization refuses to deploy without**
    - Standing-position language on each of the clauses in (8)
      — the *default demand*, the *acceptable fallback*, and
      the *walk-away*
    - The named executive who can approve a deviation from the
      standing position, and the documented exception register
    - The clauses that, in 2026, the market has moved on and
      that are now table stakes (no training on customer
      inputs by default; basic IP indemnity; documented
      incident-notification SLA); the clauses that are still
      contested
    - The exception-approval pipeline with Legal, Security,
      Trust & Safety, Procurement, and the relevant business
      unit, and the signed artifact the exception produces

### Partnership Governance Models

12. **Governance structures for load-bearing partnerships**
    - *Joint executive sponsor* — a named leader on each side,
      with the authority to redirect their organization's
      investment in the relationship
    - *Joint steering committee* — quarterly operating cadence,
      standing metrics, standing agenda items, and standing
      membership
    - *Joint operating committee* — monthly tactical review of
      SLOs, incident history, roadmap deltas, and open issues
    - *Technical working groups* — the project-level teams that
      actually ship the joint work
    - The governance-intensity ladder — supplier through
      alliance — and the specific artifacts each tier produces
      (operating-review deck, QBR, joint plan, joint
      roadmap, joint public announcement)
    - When *not* to stand up governance — the "ceremonial
      joint steering committee for a vendor relationship that
      is actually a procurement line item" failure mode

13. **Escalation and dispute resolution**
    - A documented escalation ladder with named counterparts
      at each tier, not just a generic "senior management"
      pointer
    - The published-SLA path (credit, root-cause, remediation)
      vs. the strategic-dispute path (executive meeting,
      framework re-negotiation, exit consideration)
    - Arbitration, mediation, governing-law, and venue clauses
      — and the way these play out in a multinational
      AI-vendor relationship where the vendor is in one country,
      the data is in several more, and the regulated customer
      is in a third
    - The "joint postmortem" discipline for a shared incident
      (vendor downtime, output-quality regression, safety
      incident, data-exposure incident) as the operational
      expression of a governance regime

14. **Review, renegotiation, and renewal cadence**
    - Formal annual or bi-annual relationship review — against
      the original rationale and the current environment
    - Renegotiation triggers — SLO miss above a threshold,
      material pricing change elsewhere in the market,
      material change in the vendor's capability or strategy,
      change of control, security or trust incident
    - The *scheduled* renegotiation — the organization's
      standing posture that every multi-year AI commitment
      is re-opened on a defined cadence, not left to drift
    - The "quiet renewal" anti-pattern — multi-year commits
      that auto-renew at list price because no one owned the
      opening of the renegotiation window

15. **Exit, transition, and continuity**
    - Documented exit scenarios for each load-bearing
      partnership — vendor pricing shift, vendor acquisition by
      a competitor, vendor regulatory enforcement, vendor
      trust-and-safety incident, vendor strategic pivot, vendor
      insolvency
    - The *transition-services* clause — the vendor's obligation
      to cooperate with migration for a defined period, at a
      defined rate, with defined deliverables
    - Data, model-output, and prompt-return format commitments
      that make the exit clause actually executable
    - The dual-vendor and portability-investment posture
      (MOD-406 overlap) that makes exit *affordable* rather
      than only *contractually possible*
    - The documented "we wound down vendor X" case study the
      organization keeps for its own institutional memory —
      the artifact that allows the next exit to be faster

### Ecosystem Development and Platform Strategy

16. **The "which side of the ecosystem" decision**
    - Whether the organization participates in *other people's*
      ecosystems (partner programs, marketplaces, co-sell
      motions) or operates its *own* (marketplace, agent store,
      app gallery, partner directory)
    - The economics — a participant captures a share of a
      larger pool and absorbs the ecosystem's governance; an
      operator captures a platform fee and takes on the
      governance responsibility
    - Being both at once — the dominant pattern for enterprise
      AI vendors in 2026 — and the specific conflicts it
      creates (competing on apps the organization also
      distributes; hosting agents the organization also builds;
      certifying partners who also compete with the
      organization's services arm)

17. **Running a partner program**
    - Partner tiers (registered, silver, gold, premier, elite
      — the standard ladder, under many names) and the
      *earnable benefits* at each tier (co-sell credit,
      marketing development funds, technical enablement,
      early-access to roadmap, named partner manager)
    - Certification — individual (practitioner, specialist,
      architect) and organizational (practice certification,
      competency badges) — and the integrity cost of
      certification-inflation
    - Co-marketing and co-selling motion — the "sold-with" vs.
      "sold-through" distinction, revenue recognition, and the
      compensation-plan questions that make or break
      salesforce engagement
    - Partner enablement — training, sandbox access, pre-GA
      preview, technical account management — and the
      investment pattern that signals partner commitment vs.
      partner-washing
    - Public partner directories as a governance artifact —
      the organization's statement of who is in good standing

18. **Marketplace operation**
    - The *platform governance* obligations an AI marketplace
      takes on — acceptable-use enforcement for third-party
      apps and agents, safety-review before listing, incident
      response for third-party failures, revenue-share mechanics
    - Submission, review, approval, and delisting workflow —
      and the published criteria that make the operator
      defensible rather than arbitrary
    - The *trust surface* a marketplace commits to on behalf
      of third-party listings — and the way this collides with
      the operator's own liability posture
    - Revenue-share economics — the conventional 30/70,
      20/80, and specialty splits for AI apps and agents,
      and the negotiated-enterprise deviations
      <!-- needs-research: refresh public revenue-share
      disclosures for major AI marketplaces (Salesforce
      AppExchange / Agentforce, Microsoft AppSource,
      ServiceNow Store, Google / AWS / Azure AI marketplaces,
      OpenAI GPT store, Anthropic app directory) at time of
      use -->
    - *De-listing and enforcement* authority — the operator's
      stated and exercised right to remove, downrank, or label
      listings for safety, legal, or trust reasons

19. **Open-source, standards, and consortia as partnerships**
    - Open-source contribution as a partnership with a
      community, not a vendor — license choice (Apache 2.0,
      MIT, BSL, SSPL, OpenMDW-era proposals), contribution
      governance, trademark policy, release-management
      discipline
      <!-- needs-research: refresh the state of
      source-available / "open-weights" / "open-source but
      not OSI-approved" licensing debates for model weights at
      time of use (Llama Community License, Qwen License,
      DeepSeek License, Mistral AI License, Apache-2.0
      weights, OSI-OSAID effort) -->
    - Standards participation — ISO/IEC JTC 1 SC 42 (AI),
      CEN-CENELEC JTC 21, IEEE P7000 series, NIST AI
      consortium / AISIC, MLCommons, OASIS — as a
      multi-year commitment with staffing and travel budget
      implications
    - Consortia and coalitions — Frontier Model Forum,
      Partnership on AI, AI Alliance, ML Commons, MLPerf,
      sector-specific AI consortia in finance, healthcare,
      and energy — as influence partnerships with distinct
      membership tiers and governance roles
      <!-- needs-research: refresh current membership tiers,
      governance roles, and public workstreams of the Frontier
      Model Forum, AI Alliance, Partnership on AI, and sector
      AI consortia at time of use -->
    - Standards-as-partnership — the way participation in
      drafting a standard is both a public good and a
      competitive position, and the governance disciplines
      that keep the two honest

### Co-Innovation Partnerships

20. **Joint-research and co-development structures**
    - Sponsored research agreements with universities and
      national labs — IP assignment, publication rights,
      student and postdoc involvement, export-control implications
    - Industry-lab collaborations — joint-paper and shared-
      benchmark structures, red-team and safety-evaluation
      partnerships, frontier-model access programs
    - Pre-competitive consortia — the common-good research
      that is cheaper to fund together than to replicate
      (safety benchmarks, evaluation infrastructure,
      watermarking standards, provenance infrastructure)
    - The *jointly produced artifact* — the way a co-innovation
      partnership succeeds or fails on whether it produces a
      named, dated, publicly or privately released artifact,
      and whether the two sides agree on what that artifact is
      before the work begins

21. **Co-innovation IP arrangements**
    - *Joint ownership* — the easy-looking, hard-to-execute
      default; the unpooled rights it creates, and why
      enterprise counsel will often veto it
    - *Background IP, foreground IP, and residual knowledge*
      as the standard three-part framework — and the
      specific definitions that the AI era has started to
      strain (do fine-tuning adapters count as foreground IP
      or residual knowledge? Who owns an evaluation set
      produced during a joint engagement? Who owns a prompt
      library?)
    - *Field-of-use* licensing as the alternative to joint
      ownership — each side gets exclusive rights in defined
      fields, shared rights outside
    - *Publication and talking-rights* clauses — the right of
      each side to publish, talk at conferences, blog, and
      issue press releases about the joint work, and the
      review-and-approval process that keeps those from
      becoming disputes
    - *Patent cross-licensing and non-assertion* in an area
      where the patent landscape is both unclear and
      strategically important

22. **Strategic alliances with equity or capital commitment**
    - The *compute-for-equity* pattern (hyperscaler takes equity
      or a convertible instrument in a frontier lab in exchange
      for a multi-year compute commitment) as the canonical
      AI-era alliance structure
      <!-- needs-research: refresh publicly disclosed
      hyperscaler-frontier-lab alliance structures and known
      investment / commitment terms at time of use -->
    - *Strategic minority investment* — the corporate-VC
      posture that creates an inside track to a partner's
      roadmap without triggering consolidation
    - *Partnership + reseller + co-sell* stacked structures,
      and the governance integrity problem they create (the
      partner's sales team recommending the investor's platform
      as "the preferred cloud")
    - *Joint-venture* structures for a specific market,
      jurisdiction, or capability — governance intensity is
      highest, exit is hardest, strategic lock-in is greatest

### Risk Management in Partnerships

23. **Concentration and counterparty risk**
    - The top-three-vendor concentration disclosure the board
      and a CFO will ask for — percent of AI workload
      addressable value dependent on each of the top three
      counterparties, on the top three models, on the top
      three clouds
    - *Single-point-of-failure* mapping across the stack
      — model vendor, hyperscaler, specialist cloud, data
      vendor, systems integrator — and the "would survive a
      30-day loss of any one" stress test
    - *Counterparty financial* risk, specifically for pre-
      profitability frontier labs with multi-year commitments
      that require continuing capital — the "vendor goes dark"
      scenario and the weight-escrow, source-escrow, and
      transition-services response
    - *Second-order* concentration — the way all three major
      clouds in 2026 are entangled with specific frontier labs,
      so a "dual-cloud" strategy that relies on two clouds
      hosting the same frontier lab is less diversified than
      it appears

24. **Legal, regulatory, and trust risk through partnerships**
    - *Vicarious liability* for a partner's acts — EU AI Act
      role liability (a deployer relying on a non-compliant
      GPAI provider still carries deployer obligations),
      vendor data-processing failures under GDPR, financial-
      sector third-party risk under EBA / PRA / OCC
      supervisory letters, sectoral vendor-risk expectations
      in healthcare and critical infrastructure
      <!-- needs-research: refresh current third-party /
      outsourcing / operational-resilience regulatory
      expectations in financial services (PRA SS2/21, EBA
      ICT Risk Guidelines, DORA, OCC Third-Party Risk
      Management) and in healthcare / critical infrastructure
      at time of use -->
    - *Reputational contagion* — a trust incident at a
      partner is a trust incident at the organization in the
      eyes of customers and regulators, and sometimes in
      those of enforcement authorities
    - *Export-control and sanctions* exposure via a partner —
      the Foreign Direct Product Rule and designated-party
      rules reach through corporate structures, so a
      partnership with a vendor that has a listed
      sub-processor exposes the organization
    - *Competition and antitrust* exposure — partnerships
      that look like coordination (shared compute commitments,
      interlocking directors, exclusive-channel deals with
      dominant vendors, "most-favored-nation" clauses with a
      market leader) are an increasing enforcement focus
      <!-- needs-research: refresh current competition-
      authority inquiries into major AI-industry partnerships
      and investments (FTC, DOJ, CMA, EC, BKartA) at time of
      use -->

25. **Security and trust-and-safety risk**
    - *Shared-security-model* clarity — the vendor's
      responsibility, the customer's responsibility, and the
      gap area that becomes incident scope when it is tested
    - *Third-party access* — the vendor's operators, the
      vendor's sub-processors, the vendor's AI-inside-the-
      vendor (second-order vendors), and the audit
      transparency available on each
    - *Prompt and output logging* risk — the way default
      vendor logging of prompts can create a residency,
      sensitive-data-exposure, and litigation-hold problem
      the application team does not surface
    - *Supply-chain security* on vendor-delivered models,
      adapters, and open-weights releases — provenance,
      integrity, backdoor and data-poisoning posture
    - *Trust-and-safety classifier* risk — the vendor's
      policies silently changing the behavior of a deployed
      product, the "vendor pulled the model" scenario

26. **Partnership-portfolio risk as a board-reported metric**
    - The *concentration delta* over time — whether the
      portfolio is becoming more or less diversified
    - The *contract-posture coverage* — percent of load-bearing
      partnerships operating on the standing position clause
      set vs. operating on legacy / non-conforming contracts,
      and the plan to close the gap
    - The *scenario-readiness* coverage — percent of load-
      bearing partnerships with a tested exit plan, as
      distinct from a contractual exit right
    - The *governance-health* report — on-time steering
      committees, published joint operating reviews, open
      escalations, named-sponsor continuity, SLO attainment —
      per load-bearing partnership

### Partnership Lifecycle and the Operating Rhythm

27. **The partnership lifecycle as an enterprise discipline**
    - *Identification* — scouting, warm introduction,
      preliminary fit assessment, confidentiality cover
    - *Qualification* — due diligence, business-case
      preparation, internal socialization, legal-privacy-security
      pre-review
    - *Deal construction* — term-sheet, standing-position clause
      application, exception approval, governance design
    - *Operational launch* — joint kickoff, operating cadence
      initiation, baseline SLO and metric reporting,
      communication to customers and workforce
    - *Operation* — standing cadence, QBRs, joint roadmap,
      incident and escalation handling
    - *Review and renegotiation* — scheduled framework review,
      performance against original rationale, market and
      regulatory delta, forward renewal or re-scope
    - *Exit* — scheduled, triggered, or crisis-driven
      transition; migration execution; institutional memory
      capture

28. **Communicating partnership posture**
    - **Board**: concentration, counterparty risk, named
      scenarios, posture delta over the year, capital
      commitments the portfolio represents
    - **Regulator**: load-bearing third parties, due-diligence
      regime, exit regime, incident-cooperation posture
    - **Customer (enterprise)**: the sub-processor list, the
      shared-security-model documentation, the exit/transition
      support, the stability of the vendor stack
    - **Government customer**: the specific partners that
      touch the regulated workload, their jurisdictional
      status, and the custody / sign-off commitments
    - **Partner (incoming)**: the standing position, the
      governance expectation, the exit expectation — stated
      before the term-sheet, not discovered during contract
    - **Workforce**: which partnerships are load-bearing,
      which are transitioning, and what that means for the
      roles that touch them

---

## Module Structure

```
mod-407-strategic-partnerships/
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

### Week 1: The Partnership Ecosystem Map and Vendor-Stack Inventory (6 hours)

**Topics:**
- The AI-vendor stack as layered dependency — foundation-model
  layer, compute layer, data layer, platform and application
  layer, services layer — read as *partnerships* rather than as
  procurement line items
- Partnership roles and archetypes — supplier, strategic vendor,
  strategic partner, alliance, joint venture — and the
  governance intensity each tier actually requires
- The ecosystem role the organization plays — builder, assembler,
  channel, platform, marketplace — and the failure mode of
  being three without having chosen
- Reading the organization's current partnership portfolio as a
  concentration-risk disclosure — counterparty, substitutability,
  contractual posture, governance health

**Readings:**
- Primary-source hyperscaler partner-program pages (AWS Partner
  Network, Microsoft AI Cloud Partner Program, Google Cloud
  Partner Advantage) as a map of partnership archetypes
  <!-- needs-research: refresh current partner-program tier
  structures at time of use; these are re-named roughly every
  18 months -->
- Frontier-lab developer and enterprise documentation on
  deployment options and partner programs (OpenAI Enterprise,
  Anthropic Enterprise and Partners, Google Cloud / Vertex AI
  partner materials, AWS Bedrock partner materials)
  <!-- needs-research: refresh current frontier-lab enterprise
  and partner program structures at time of use -->
- Anu Bradford — *Digital Empires* (background on the
  regulatory and competitive frame in which AI partnerships now
  operate)
- The organization's own current vendor-stack inventory (bring
  it to Week 1; this is the baseline for the module)

**Exercise:** Audit your organization's current AI partnership
portfolio. Draw the ecosystem map (model vendor, cloud vendor,
GPU-specialist cloud, data vendor, systems-integrator, platform
and tooling vendors) and classify each by role, substitutability,
counterparty risk, and contractual posture. A one-page memo to
the CTO on what the map actually shows. See
`exercises/exercise-01-case-study.md` for a structured version.

---

### Week 2: Vendor Evaluation and Due Diligence at Enterprise Scale (7 hours)

**Topics:**
- The AI-vendor due-diligence framework across six dimensions
  (technical, financial, legal and regulatory, security and
  trust, operational, strategic) — as a standing checklist and
  a sequenced workflow
- Model-vendor-specific diligence — provenance, evaluation
  posture, safety and T&S, fine-tuning and customization terms,
  deployment options, model-lifecycle commitments
- Hyperscaler and compute-vendor-specific diligence — EDP /
  MACC / CUD mechanics, reserved vs. on-demand accelerator
  inventory, capacity commitments, egress economics,
  portability clauses, marketplace participation
- Systems-integrator and services-partner diligence — partner
  tiers and what they mean, delivery-risk evaluation, IP and
  deliverables
- The "pre-GA vendor" problem — committing to a counterparty
  whose product, pricing, and corporate form are still forming,
  and the specific contractual and governance mitigations

**Readings:**
- NIST AI 600-1 — *Generative AI Profile*, with emphasis on
  third-party / supply-chain risk categories
- ISO/IEC 42001 — *AI management system* clauses on third-party
  AI relationships
  <!-- needs-research: confirm current ISO/IEC 42001 clause
  references and any published implementation guides at time
  of use -->
- Published due-diligence frameworks from financial-sector
  supervisors (OCC Third-Party Risk Management guidance, EBA
  Guidelines on outsourcing arrangements, UK PRA SS2/21,
  EU DORA on ICT third-party risk)
  <!-- needs-research: confirm current revisions and effective
  dates of each at time of use; financial-services third-party
  risk guidance is an active regulatory frontier -->
- Primary-source vendor transparency documents — model cards,
  system cards, usage policies, trust centers, sub-processor
  lists — from the counterparties in your Week 1 inventory
- Published AI-vendor security and trust posture documents
  (SOC 2 Type II reports, ISO/IEC 42001 certifications, FedRAMP
  authorizations, HIPAA attestation letters) for a representative
  sample of the vendor stack

**Case Study:** A global retailer is evaluating two candidate
foundation-model vendors as the strategic model partner for a
customer-facing GenAI assistant: a frontier lab with a
hyperscaler affiliation (pre-profitability, multi-year equity
and compute commitments) and a sovereign-aligned vendor with
in-region operator access and lower per-request pricing.
Produce a comparative due-diligence memo across the six
dimensions, call out the three dimensions where the choice is
clear and the three where the trade-offs are genuine, and
recommend a primary + secondary posture.

**Deliverable:** A vendor-evaluation framework (10-15 pages)
covering:
- The six-dimension due-diligence checklist as applied to the
  organization's workload mix
- Named evidence artifacts collected for each dimension
- The decision log and sign-off ladder
- Counterparty-risk disclosure to the CRO and the board-risk
  committee

---

### Week 3: Contract Architecture and Negotiation (8 hours)

**Topics:**
- The AI-specific clause set that distinguishes an AI vendor
  contract from a generic SaaS contract — input rights, output
  rights, training-data warranties, IP indemnification,
  evaluation and audit rights, change-of-control, AI-specific
  SLOs, deprecation and version policy, residency and operator-
  access, exit and transition
- Commercial and pricing structures — per-token, per-request,
  per-GPU-hour, per-seat, committed-use, enterprise-rate
  construction, price-protection, budget-governor, migration-
  credit programs
- Data-partner and training-data licensing specifics — content-
  license structures, opt-out and TDM-exception mechanics,
  labeling and RLHF vendor terms, synthetic-data contracts
- The clause positions the organization refuses to deploy
  without — standing-position language, acceptable fallback,
  walk-away, the named approver of each deviation, the
  exception register
- Negotiation choreography — procurement, legal, security,
  trust-and-safety, business-unit, and executive sequencing;
  avoiding the "contract signed before T&S reviewed it"
  failure mode

**Readings:**
- Primary-source vendor master service agreements and
  enterprise terms for at least two foundation-model vendors
  and two hyperscalers (publicly posted versions), read
  side-by-side against the organization's standing position
- Published model-vendor training-data and output-rights
  position documents and model-card appendices
- IAPP — *AI Vendor Risk Management* practical guidance; and
  the relevant SIG (Shared Assessments) and CAIQ (CSA)
  questionnaires as a floor rather than a ceiling
  <!-- needs-research: confirm current IAPP, Shared
  Assessments, and Cloud Security Alliance AI-vendor
  questionnaire versions at time of use -->
- Published IP-indemnity program documents from major model
  vendors and hyperscalers
  <!-- needs-research: refresh the current scope, caps, and
  conditions of the major copyright-indemnity programs at
  time of use -->
- The organization's own existing AI vendor contracts, as a
  gap-analysis input against the standing-position clause set

**Exercise:** Draft the organization's standing-position clause
set as a one-page internal reference — the default demand, the
acceptable fallback, and the walk-away for each of the AI-
specific clauses. Identify the top three clauses where the
organization's current contracts do not meet the standing
position, and the remediation plan. See
`exercises/exercise-02-strategy-memo.md` for a structured version.

**Deliverable:** A contract-architecture playbook (10-15 pages)
covering:
- The standing-position clause set with default / fallback /
  walk-away language for each clause
- The exception-approval pipeline and the named approvers
- The gap-analysis against current contracts and a
  remediation roadmap
- The named standing-position reviewer (typically General
  Counsel + Chief Trust Officer + CPO) and the quarterly
  review cadence

---

### Week 4: Partnership Governance, Co-Innovation, and Alliances (8 hours)

**Topics:**
- Governance structures for load-bearing partnerships — joint
  executive sponsor, joint steering committee, joint operating
  committee, technical working groups — and the governance-
  intensity ladder from supplier through alliance
- Escalation and dispute resolution — the published-SLA path
  vs. the strategic-dispute path, governing-law and venue in a
  multinational AI relationship, joint-postmortem discipline
- Review, renegotiation, and renewal cadence — scheduled
  renegotiation as a standing posture, renegotiation triggers,
  the "quiet renewal" anti-pattern
- Co-innovation structures — sponsored research, industry-lab
  collaborations, pre-competitive consortia, the jointly
  produced artifact as the success test
- Co-innovation IP arrangements — joint ownership, background /
  foreground / residual knowledge, field-of-use licensing,
  publication and talking-rights, patent cross-licensing
- Strategic alliances with equity or capital commitment —
  compute-for-equity as the canonical AI-era structure,
  corporate-VC strategic minority investment, stacked
  partnership + reseller + co-sell + investment structures and
  their governance-integrity costs

**Readings:**
- Publicly disclosed strategic AI alliances and their
  announced governance structures — Microsoft-OpenAI, Amazon-
  Anthropic, Google-Anthropic, Oracle-OpenAI, NVIDIA
  investments in frontier labs, sovereign-vendor alliances
  (e.g., Microsoft-G42)
  <!-- needs-research: refresh the current list of major
  publicly disclosed AI alliances with commitment scale and
  governance disclosures at time of use -->
- Frontier Model Forum, Partnership on AI, AI Alliance public
  governance documents
  <!-- needs-research: refresh membership, workstream, and
  governance documents at time of use -->
- MLCommons / MLPerf governance and participation structure
- Published joint-research-partnership templates from
  university tech-transfer offices (Stanford OTL, MIT TLO,
  Oxford OUI, Cambridge Enterprise) — the industry-friendly
  defaults and their negotiation surface
- Primary-source open-source AI license texts and the state of
  the "open-source for model weights" debate (Llama Community
  License, Qwen License, DeepSeek License, Mistral AI License,
  Apache-2.0 weights releases, the OSI OSAID effort)
  <!-- needs-research: refresh license landscape at time of use;
  this is an actively contested area -->

**Case Study:** Your organization is negotiating a strategic
alliance with a frontier lab that includes a multi-year compute
and model commitment, a joint go-to-market motion, access to
pre-GA model checkpoints, and a corporate-VC investment. The
General Counsel is concerned about competition exposure from
the stacked structure and about the organization's ability to
exit if the lab's strategy diverges. The Chief Trust Officer
is concerned about reputational linkage to the lab's
trust-and-safety incidents. The CFO wants a structure that
accounts for both the partnership economics and the
investment carry. Design the governance, decision-rights, and
exit architecture for the alliance.

**Deliverable:** A partnership governance model (10-15 pages)
covering:
- Governance intensity by partnership tier, with named
  artifacts and cadence
- The escalation and dispute-resolution ladder with named
  counterparts
- The scheduled renegotiation and renewal cadence per tier
- The co-innovation IP framework (background / foreground /
  residual knowledge; publication and talking-rights;
  field-of-use)
- The alliance-structure decision framework (when equity,
  when JV, when co-sell only)

---

### Week 5: Ecosystem Strategy and Platform Partnerships (6 hours)

**Topics:**
- The "which side of the ecosystem" decision — participant in
  others' ecosystems vs. operator of the organization's own —
  and the conflict profile of being both at once
- Running a partner program — tier structure, earnable
  benefits, certification integrity, co-sell / sold-with /
  sold-through mechanics, enablement investment, public
  partner directories as a governance artifact
- Marketplace operation — platform-governance obligations,
  submission / review / approval / delisting workflow,
  revenue-share economics, trust surface, de-listing authority
- Open-source, standards, and consortia as partnerships —
  license choice, contribution governance, standards
  participation (ISO/IEC JTC 1 SC 42, CEN-CENELEC JTC 21, IEEE,
  NIST, MLCommons, OASIS), coalition membership (Frontier Model
  Forum, Partnership on AI, AI Alliance, sector AI consortia)
- Standards-as-partnership — participation as public good and
  as competitive position, and the governance disciplines that
  keep the two honest

**Readings:**
- Salesforce AppExchange and Agentforce ecosystem public
  documentation — tier structure, submission and security
  review, revenue share
- Microsoft AppSource, ServiceNow Store, and ServiceNow /
  Salesforce Agentforce ecosystem announcements
- AWS Marketplace and Bedrock Marketplace vendor-onboarding
  and listing policies
- Apple App Store, Google Play Store, and the current state of
  app-store policy as a baseline for AI-marketplace trust and
  liability
- ISO/IEC JTC 1 SC 42 and CEN-CENELEC JTC 21 public work
  programs — the active standards and their harmonised-
  standard status under the EU AI Act
  <!-- needs-research: refresh current SC 42 and JTC 21 work
  programs at time of use -->
- Frontier Model Forum, AI Alliance, Partnership on AI, and
  sector AI consortia public workstreams and membership tiers
  <!-- needs-research: refresh at time of use -->

**Case Study:** A B2B software vendor with a strong vertical
product is deciding between three ecosystem postures: (a) joining
a dominant platform's agent marketplace as a listed app, (b)
standing up its own vertical AI-agent marketplace on top of its
existing data assets, or (c) building a hybrid — participating
in a dominant platform *and* operating a specialist marketplace
in its vertical. Analyze the economics, the governance cost, the
competitive exposure, and the recommended posture.

**Deliverable:** An ecosystem-strategy memo (8-10 pages)
covering:
- The organization's chosen position on the builder / assembler
  / channel / platform / marketplace axis
- The partner-program design (if applicable) — tiers, earnable
  benefits, certification, enablement, directory
- The marketplace-governance design (if applicable) —
  submission, review, revenue share, de-listing, trust surface
- The standards and consortia participation plan with named
  workstreams and assigned staff

---

### Week 6: Risk, Resilience, and Partnership Crisis Communication (6 hours)

**Topics:**
- Concentration and counterparty risk — the top-three-vendor
  disclosure, single-point-of-failure mapping, counterparty
  financial risk for pre-profitability frontier labs, second-
  order concentration through hyperscaler-lab entanglement
- Legal, regulatory, and trust risk through partnerships —
  vicarious liability under EU AI Act role mapping and under
  financial-sector third-party-risk regimes, reputational
  contagion, export-control exposure, competition / antitrust
  exposure
- Security and trust-and-safety risk — shared-security-model
  clarity, third-party access and sub-processors, prompt and
  output logging as a residency / exposure surface, supply-
  chain security on vendor-delivered models and adapters, T&S
  classifier risk
- Partnership-crisis scenarios — vendor pricing shift, vendor
  acquisition by a competitor, vendor trust incident, vendor
  regulatory enforcement, vendor strategic pivot, vendor
  insolvency, vendor "goes dark" scenario
- Resilience design under partnership stress — dual-vendor
  posture, portability investment, weight / source / data
  escrow, documented transition services, a tested exit plan
  rather than a contractual exit right
- Board-level partnership reporting — concentration delta,
  contract-posture coverage, scenario-readiness coverage,
  governance-health report, as a quarterly standing agenda item
- Partnership-crisis communication — board, regulator, customer,
  government customer, incoming partner, workforce

**Readings:**
- Gary Klein, HBR — "Performing a Project Premortem" (applied
  to the partnership-crisis scenario set; reinforced from
  MOD-402, MOD-404, MOD-406)
- Barbara Minto — *The Pyramid Principle* (reinforced from
  MOD-402 for board and crisis communication)
- Published post-mortems and regulator actions involving AI
  vendor and third-party failures — vendor data incidents,
  shared-security-model disputes, open regulator inquiries
  <!-- needs-research: assemble a short list of
  partnership-relevant incident post-mortems and regulator
  actions within the last 24 months at time of use -->
- Published 10-K risk factors on AI-vendor concentration,
  counterparty exposure, and competition/antitrust in AI from
  AI-heavy public companies
  <!-- needs-research: assemble a current short list -->
- NIST SP 800-161 (Cybersecurity Supply Chain Risk
  Management) applied to AI vendor dependencies
  <!-- needs-research: confirm current revision of SP 800-161
  and any AI-specific supply-chain guidance from NIST or
  NIAC at time of use -->

**Scenario:** On a Thursday afternoon the primary foundation-
model vendor for your flagship GenAI product announces (a) a
50% price increase on the capacity tier your workload is
committed to, (b) a change-of-control — a competitor of yours
has agreed to acquire a controlling stake, pending regulator
sign-off, and (c) a six-month deprecation window on the
specific model version you deployed your product on, with a
successor that scores measurably differently on your in-house
evaluation. Your board has a scheduled meeting Tuesday. Draft:
- 1-page board briefing (what is contained, what is not,
  options with 30/60/90-day impact, what you are asking the
  board to approve)
- Internal all-hands note (workforce framing, including the
  teams that would move or pause under each option)
- Customer communication under each option (including named
  customers under custom contractual commitments)
- Regulator communications under each option (home
  jurisdiction and, where applicable, financial-sector or
  AI-specific supervisor)
- 30/60/90-day plan under the chosen option with named owners
- Decision log template for the next 72 hours

**Exercise:** Board-level presentation on the current state of
the organization's AI partnership portfolio. See
`exercises/exercise-05-presentation.md`.

**Deliverable:** Board-ready deck (10-15 slides) on the state
of the organization's AI partnership program — concentration,
counterparty risk, contract-posture coverage, scenario-
readiness coverage, and the forward plan — reviewed with a
peer using the "so what?" test at every slide.

---

## Case Studies

### Case Study 1: AWS as the Enterprise Partnership Reference

**Background:**
- The incumbent hyperscaler's partner program (AWS Partner
  Network) and its enterprise-discount, co-sell, marketplace,
  and competency architecture as a reference for how a
  partnership program is designed and run at scale
  <!-- needs-research: refresh current APN tier structure,
  competency framework, co-sell program (ACE), marketplace
  listing categories, and strategic collaboration agreement
  (SCA) mechanics at time of use -->
- The Bedrock and model-marketplace overlay as the AI-era
  partnership shape — multiple frontier labs offered under a
  single commercial surface, with the hyperscaler as
  intermediary and partial counterparty
  <!-- needs-research: refresh Bedrock model lineup and
  partner-lab commercial posture at time of use -->
- The Amazon-Anthropic strategic alliance as the AI-era
  compute-for-equity pattern, and the specific implications
  for an enterprise buyer whose "cloud vendor" and "model
  vendor" are now related parties
  <!-- needs-research: verify the current public disclosures
  of the Amazon-Anthropic investment and commercial
  relationship at time of use -->
- Strategic Collaboration Agreements as the top-tier
  partnership instrument and the governance intensity they
  carry

**Your Role:** Senior AI infrastructure architect at a large
enterprise deployer evaluating the organization's current AWS
partnership posture — tier, co-sell participation, enterprise
discount program, Bedrock usage, and the specific second-order
exposure to the hyperscaler's model-vendor affiliations.

**Assignment:**
1. Produce a current-state assessment of the organization's
   AWS partnership — tier, discount structure, co-sell
   participation, marketplace listings bought and sold, AI-
   service consumption, model-vendor affiliations reached
   through the hyperscaler
2. Identify the three partnership dimensions where the current
   posture is *under-realized* (benefits earned but unclaimed,
   roadmap input available but un-used) and the three where it
   is *over-committed* (concentration, unused commit, SLA
   exposure)
3. Produce a recommended twelve-month partnership plan — tier
   placement, commit structure, Bedrock and marketplace
   posture, co-sell participation, and the explicit
   concentration-mitigation steps
4. Pre-wire the plan with CFO, CTO, CRO, General Counsel, and
   the relevant business-unit leaders

**Deliverables:**
- Current-state assessment (8-10 pages)
- Comparative partnership-posture memo across the two or
  three realistic alternative postures (5-7 pages)
- Three-option decision brief (deepen / rebalance / split)
- Stakeholder pre-wiring plan
- Board-facing recommendation memo

**Success Criteria:**
- Assessment is defensible under an external audit on
  concentration risk and counterparty-affiliation disclosure
- Decision survives a CFO challenge on multi-year committed-
  spend and a CRO challenge on counterparty-affiliation
  risk through the hyperscaler-lab linkage
- Partnership-plan recommendations are specific and testable,
  not "deepen the strategic relationship"

---

### Case Study 2: Salesforce AppExchange and Agentforce as a Marketplace-Operator Reference

**Background:**
- One of the longest-running enterprise software marketplaces,
  with decades of accumulated governance practice —
  submission, security review, revenue share, listing
  policies, de-listing — now extended into agent distribution
  under the Agentforce brand
  <!-- needs-research: refresh current Agentforce and
  AppExchange policies on agent submission, security review,
  revenue share, and partner-tier structure at time of use -->
- The ISV partner ecosystem as both a distribution asset for
  Salesforce and a strategic obligation — the partners have
  made multi-year investments on top of Salesforce's platform
  and expect governance continuity, roadmap input, and
  commercial equity
- The AI-agent distribution question — whether the marketplace
  operator competes with its own ISV partners on specific agent
  categories, and the published posture on this
- The regulatory layer — agent and app marketplaces as a
  category under increasing scrutiny from competition
  authorities, consumer-protection regulators, and AI-specific
  regulators (EU AI Act transparency obligations on deployers;
  US state AI laws on employment-adjacent uses)

**Your Role:** Senior AI infrastructure architect at a B2B
software vendor deciding whether and how to participate in the
Salesforce Agentforce ecosystem, whether to stand up a
competing specialist marketplace in the organization's
vertical, or to pursue a hybrid.

**Assignment:**
1. Produce a current-state assessment of the Salesforce agent
   and app ecosystem as a partner opportunity — tier structure,
   revenue share, security-review posture, SLA implications
   for agent listings, and the specific exposure to
   marketplace-operator-as-competitor on the organization's
   categories
2. Produce the comparable assessment of running the
   organization's own specialist marketplace — the trust-
   surface obligations, the governance-staff investment, the
   listing policy, the submission / review / de-listing
   workflow, the revenue-share mechanics
3. Produce the hybrid-posture analysis — the partnership
   governance disciplines that make "participate *and*
   operate" honest rather than conflicted
4. Pre-wire the posture with CEO, CTO, CRO, General Counsel,
   Chief Trust Officer, and the business-unit leader
   responsible for the vertical

**Deliverables:**
- Ecosystem-position memo (8-10 pages)
- Partner-program or marketplace-operator design artifact
  (as applicable) — tiers, governance, listing policy,
  revenue share, de-listing authority
- Trust-and-safety governance document for third-party listings
  (if operating a marketplace)
- Board-facing ecosystem-strategy recommendation

**Success Criteria:**
- Ecosystem position is defensible to the organization's
  largest customers *and* to the Salesforce partner-team
  counterpart
- The hybrid posture (if chosen) has explicit, named
  governance disciplines that prevent conflict-of-interest
  escalations rather than discovering them in a dispute
- The marketplace-operator design (if chosen) has a tested
  listing-submission-to-approval workflow and a documented
  de-listing authority with named approver

---

### Case Study 3: An HSBC-Style Enterprise AI Partnership Portfolio Across the Stack

**Background:**
- Global financial-services organization with a shared AI
  platform ambition (see MOD-406 Case Study 3 for the
  infrastructure dimension) and a partnership portfolio that
  spans multiple hyperscalers, multiple frontier labs
  (via direct and hyperscaler-intermediated paths), multiple
  data vendors (market data, consumer data, labeled training
  data), and multiple systems-integration partners
- Financial-sector third-party-risk regulators (PRA SS2/21 and
  the UK Operational Resilience regime, EBA Outsourcing and
  ICT-Risk guidelines, EU DORA, OCC Third-Party Risk
  Management, HKMA TM-G-1 and third-party guidance, MAS
  outsourcing and technology risk guidance) each have their own
  expectations about load-bearing vendor identification,
  due-diligence evidence, contractual clause minima, exit
  planning, and incident-cooperation discipline
  <!-- needs-research: refresh current revision and effective
  dates for each named third-party-risk regime at time of use -->
- Workloads span credit decisioning (high-risk under EU AI
  Act, model-risk under PRA SS1/23 and SR 11-7), customer
  service (lower-risk, transparency-obligated), financial-
  crime screening (sector-overlay-heavy), and internal
  productivity
- Historic reality: the partnership portfolio is layered,
  multi-generation, and inconsistent — some workloads on
  standing-position contracts, some on legacy contracts, some
  on handshake arrangements with ambiguous SLAs

**Your Role:** Senior AI infrastructure architect, newly
chartered to produce the enterprise AI partnership-portfolio
posture and the clause-and-governance standardization plan,
reporting to the Group CIO with a dotted line to the Chief Risk
Officer, the Chief Compliance Officer, and the Head of Third-
Party Risk.

**Assignment:**
1. Produce a defensible enterprise AI partnership portfolio —
   named load-bearing partners, roles, contractual posture,
   governance tier, substitutability class, and concentration
   contribution — grounded in the organization's actual
   workload mix and regulatory footprint
2. Produce the standing-position clause set the organization
   will refuse to deploy AI workloads without, with named
   default / fallback / walk-away language on each clause,
   and the exception-approval pipeline
3. Design the partnership governance regime — tier structure,
   named sponsors, standing cadence, escalation ladder,
   scheduled-renegotiation cadence, exit plan per load-
   bearing partnership
4. Produce the partnership-portfolio contingency regime —
   dual-vendor, portability, weight / data / source escrow,
   transition-services commitments — with the specific
   workloads each contingency actually protects
5. Pre-wire the portfolio with CFO, CRO, CCO, Chief Trust
   Officer, General Counsel, Head of Third-Party Risk,
   business-unit CEOs, and the board risk committee

**Deliverables:**
- Enterprise AI partnership portfolio (15-20 pages)
- Standing-position clause set (concise reference artifact)
  and the gap-and-remediation plan against current contracts
- Partnership-governance model (tier structure, cadence,
  artifacts, named sponsors, escalation, scheduled
  renegotiation, exit)
- Partnership-portfolio contingency plan (named scenarios,
  tested exits, escrow and transition-services posture)
- Board-risk-committee communication pack
- Third-party-risk evidence mapping — demonstrating how the
  portfolio and clause set meet each named regulator's
  third-party-risk expectation

**Success Criteria:**
- Portfolio is defensible under the PRA / FCA / EBA / OCC /
  HKMA / MAS third-party-risk regimes simultaneously, under
  the EU AI Act provider-and-deployer role allocation, and
  under US competition-authority scrutiny of AI-specific
  partnerships
- Standing-position clause set has executive sign-off from
  General Counsel, Chief Trust Officer, and CPO, and is
  reflected in the organization's buying templates within
  the following quarter
- Contingency regime has tabletop-exercised at least two
  of the named scenarios before go-live
- The portfolio survives a leadership change, a visible
  vendor incident, and a regulatory enforcement action
  against a partner without the enterprise AI program being
  re-designed from scratch

---

## Exercises and Activities

The five exercises in `exercises/` are structured so each one feeds
the next. Treat them as a sequence, not a menu.

### Exercise 1: Case Study Analysis (3 hours)
Find a published AI-partnership case (HBR, Stanford, MIT,
primary-source joint announcement or 8-K / merger-filing from a
publicly disclosed AI alliance, or a published regulator
enforcement action or competition-authority inquiry involving
an AI partnership). Summarize, critique trade-offs, and apply
three lessons to your own organization.
See `exercises/exercise-01-case-study.md`.

### Exercise 2: 1-Page Strategy Memo (3 hours)
Write a 1-page memo to your CEO, CTO, CRO, Chief Trust Officer,
or board chair on a specific partnership investment — e.g.,
"Enter a multi-year strategic alliance with foundation-model
vendor X, with specific clauses on evaluation rights, exit,
and weight-custody for custom checkpoints," or "Deprecate and
exit the current systems-integration partner Y on the following
schedule, with named replacement partners for each workstream."
TL;DR, current state, recommendation, ask, risks, red-line
commitments.
See `exercises/exercise-02-strategy-memo.md`.

### Exercise 3: Stakeholder Map + Influence Plan (4 hours)
Map sponsors, supporters, neutrals, and blockers across CEO,
CFO, CTO, CRO, CISO, CPO, General Counsel, Chief Trust Officer,
Chief Communications Officer, Head of Procurement, Head of
Third-Party Risk, business-unit leaders, worker representation,
and at least one external stakeholder (partner executive
counterpart, regulator, government customer, investor).
Convert to a 90-day engagement plan with sequenced
conversations.
See `exercises/exercise-03-stakeholder-mapping.md`.

### Exercise 4: 3-Year Partnership Portfolio Roadmap (5 hours)
Draft a 3-year roadmap for the enterprise AI partnership
portfolio, broken into quarterly milestones. Each phase:
success metrics (concentration delta, contract-posture
coverage, governance-health, scenario-readiness coverage),
investment, key deliverables, and the specific partnership
portfolio delta over the prior quarter.
See `exercises/exercise-04-roadmap.md`.

### Exercise 5: Board-Level Presentation (5 hours)
A 10-slide deck for a board (or board risk / technology
committee) on the current state and forward plan of the
enterprise AI partnership portfolio, reviewed with a peer
using the "so what?" test at every slide.
See `exercises/exercise-05-presentation.md`.

---

## Assessment

### Module Quiz

Short strategic-thinking questions — no crisp right answers, defend
your position. See `quiz.md` for the full prompt list.

### Strategic Partnership Portfolio (8-10 hours)

A single coherent artifact set built around *one* enterprise AI
partnership portfolio you would design for a real (or realistic
composite) organization:

1. **Enterprise AI partnership portfolio** (15-20 pages,
   CFO- and CRO-approvable), with named load-bearing partners,
   roles, contractual posture, governance tier, and
   substitutability class
2. **Vendor-evaluation framework** (standing six-dimension
   due-diligence checklist, evidence artifacts, decision log,
   sign-off ladder)
3. **Contract-architecture playbook** (standing-position clause
   set, default / fallback / walk-away language, exception-
   approval pipeline, gap-analysis against current contracts)
4. **Partnership-governance model** (tier structure, cadence,
   artifacts, named sponsors, escalation ladder, scheduled-
   renegotiation cadence, exit plan per load-bearing
   partnership)
5. **Partnership-portfolio contingency plan** (named scenarios,
   dual-vendor positions, weight / data / source escrow,
   transition services, tested exits)
6. **Board-level status deck** (10-12 slides)

All six artifacts must describe the *same* AI partnership
portfolio and must be internally consistent. A reviewer should
be able to spot-check any two and find the same named partners,
the same contractual postures, the same governance tiers, and
the same contingency vocabulary.

**Evaluation Criteria:**
- **Internal coherence** (25%) — portfolio, evaluation
  framework, contract architecture, governance model,
  contingency plan, and board deck tell the same story at
  every altitude
- **Clause-posture rigor** (20%) — standing position holds up
  on the AI-specific clauses (input rights, output rights,
  IP indemnity, evaluation rights, residency, exit) rather
  than defaulting to a generic SaaS template
- **Counterparty and concentration realism** (15%) —
  portfolio treats affiliated counterparties (hyperscaler-lab
  entanglement, stacked partnership + investment structures)
  as material, not as a footnote
- **Governance realism** (15%) — governance model is
  something a real steering committee can run across time
  zones and leadership turnover, not an org chart
- **Executive communication** (15%) — board deck is
  answer-first, concentration and scenario readiness over
  vanity partner-count numbers
- **Right-sizing** (10%) — the portfolio fits the
  organization, neither alliance-theater nor an unmanaged
  procurement-line-item inventory

---

## Resources

### Required Reading

1. **Primary frameworks, standards, and law**
   - EU Regulation 2024/1689 (EU AI Act) — Articles 1-6,
     25 (provider / deployer / distributor / importer /
     authorised representative obligations), 50-55 (GPAI
     provider obligations and transparency), 85-99 (enforcement
     and fines)
     <!-- needs-research: confirm current application-date
     table and any delegated / implementing acts affecting
     the Article 25 role allocation at time of use -->
   - NIST AI 100-1 — *AI Risk Management Framework (AI RMF 1.0)*
   - NIST AI 600-1 — *Generative AI Profile*, with emphasis on
     third-party / supply-chain risk categories
   - ISO/IEC 42001 (AI management system) — third-party-AI and
     supplier-relationship clauses
     <!-- needs-research: confirm the specific clause citations
     at time of use -->
   - NIST SP 800-161 (Cybersecurity Supply Chain Risk
     Management) applied to AI vendor dependencies
   - Financial-sector third-party-risk regimes — OCC
     Third-Party Risk Management, EBA Outsourcing Guidelines,
     EBA ICT Risk Guidelines, EU DORA, UK PRA SS2/21 and the
     Operational Resilience regime, HKMA and MAS third-party
     guidance
     <!-- needs-research: confirm current revisions and
     effective dates at time of use -->

2. **Books and long-form references**
   - Chris Miller — *Chip War: The Fight for the World's Most
     Critical Technology* (reinforced from MOD-406; the
     supply-chain-as-partnership frame)
   - Anu Bradford — *Digital Empires: The Global Battle to
     Regulate Technology*
   - Andrew McAfee and Erik Brynjolfsson — *Machine, Platform,
     Crowd* (platform-economics background that underlies
     marketplace governance)
   - David Yoffie and Michael Cusumano — *Strategy Rules*
     (platform-and-ecosystem strategy, background for
     ecosystem-position decisions)
   - Deborah Ancona and Henrik Bresman — *X-Teams* (background
     on cross-organization team design, applied to joint
     working groups)

3. **Policy, industry, and technical reports**
   - Published strategic-AI-alliance announcements and 8-K
     filings (Microsoft-OpenAI, Amazon-Anthropic, Google-
     Anthropic, Oracle-OpenAI, NVIDIA investments in frontier
     labs, sovereign-vendor alliances)
     <!-- needs-research: refresh the current list of major
     publicly disclosed AI alliances with commitment scale and
     governance disclosures at time of use -->
   - Frontier Model Forum, Partnership on AI, AI Alliance,
     MLCommons / MLPerf public governance documents
     <!-- needs-research: refresh at time of use -->
   - CSET, CNAS, CSIS Wadhwani AI Center — published reports
     on AI industry structure, compute partnerships, and
     industrial-policy dimensions of AI partnerships
     <!-- needs-research: refresh current report lists at time
     of use -->
   - Published competition-authority inquiries and reports on
     AI-industry partnerships and investments (FTC 6(b), DOJ,
     UK CMA, European Commission, BKartA)
     <!-- needs-research: assemble a current short list at
     time of use -->
   - Primary-source AI-vendor trust centers, sub-processor
     lists, model cards, system cards, and usage policies for
     the counterparties in the organization's vendor stack

### Supplementary Resources

- Hyperscaler primary-source partner-program documentation
  (AWS Partner Network, Microsoft AI Cloud Partner Program,
  Google Cloud Partner Advantage, Oracle Partner Network,
  IBM Partner Plus)
  <!-- needs-research: refresh current partner-program
  structures at time of use -->
- Frontier-lab enterprise-partnership documentation (OpenAI
  Enterprise, Anthropic Enterprise and Partners, Google
  Cloud / Vertex AI partner materials, AWS Bedrock partner
  materials, Microsoft Azure OpenAI / Azure AI Foundry partner
  materials)
- Marketplace operator primary-source policies (Salesforce
  AppExchange / Agentforce, Microsoft AppSource, ServiceNow
  Store, AWS Marketplace / Bedrock Marketplace, Google Cloud
  Marketplace, OpenAI GPT Store, Anthropic app directory)
  <!-- needs-research: refresh listing, review, and revenue-
  share policies at time of use -->
- IAPP, Shared Assessments (SIG), and Cloud Security Alliance
  (CAIQ, CAIQ-AI) vendor-risk questionnaires as a floor for
  structured due diligence
  <!-- needs-research: confirm current questionnaire versions
  at time of use -->
- Published 10-K risk factors on AI vendor concentration,
  counterparty exposure, and competition / antitrust in AI
  from AI-heavy public companies
  <!-- needs-research: assemble a current short list -->
- AI Incident Database and Partnership on AI AI Incident
  Hub — partnership-adjacent incident patterns

See also `resources.md` in this module for the running reading list.

---

## Next Steps

Upon completing MOD-407, you will be prepared to:

1. **Produce and defend** an enterprise AI partnership portfolio
   across foundation-model, cloud, compute, data, platform,
   and services layers
2. **Classify** every load-bearing AI vendor relationship by
   role, substitutability, counterparty risk, and contractual
   posture
3. **Translate** foundation-model licensing terms, hyperscaler
   enterprise agreements, and systems-integrator master-service
   terms into a build / partner / resell / decline decision
4. **Negotiate** the AI-specific clauses — input and output
   rights, training-data warranties, IP indemnification,
   evaluation and audit rights, residency and operator-access,
   exit and transition — as a standing enterprise position
5. **Design** a partnership-governance regime that survives
   leadership change on either side
6. **Lead** the organization through a partnership crisis —
   pricing shift, change of control, trust incident,
   regulatory action, or vendor-dark scenario — with the
   regulator, workforce, customer, and board communications
   under time pressure
7. **Progress to MOD-408**: M&A and Technical Due Diligence,
   where partnership diligence deepens into acquisition
   diligence and post-merger integration

---

**Ready to begin?** Start with Week 1: The Partnership
Ecosystem Map and Vendor-Stack Inventory.

## Cross-references
- Engineering-level prerequisite: see ai-infra-engineer-learning + ai-infra-senior-engineer-learning
- Solutions repo: ai-infra-senior-architect-solutions/modules/mod-407-strategic-partnerships
