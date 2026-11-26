# MOD-408: M&A and Technical Due Diligence

**Level**: Senior Architect (Strategic / Executive)
**Duration**: 35-50 hours
**Prerequisites**: Architect-level experience; mod-401 (Enterprise AI Strategy); mod-403 (Enterprise Governance), mod-405 (Responsible AI), mod-406 (Global Infrastructure), and mod-407 (Strategic Partnerships) recommended

## Module Overview

This module is part of the Senior AI Infrastructure Architect curriculum
(level 400). Focus: M&A and technical due diligence of AI assets,
companies, and data estates.

Senior-architect modules emphasize executive communication, strategic
thinking, and organizational influence — not hands-on implementation.
For hands-on technical material on related topics (model-weight
packaging, dataset lineage tooling, evaluation harnesses, MLOps
migration), see the engineer-level and senior-engineer-level repos.

### Executive Summary

MOD-407 taught you to govern the counterparties the organization
*assembles* its platform from. MOD-408 asks the question that sits
one layer deeper: *what happens when the organization proposes to
buy a counterparty, sell a business unit that contains one, or
make a minority investment that will later pull it inside the
corporate boundary?* M&A is where every discipline in the previous
seven modules — strategy, executive leadership, governance, R&D,
responsible AI, global infrastructure, partnerships — is
simultaneously stress-tested against a counterparty whose
disclosures are limited, whose timeline is compressed, and whose
information asymmetry is structural.

At enterprise scale in 2026, AI assets rarely sit on their own:
they are entangled with training-data provenance that may or may
not be clean, model weights that may or may not be derivable or
redistributable, hyperscaler and model-vendor commitments that may
or may not transfer, open-source licenses whose compliance history
is uneven, researchers whose non-competes and retention economics
are the acquisition's actual value, and regulatory exposures that
travel with the asset into the acquirer's compliance perimeter
(EU AI Act obligations, GDPR Article 82 joint liability, sectoral
third-party-risk expectations, US state AI laws with private
rights of action). The senior architect's job in M&A is to
produce the technical diligence report the deal cannot close
without — the artifact that a CFO, a General Counsel, a Chief
Trust Officer, a CISO, and a board transaction committee can
each sign — and to produce it on a timeline measured in weeks,
not quarters.

At this level, AI M&A diligence is a program with six parts that
must co-exist: a **diligence framework** (the standing dimensions
and evidence artifacts across model, data, infrastructure, talent,
IP, regulatory, security, and commercial), a **valuation posture**
(how AI assets are valued, how diligence findings move price, and
how earn-outs and escrows absorb residual risk), a **deal-
structure vocabulary** (acquisition, acqui-hire, carve-out,
minority investment, joint venture, divestiture, and the diligence
emphasis that each shape calls for), an **integration or
separation plan** (the 100-day plan that makes the deal real —
or the TSA regime that makes the separation survivable), a
**regulatory and trust risk inheritance assessment** (what the
acquirer inherits that is not on the balance sheet), and an
**executive communication regime** (how the diligence findings
and integration risks are presented to the deal committee, the
board, the regulator, and — post-close — the acquired workforce).
A program with five of the six works until the sixth is tested,
and then it does not.

By the end of this module, you will be able to:

- Produce an AI-technical-diligence report that a CFO, CRO, Chief
  Trust Officer, General Counsel, CISO, and board transaction
  committee can each sign without a follow-on round of questions
- Classify any AI-era target on the deal-shape spectrum
  (acquisition of a platform, acqui-hire of a research team,
  carve-out of a product line, minority investment with option,
  joint venture) and lead the diligence emphasis each shape
  requires
- Translate diligence findings into deal-term consequences —
  purchase-price adjustment, representations and warranties, R&W
  insurance posture, escrow sizing, earn-out structure, closing
  conditions, walk-away rights
- Diligence AI-specific IP and data provenance — training-data
  sources, licensing, opt-out and removal-request history,
  derivative-model claims, contributor- and employee-assignment
  chains, open-source license compliance — to a standard that
  survives a post-close dispute
- Diligence AI-specific regulatory inheritance — EU AI Act role
  carry-over, GDPR joint-controller and data-transfer exposure,
  sectoral obligations, and US state AI law exposure (including
  private rights of action) — before the acquirer assumes it
- Design a 100-day post-close integration plan (or, for a carve-
  out or divestiture, a 12-to-24-month separation plan) that
  accounts for infrastructure, model inventory, data boundaries,
  talent retention, trust and safety, and public communications
- Communicate deal recommendations and integration risks to a
  transaction committee, a board, a regulator, government
  customers, and — post-close — the acquired workforce with the
  same vocabulary and the same numbers

---

## Learning Objectives

### The AI-M&A Landscape and Deal Shapes

1. **Why AI M&A is different from classical software M&A**
   - The asset is partly tacit (researcher skill, operational
     discipline, evaluation know-how) and partly opaque (data
     provenance that is not fully documented, model weights
     whose derivation chain is partial)
   - The regulatory perimeter travels with the asset in ways a
     SaaS acquisition historically did not — EU AI Act role
     obligations, GDPR-era data liability, FTC algorithmic-
     disgorgement precedent (Everalbum/Paravision 2021, WW/Kurbo
     2022, Amazon Alexa and Ring 2023, Rite Aid 2023, Avast 2024),
     sectoral regulator expectations
   - The competition-authority surface is active — the EC, CMA,
     DOJ, FTC, and BKartA have each opened AI-specific inquiries
     into partnerships and investments (CMA's Microsoft-OpenAI
     and Amazon-Anthropic reviews, the FTC's 6(b) staff report on
     AI cloud partnerships, and BKartA's Microsoft-Inflection
     review); an M&A transaction is a higher-friction version of
     the same scrutiny
   - The value is often in a small number of people, and those
     people have options; a diligence that does not price
     retention is incomplete

2. **The deal-shape spectrum**
   - **Acquisition of a platform** — the target is an operating
     business with revenue, customers, and a product; diligence
     emphasis on commercial, integration, and inherited regulatory
     obligation
   - **Acqui-hire** — the target is primarily a team; diligence
     emphasis on individual retention economics, non-compete and
     non-solicit enforceability, invention-assignment chains, and
     the specific projects the team is bringing out the door
   - **Carve-out acquisition** — the target is a subset of a
     larger seller; diligence emphasis on separation feasibility,
     the TSA scope the seller will support, and the IP and data
     boundaries that must be drawn
   - **Divestiture** — the organization is the seller; diligence
     emphasis on what the buyer will be told, what the
     organization is prepared to represent and warrant, and what
     stays behind
   - **Minority investment with option** — the organization takes
     a strategic stake with pre-emption or acquisition rights;
     diligence emphasis on governance (information rights, board
     seat, consent list) and on the trigger events that convert
     the option
   - **Joint venture or co-founded entity** — a separate legal
     vehicle; diligence emphasis on contribution IP, ongoing
     licensing, governance, and exit
   - **Asset deal vs. share deal** — the mechanical choice between
     buying the shares of the target entity (and inheriting
     everything) and buying only named assets (and leaving
     specific liabilities behind); the AI-era twist is that
     training-data provenance and model-weight derivation chains
     often require the share deal to be workable at all

3. **Minority investment, corporate VC, and the "optionality" deal**
   - Corporate-VC posture as a diligence-and-governance
     discipline — what information rights actually buy in
     practice, what consent-list items are worth negotiating, and
     the distinction between a seat and an observer
   - Pre-emption, right-of-first-refusal, and right-of-first-
     offer as the mechanics of future-deal optionality, and the
     way these interact with competition-authority sensitivities
     at the next round
   - The *stacked* structure — partnership + reseller + co-sell +
     equity — as the canonical AI-era alliance (reinforced from
     MOD-407), now read as the proto-M&A move it often becomes

### The Diligence Framework

4. **The AI-M&A diligence framework across eight dimensions**
   - *Commercial* — customers, pipeline, retention, contract
     quality, unit economics, revenue concentration, ARR quality,
     deferred-revenue hygiene, and the AI-specific "usage-
     consumption vs. subscription" revenue question
   - *Model* — model inventory, training recipe, evaluation
     evidence, safety and red-team history, fine-tuning posture,
     checkpoint inventory and provenance, dependence on third-
     party base models
   - *Data* — training-data sources, licensing chain, opt-out
     and removal-request history, synthetic-data provenance,
     evaluation-set construction, labeled-data provenance,
     residency posture
   - *Infrastructure and operations* — compute footprint,
     hyperscaler commitments, specialist-cloud and GPU-cloud
     contracts, observability and MLOps maturity, incident
     history, SLO attainment, cost base and controllability
   - *Talent* — key-person identification, retention economics,
     invention-assignment and non-solicit posture, visa and
     mobility profile, remote-work and jurisdictional spread
   - *IP, licensing, and open-source* — patent and trademark
     portfolio, open-source-license compliance history, model-
     license posture (Apache-2.0 / Llama-license /
     Qwen-license / Mistral-license / DeepSeek-license / BSL
     patterns), third-party dependency hygiene
   - *Regulatory and legal* — EU AI Act provider / deployer
     role, GDPR controller / processor posture, sectoral
     regulator exposure, US state AI law exposure, pending
     litigation, open regulator investigations, trust-and-safety
     incident history, consent-decree or settlement footprint
   - *Security and trust* — SOC 2 Type II, ISO/IEC 27001,
     ISO/IEC 42001, FedRAMP tier, HIPAA readiness,
     penetration-test history, incident history, responsible-
     disclosure track record, operator-access controls,
     subprocessor transparency

5. **Dimension interactions — the "the asset is clean along five axes but fatal along the sixth" failure mode**
   - A target with excellent model evaluations and a clean
     commercial book can still be un-ownable if its training-data
     chain contains non-opt-outable copyrighted material and the
     acquirer's jurisdiction does not have a TDM exception that
     covers it
   - A target with excellent data provenance can still be
     un-integrable if the two or three researchers who understand
     the training recipe are not retainable
   - A target with excellent talent can still be un-financeable
     if its hyperscaler commitment is a multi-year take-or-pay
     against which the acquirer's own enterprise discount
     structure cannot absorb the double-committed consumption
   - The diligence report's job is to find the dimension that
     breaks the deal, not to produce a clean-across-all-dimensions
     narrative

6. **Diligence-evidence artifacts — what "diligenced" actually means**
   - *Document-room artifacts* — model cards, system cards,
     evaluation reports, training-data inventories with per-
     source licensing, DPIAs, trust-center documents, SOC 2 Type
     II reports, pen-test reports, ISO/IEC 42001 certificate (if
     applicable), subprocessor list, breach register, open-
     regulator-inquiry register, OSS license audit output, SBOM
     for inference and training surfaces
   - *Management presentations* — the target's own framing of
     the above, read critically
   - *Expert sessions* — model-behavior deep-dives, data-chain
     walkthroughs, infrastructure-architecture reviews,
     T&S-incident postmortems
   - *Independent artifacts commissioned by the acquirer* —
     third-party model evaluation on buyer-provided data, third-
     party pen test, third-party data-lineage audit, third-party
     retention-economics assessment
   - *Site visits and operational observations* — code-review
     access on representative repositories (with the usual
     counsel-mediated clean-room discipline), incident runbook
     review, on-call rotation review
   - *Reference calls* — customers, departed employees,
     subprocessors, open-source counterparties

### Model and Data Diligence Specifics

7. **Model-estate diligence**
   - *Model inventory* — every model in production, pilot, and
     recent R&D, with version lineage and deprecation schedule;
     the "shadow model" problem (business units running models
     that do not appear in the central inventory)
   - *Training-recipe transparency* — the ability to reconstruct
     each production model from documented data and code; the
     "institutional-memory" risk when training recipe lives in
     two researchers' heads
   - *Dependence on third-party base models* — whether
     production models are fine-tuned from a licensed base
     (and under which license terms), distilled from a larger
     model (and whether that larger model's terms permit it),
     or trained from scratch
   - *Evaluation posture* — standardized benchmarks, in-
     production evaluation discipline, safety and hazard
     evaluations, third-party evaluation history, the
     organization's willingness to let the acquirer evaluate on
     acquirer-provided data (and the time cost that implies)
   - *Model-behavior equivalence under acquisition* — the risk
     that integration or vendor-stack changes under the acquirer
     silently move model behavior in production
   - *Weights, checkpoints, and adapters* — the inventory of
     every meaningful artifact, whether it is reproducible,
     whether it is redistributable, and whether the staff who
     produced it are under invention-assignment that survives
     departure

8. **Data-estate diligence**
   - *Training-data sources* — per-dataset provenance,
     licensing, opt-out and removal-request history, scraping
     vs. licensed-crawl vs. partner-supplied distinctions
   - *TDM and fair-use posture* — the acquirer's and the
     target's jurisdictional footprint against the EU DSM
     Directive Article 4 TDM-opt-out mechanics, the UK TDM
     exception, Japan Article 30-4, and the state of US fair-use
     litigation
   - *Content-license deals* — the licensed-corpus vendors the
     target depends on, the assignability of those agreements
     on change of control, and the renewal cost profile
   - *Evaluation-set construction* — whether evaluation sets
     are clean of training-data contamination, whether they are
     licensed for the use the target claims, and whether the
     evaluations are actually run on the stated schedule
   - *Labeled-data provenance* — the labeling vendors, worker-
     welfare commitments, contested-jurisdiction labor exposure,
     and the specific categories of label (consent-sensitive,
     medically sensitive, moderation-sensitive) that require
     their own diligence
   - *Residency and transfer* — where the training and
     inference data physically sits, what cross-border transfer
     mechanisms are in place (SCCs, Adequacy, DPF and successor
     frameworks), and the operator-access reality

9. **Derivative-model and output-rights diligence**
   - When the target's production models are fine-tuned from a
     licensed base, the specific terms the base-model license
     imposes on the fine-tuned artifact — redistribution,
     commercial use, attribution, acceptable-use, and "no
     training on competing base models" clauses
   - *Distillation* claims — whether the target's smaller models
     are distilled from larger third-party models under terms
     that permit distillation and the resulting commercial use
   - *Output-rights* history — whether the target's customers
     have an expectation of output ownership that constrains
     the acquirer's own template contracts
   - *Cross-customer training* commitments — whether the target
     has represented "no training on customer inputs" and
     whether its logging and retention actually conform

10. **Open-source and model-license diligence**
    - The target's OSS-license audit history — presence, cadence,
      and findings-remediation track record
    - Model-weight license exposure — Llama Community License,
      Qwen License, Mistral AI License, DeepSeek License,
      Apache-2.0 weights releases, BSL variants, OpenRAIL
      descendants — and the way each constrains redistribution,
      hosted-service offering, and derivative-model training
    - Dependency hygiene — SBOM presence and freshness for
      training and inference, known-vulnerability posture, the
      organization's response-time to published advisories
    - *License-incompatibility* findings that constrain the
      acquirer's intended integration path (GPL-adjacent
      obligations, patent-retaliation clauses, source-
      availability obligations)

### Infrastructure, Operations, and Commercial Diligence

11. **AI-infrastructure diligence**
    - Hyperscaler commitment profile — EDP / MACC / CUD
      structure, remaining term, remaining commit, double-
      commit risk after acquirer absorption
    - Specialist-cloud and GPU-cloud contracts — term, exit
      posture, and the specific reservation / co-location
      commitments that may or may not transfer
    - Observability, MLOps, and evaluation tooling — build
      quality, operator burden, and the integration cost of
      moving to the acquirer's standard stack
    - Capacity reality — the gap between contractually committed
      capacity and operationally available capacity, and the
      way "we have capacity reserved" becomes "we have a line
      item" when the acquirer joins the queue
    - Cost base — the per-request, per-token, per-GPU-hour
      unit economics that the acquirer will need to re-model
      under its own rate card

12. **Commercial and customer-base diligence**
    - Revenue quality — the usage-consumption share vs. the
      subscription share, the discounting history, the pipeline
      coverage and conversion, the enterprise-logo
      concentration
    - Customer-contract portability — the change-of-control
      clauses in the target's customer contracts, the
      assignment-consent posture of its largest customers,
      and the customer-side veto risk
    - Churn dynamics — gross and net retention, the specific
      cohorts that churn, the "pilot-to-production conversion"
      rate for AI deployments
    - Sales motion — who sells (ISV, SI, hyperscaler marketplace,
      direct), the commission plan, and the sales-team
      continuity risk in a change of control
    - Pipeline-realism — the pattern of booked revenue vs.
      committed-but-ramping revenue vs. aspirational pipeline,
      and the acquirer's ability to re-forecast under its own
      methodology

13. **Talent and key-person diligence**
    - Identification of key individuals — the two-to-twenty
      researchers, engineers, and operators whose departure
      materially damages the asset
    - Retention economics — current comp, equity vesting,
      refresh grants, retention-bonus structures in place, and
      the acquirer's own retention offer
    - Non-compete and non-solicit posture — what is enforceable
      in each relevant jurisdiction, and the specific countries
      and US states where the non-compete is effectively
      unavailable (California, North Dakota, Oklahoma, Minnesota,
      and — effective June 30, 2027 — Washington)
    - Invention-assignment and work-for-hire chains — the
      cleanliness of IP attribution from individual contributor
      to corporate entity, including the open-source
      contributions and public-benchmark history of senior
      researchers
    - Visa and mobility profile — the share of key talent on
      employer-sponsored status, the renewal exposure, and the
      integration implications of a legal-entity change
    - Public profile and reputational risk — the senior
      researchers' public positions on AI safety, policy, and
      ethics, and the reputational carry-over into the acquirer

### Regulatory, Trust, and IP Risk Inheritance

14. **Regulatory-inheritance diligence**
    - EU AI Act role carry-over — the target's provider or
      deployer role on each production system, the General-
      Purpose AI provider classification (if applicable), and
      the specific obligations the acquirer assumes on close
      (Article 25 entered into application on 2 August 2026,
      alongside the broader high-risk and governance block)
    - GDPR Article 82 joint-controller exposure — the target's
      historic data-controller decisions and the open claims
      they create
    - Sectoral regulator exposure — financial-services (PRA
      SS1/23 / SS2/21, SR 11-7, MAS and HKMA technology-risk,
      DORA), healthcare (HIPAA, FDA SaMD, EMA / MDR), critical
      infrastructure (CISA, NIS2, sector-specific regulators)
      — as applicable to the target's workloads
    - US state AI law exposure — the Colorado AI Act (revised
      by SB 26-189), the Texas Responsible AI Governance Act
      (effective 1 Jan 2026), California CPPA ADMT regulations
      (effective 1 Jan 2026), NYC Local Law 144, Illinois BIPA
      analogues, and the growing set of state employment /
      insurance / lending AI laws (with BIPA remaining the
      principal private-right-of-action risk in this set)
    - Export-control and sanctions exposure — the target's
      customer footprint against OFAC designations, the EAR
      Foreign Direct Product Rule reach, UK sanctions, EU
      restrictive measures, and the target's own compute
      supply chain

15. **Open-regulatory-inquiry and litigation diligence**
    - Open regulator investigations the target is party to
      (data-protection authority inquiries, FTC / DOJ /
      competition-authority preliminary inquiries, sectoral
      enforcement) — the "when did it start, what does the
      request-for-information actually say, who is responding"
      diligence
    - Pending litigation — IP-infringement claims (training-data
      litigation and model-output litigation), contract claims,
      privacy claims (BIPA and analogues), consumer-protection
      claims
    - Consent-decree and settlement footprint — the forward
      obligations the acquirer assumes by taking on the asset,
      including any outstanding algorithmic-disgorgement or
      model-deletion obligations (Rite Aid's five-year facial-
      recognition ban, Amazon Alexa's COPPA order, Ring's twenty-
      year privacy and security program, and Avast's data- and
      model-destruction obligations as representative examples)

16. **Trust-and-safety and incident-history diligence**
    - Incident register — the target's own record of T&S
      incidents, safety-evaluation failures, model-behavior
      regressions, and the remediation evidence
    - Classifier history — the posture, the enforcement
      cadence, and the escalation record on acceptable-use
      disputes
    - Red-team and safety-case artifacts — the specific
      hazards evaluated, the methodology, the external review
      (if any), and the disclosure practice
    - Public-facing policy history — the target's historic
      public statements on safety and responsible use, and the
      carry-over to the acquirer's own policy regime

17. **Security and trust diligence**
    - Standard enterprise security evidence — SOC 2 Type II,
      ISO/IEC 27001, ISO/IEC 42001 (where applicable), FedRAMP
      authorization, HIPAA attestation — read against the
      acquirer's own assurance posture
    - Breach register — the target's historic security
      incidents, their disclosure history, and the remediation
      follow-through
    - Operator-access controls — the target's own employee and
      contractor access to customer data and to production
      models, the just-in-time and privileged-access discipline,
      and the audit-trail completeness
    - Subprocessor transparency — the target's subprocessor
      list, the change-notification discipline, and the
      customer-contractual posture on subprocessor changes
    - Supply-chain security — the target's own model and
      dataset supply chain, backdoor and data-poisoning
      posture, and the cryptographic signing and provenance
      hygiene on shipped artifacts

### Valuation, Deal Mechanics, and Negotiation

18. **How diligence findings move the deal**
    - *Purchase-price adjustment* — the dollar consequence of
      a diligence finding, and the way it is expressed
      (base-price reduction, escrow holdback, specific
      indemnity, earn-out gating)
    - *Representations and warranties* — the AI-specific reps
      the acquirer demands (training-data lawfulness, model-
      provenance, OSS-license compliance, no-pending-regulatory-
      action beyond disclosed, no undisclosed consent-decree
      obligations, no undisclosed cross-customer training), and
      the knowledge qualifiers (seller's knowledge, actual
      knowledge of named individuals) that absorb negotiation
    - *R&W insurance* — the state of the market for AI-asset
      R&W policies, the exclusions that are standard in 2026
      (AI-specific IP litigation, open regulatory inquiries,
      training-data litigation), and the way the exclusion set
      drives the escrow sizing
    - *Escrow sizing* — the standard-market escrow against the
      standing-position escrow the acquirer needs for AI-asset-
      specific risks
    - *Earn-out structure* — the AI-era earn-out gates
      (retention of named researchers, migration milestones,
      evaluation-equivalence under integration, customer
      retention through change of control)
    - *Closing conditions* — the specific regulator approvals,
      customer consents, and third-party vendor consents that
      gate signing-to-closing

19. **Deal-term vocabulary for AI-specific risk**
    - *Fundamental reps* that survive indefinitely (title,
      authority, capitalization) vs. *general reps* with
      survival periods, as applied to AI-asset-specific reps
    - *Specific-indemnity* dollar carve-outs for identified
      risks (open litigation, open regulator inquiry, known
      OSS-license defect), separate from the general-indemnity
      basket
    - *Caps, baskets, and deductibles* — the dollar architecture
      of the indemnity, read against the diligence-finding
      profile
    - *Walk-away rights* — material-adverse-change (MAC) and
      specifically-defined-closing-condition failures as the
      acquirer's walk-away path
    - *Reverse-termination fees* and *break-up fees* — the
      acquirer's and the seller's exposure if the deal does
      not close
    - *Antitrust and regulatory-clearance* allocation — who
      bears the risk of a regulator-mandated remedy or a
      blocked transaction, and the hell-or-high-water vs.
      efforts-standard spectrum

20. **Deal-mechanics and process**
    - *Auction* vs. *negotiated* vs. *proprietary* deal
      processes, and the diligence depth each supports
    - *Signed-NDA document-room* mechanics, including the
      counsel-mediated clean-room regime for sensitive
      diligence streams (source code, pending litigation,
      competitively sensitive contracts, internal T&S
      incident records)
    - *Confirmatory diligence* — the post-exclusivity, pre-
      signing deep dive that closes the open items from
      preliminary diligence
    - *Antitrust and foreign-investment-review* pre-work —
      HSR, EC merger control, CMA merger control, CFIUS,
      and the equivalents in Japan, Korea, Germany, and the
      increasing number of jurisdictions with AI-sensitive
      review regimes (the UK NSIA 2021, which names AI as a
      mandatory-notification sector, and the revised EU FDI
      Regulation agreed in December 2025 are the current
      reference points)

### Integration, Separation, and Post-Close Execution

21. **The 100-day post-close integration plan for AI assets**
    - Day 1 — change of control: customer communication,
      employee communication, access and identity change, the
      "nothing changes today" narrative that must still be
      literally true in production
    - The first 30 days — diligence-finding closure, immediate
      retention execution, infrastructure-and-tooling dual-
      running validation, open-regulator-inquiry notification
    - The 31-60 days — integration-roadmap sign-off, product-
      roadmap reconciliation, early-indicator reporting on the
      retention and evaluation-equivalence KPIs
    - The 61-100 days — first integrated release cycle, first
      shared QBR, first board-level readout on integration
      status
    - The *integration committee* that owns this — standing
      membership from product, engineering, infrastructure,
      legal, HR, communications, and finance, with a named
      integration lead who is not simultaneously a line leader

22. **Model, data, and infrastructure integration**
    - Model-inventory consolidation — merging the target's
      inventory into the acquirer's, re-evaluating under the
      acquirer's standards, and the deprecation / retirement
      / re-licensing decisions each merged model forces
    - Data-estate integration — residency reconciliation,
      lineage integration, consent-record reconciliation,
      opt-out registry merger, and the deliberate choice of
      *not* integrating certain datasets where contamination
      risk exists
    - Infrastructure integration — compute-commitment
      rationalization, hyperscaler enterprise-agreement
      renegotiation, observability-and-MLOps consolidation,
      security-tooling consolidation
    - Evaluation-regime integration — adoption of a single
      evaluation standard across the merged inventory, and
      the explicit regression gate before the acquirer's
      brand applies to the target's products
    - *What not to integrate* — the deliberate "ring-fence"
      decisions, usually for regulatory, customer-contractual,
      or trust reasons

23. **Talent retention, cultural integration, and workforce communication**
    - Retention-grant sequencing — Day-1 grants vs. 30-day
      grants vs. 90-day grants vs. 12-month retention milestones
    - Role, title, and reporting-line clarity — the
      organization-chart decisions that must be made by Day 1,
      Week 2, and Day 30 at the latest
    - Compensation integration — the pay-band harmonization
      choice (lift to acquirer's bands, hold flat, blend), its
      budget cost, and its cultural signal
    - Equity-exchange and treatment of outstanding equity —
      the mechanics for vested and unvested equity in the
      target
    - Public-position carry-over — researchers' and executives'
      public writing, conference appearances, and policy
      positions, and the explicit conversation about continuity
      vs. harmonization
    - Workforce-communication cadence — the first all-hands
      (joint), the subsequent target-only sessions, the
      acquirer's own workforce briefing on integration, the
      anti-"rumor-mill" discipline

24. **Customer, partner, regulator, and public communication**
    - Customer communication — the pre-announce cadence to
      strategic accounts, the public announcement, the first-30-
      day customer-success sweep, and the specific messages for
      customers whose contracts have change-of-control triggers
    - Partner and vendor communication — reseller, SI,
      hyperscaler, and ISV counterparties, and the specific
      conversations each requires
    - Regulator communication — the home regulator, the sector
      regulator, and the data-protection authority briefings,
      and the specific cross-border notifications that attach
      to change of control
    - Public and industry communication — the press release,
      the industry-analyst briefing, the researcher community's
      read, and the explicit decision about whether the target
      brand is preserved, co-branded, sunset, or absorbed

25. **Divestiture and carve-out separation planning**
    - Separation-feasibility assessment — the "could the target
      stand alone in 12 to 24 months" question, read across
      infrastructure, data, model, talent, and commercial axes
    - *Transition-services agreement* (TSA) scope — the
      functions the seller continues to provide post-close, at
      what rate, for what term, with what sunset (AI-era TSAs
      typically extend beyond the classical finance / HR / IT
      scope to cover model-inference continuity, evaluation
      infrastructure, and MLOps tooling, though no canonical
      published norms exist)
    - Shared-infrastructure separation — the cost and timeline
      to carve a joint tenancy, a shared vector store, or a
      shared evaluation harness into two
    - Data-estate separation — the lineage reconstruction,
      consent-record split, residency split, and the
      documented provenance the buyer will need to operate
    - Model-estate separation — which checkpoints and adapters
      go with the carve-out, which remain, and how the
      derivation chain is proved to each side's satisfaction
    - Talent split — who goes with the carve-out, who stays
      with the seller, the retention mechanics for each cohort,
      and the non-solicit regime between the two future
      organizations
    - Customer-split logistics — the contract-assignment and
      novation mechanics, and the specific customer-side
      consent risk

### Portfolio-Level and Governance Perspectives

26. **The organization's M&A posture as a program**
    - A standing M&A playbook that does not re-invent process
      per deal — the named diligence streams, the standing
      evidence requirements, the standing deal-term positions,
      the named approvers at each gate
    - The *corporate development* function and its relationship
      to the senior AI architect — where the architect is
      consulted, where the architect decides, and where the
      architect's sign-off is a gate
    - The *investment-committee* model for AI-era deals, with
      standing membership (CFO, CTO, CSO, CRO, General Counsel,
      Chief Trust Officer, Head of Corporate Development, the
      senior AI architect), standing cadence, and standing
      decision-rights
    - The *deal-review* retrospective — the 12-month and 24-
      month look-back on each closed deal, against the
      diligence case and the integration plan, and the
      institutional-memory artifact it produces

27. **Board, committee, and executive communication**
    - The *transaction-committee* readout — the deal thesis,
      the diligence highlights, the material risks, the
      recommended deal terms, and the request for approval
    - The *board* readout — above the transaction committee,
      focused on the strategic rationale, the capital
      commitment, and the integration-risk profile
    - The *audit-committee* readout — on the financial-
      reporting and controls implications of the acquired
      asset, including the AI-specific controls inheritance
    - The *risk-committee* readout — on the concentration,
      regulatory-inheritance, and counterparty-risk
      consequences
    - The *regulator* briefings — pre- and post-close, with
      standing content on EU AI Act role succession, sectoral-
      regulator notification, and competition-authority
      clearance posture

28. **Governance through the deal lifecycle**
    - *Pre-signing* governance — the sponsor executive, the
      deal team, the approvals that gate a signed letter of
      intent, the information-barrier discipline when the
      target is a public counterparty or a known customer or
      partner
    - *Signing-to-closing* governance — the interim-operating
      covenants that constrain the target's behavior between
      signing and closing, and the acquirer's monitoring
      posture
    - *Post-closing* governance — the integration-committee
      cadence, the escalation ladder, the earn-out and
      retention-milestone review, the standing readout to the
      investment committee and the board
    - *Deal-review* governance — the scheduled 12-month and
      24-month retrospectives, with explicit "what did we get
      wrong in diligence" discipline

---

## Module Structure

```
mod-408-ma-due-diligence/
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

### Week 1: The AI-M&A Landscape and Deal-Shape Framework (6 hours)

**Topics:**
- Why AI M&A is different from classical software M&A — tacit
  assets, opaque data chains, regulatory perimeter that travels
  with the target, competition-authority sensitivity, retention
  as the actual value
- The deal-shape spectrum — acquisition, acqui-hire, carve-out,
  divestiture, minority investment, joint venture — and the
  diligence emphasis each shape calls for
- Asset deal vs. share deal in the AI era, and the training-
  data-provenance reasons the choice is often forced
- Minority investment, corporate VC, and the "optionality" deal
  as the proto-M&A move; the stacked partnership + equity
  structure (reinforced from MOD-407) as the canonical AI-era
  alliance that is sometimes an acquisition on a delay

**Readings:**
- Publicly disclosed AI acquisitions and their primary-source
  filings — press releases, 8-Ks, 10-Qs, and merger-filing
  narratives from recent transactions in the AI stack
  (Databricks-MosaicML, Microsoft-Inflection, Google-Character.AI,
  Amazon-Adept, and Nvidia's Run:ai and Gretel acquisitions are
  canonical reference points)
- Publicly disclosed strategic-alliance-to-acquisition paths
  (Microsoft-OpenAI structure and the public commentary on its
  "quasi-acquisition" character — including the CMA's March 2025
  conclusion that Microsoft exerts "material influence" but not
  control over OpenAI; Amazon-Anthropic, cleared by the CMA in
  September 2024; Google-Anthropic) as reference patterns
- Anu Bradford — *Digital Empires* (background on the
  regulatory and competitive frame in which AI M&A now
  operates; reinforced from MOD-407)
- Published competition-authority reports on AI-sector
  partnerships and acquisitions (the CMA's AI Foundation Models
  Update Paper of April 2024, the FTC's January 2025 6(b) staff
  report on AI-cloud partnerships, EC Phase I decisions, and CMA
  phase-1 / phase-2 narratives)

**Exercise:** Classify three recent AI transactions on the deal-
shape spectrum, state the diligence emphasis each would require,
and identify the single dimension on which each transaction
most plausibly turned. A one-page memo to the CEO. See
`exercises/exercise-01-case-study.md` for a structured version.

---

### Week 2: The Diligence Framework and Model / Data Diligence (8 hours)

**Topics:**
- The AI-M&A diligence framework across eight dimensions —
  commercial, model, data, infrastructure and operations,
  talent, IP and open-source, regulatory and legal, security
  and trust — as a standing checklist and a sequenced workflow
- Dimension interactions — the "the asset is clean along five
  axes but fatal along the sixth" failure mode, and the
  diligence discipline that surfaces it
- Model-estate diligence — inventory, training-recipe
  transparency, third-party base-model dependence, evaluation
  posture, behavior-equivalence under acquisition, weight-
  checkpoint-and-adapter inventory
- Data-estate diligence — training-data sources, TDM and fair-
  use posture, content-license deals, evaluation-set
  construction, labeled-data provenance, residency and
  transfer
- Derivative-model and output-rights diligence — license carry-
  through on fine-tuning, distillation posture, output-rights
  history, cross-customer training commitments
- Open-source and model-weight license diligence — OSS-license
  audit history, model-weight license exposure, dependency
  hygiene, license-incompatibility findings

**Readings:**
- NIST AI 600-1 — *Generative AI Profile* (reinforced from
  MOD-407), with emphasis on data-and-model supply-chain risk
  categories applied in diligence
- ISO/IEC 42001 — *AI management system* clauses on data,
  model, and supplier management (Clauses 6-10 of the main text
  and Annex A controls on data, lifecycle, use information, and
  third-party relationships), read as a diligence checklist
- NIST SP 800-161 Rev. 1 (Cybersecurity Supply Chain Risk
  Management, as updated November 2024) applied to AI-asset
  diligence, read alongside NIST AI 600-1 as the AI-specific
  supply-chain companion
- Primary-source model cards, system cards, training-data
  transparency summaries, and usage policies from the major
  foundation-model vendors, as the public floor for the
  diligence evidence a target should be able to produce on its
  own models
- Primary-source training-data litigation filings and
  dispositive rulings (NYT v. OpenAI, Getty v. Stability AI,
  Andersen v. Stability AI, Doe v. GitHub, and the music-label
  suits against Anthropic, Suno, and Udio as reference points)
- Model-weight license primary sources — Llama Community
  License, Qwen License, Mistral AI License, DeepSeek License,
  Apache-2.0 model-weight releases, BSL variants, OpenRAIL
  descendants — read against the target's own model-license
  posture, and against OSI's Open Source AI Definition (OSAID
  1.0, published October 2024) as the reference for whether
  a given release is genuinely open source or merely open-weight

**Case Study:** A large enterprise software vendor is evaluating
the acquisition of an AI-native startup whose production models
are fine-tuned from a mixture of open-weights base models (one
under the Llama Community License, one under Apache-2.0) and
whose training data is a mixture of licensed corpora and
scraped web data. The startup's evaluation suite is strong on
standardized benchmarks and thin on the buyer-provided
evaluation requested during diligence. Produce a two-page
diligence-risk memo identifying the three most material model-
and-data findings, the specific deal-term consequences each
implies (R&W, specific indemnity, escrow, earn-out, walk-away),
and the information requests the acquirer should make before
confirmatory diligence.

**Deliverable:** An AI-asset diligence framework (15-20 pages)
covering:
- The eight-dimension due-diligence checklist as applied to the
  organization's acquisition thesis
- Named evidence artifacts collected for each dimension, with
  the "what the target must produce," "what the acquirer must
  produce independently," and "what the acquirer must commission
  from a third party" split
- The decision log and sign-off ladder
- The counterparty-risk disclosure to the transaction committee
  and the board

---

### Week 3: Infrastructure, Operations, Commercial, and Talent Diligence (7 hours)

**Topics:**
- AI-infrastructure diligence — hyperscaler commitment profile,
  specialist-cloud and GPU-cloud contracts, observability-and-
  MLOps maturity, capacity reality vs. capacity on paper, cost
  base
- Commercial and customer-base diligence — revenue quality,
  customer-contract portability under change of control, churn
  dynamics, sales-motion continuity, pipeline realism
- Talent and key-person diligence — key-individual
  identification, retention economics, non-compete and
  non-solicit posture, invention-assignment chains, visa and
  mobility profile, public-profile reputational carry-over
- The *integration-cost* dimension — the diligence-time estimate
  of what it will cost to bring the target's infrastructure,
  operations, and people into the acquirer's standards; the
  "deal looked cheap until we modeled integration" failure mode

**Readings:**
- Primary-source hyperscaler enterprise-agreement terms and
  publicly posted standard-contract language on change of
  control and assignment (the AWS Customer Agreement, Microsoft
  Customer Agreement / EA, and Google Cloud Platform Terms of
  Service as the canonical references)
- Primary-source commercial-contract templates for AI-era
  change-of-control mechanics (the common variations of
  "consent required," "notice only," "deemed consent after N
  days" clauses)
- Published analyses of AI-sector retention economics, non-
  compete reform, and talent-market dynamics (CSET, Stanford
  HAI AI Index, Tortoise AI Index, published academic salary
  and mobility studies)
- The organization's own standing retention-economics data,
  as the benchmark against which target retention economics
  will be read
- Primary-source FTC non-compete rulemaking record and the
  state-by-state non-compete landscape (California, Minnesota,
  Oklahoma, North Dakota, and the evolving list)
  <!-- needs-research: refresh non-compete enforceability at
  time of use; this is an active regulatory and litigation
  frontier -->

**Exercise:** For a hypothetical acquisition of an AI-native
startup, produce a one-page retention-economics memo covering:
- The named key individuals (two-to-twenty)
- The acquirer's retention-grant proposal for each cohort
- The non-compete and non-solicit posture in each relevant
  jurisdiction
- The integration-risk profile if the top-three retention
  targets depart within 12 months
See `exercises/exercise-02-strategy-memo.md` for a structured
version.

**Deliverable:** An infrastructure-operations-commercial-and-
talent diligence playbook (12-15 pages) covering:
- The standing diligence requests on each dimension
- The evidence artifacts and the cross-check sources
- The named-approver and sign-off ladder
- The integration-cost estimate methodology and the sensitivity
  analysis

---

### Week 4: Regulatory, Trust, and IP Risk Inheritance (6 hours)

**Topics:**
- Regulatory-inheritance diligence — EU AI Act role carry-over,
  GDPR joint-controller exposure, sectoral regulator exposure,
  US state AI law exposure (including private rights of
  action), export-control and sanctions exposure
- Open-regulatory-inquiry and litigation diligence — the
  active inquiries, the pending cases, the consent-decree and
  settlement footprint with ongoing compliance obligations
- Trust-and-safety and incident-history diligence — the
  target's T&S register, classifier history, red-team posture,
  public-facing policy history
- Security and trust diligence — standard enterprise security
  evidence against the acquirer's assurance posture, breach
  register, operator-access controls, subprocessor
  transparency, supply-chain security on model and dataset
  artifacts
- The "what the acquirer inherits that is not on the balance
  sheet" discipline — the register of risks that do not show
  up as a line item but become operational and reputational
  obligations on close

**Readings:**
- EU Regulation 2024/1689 (EU AI Act) — Articles 1-6, 25
  (provider / deployer / distributor / importer / authorised
  representative obligations, including role succession on
  change of control), 50-55 (GPAI provider obligations and
  transparency), 85-99 (enforcement and fines) — read as a
  diligence checklist for role-carry-over
  <!-- needs-research: confirm current application-date table
  and any delegated / implementing acts affecting Article 25
  role allocation at time of use -->
- NIST AI 100-1 — *AI Risk Management Framework (AI RMF 1.0)*
  as the common vocabulary the diligence report uses for
  governance, map, measure, manage
- US state AI law primary sources — Colorado AI Act, California
  ADMT regulations, NYC Local Law 144, Illinois BIPA, and the
  state employment / insurance / lending AI laws with private
  rights of action
  <!-- needs-research: refresh US state AI law effective dates
  and private-right-of-action scope at time of use -->
- Financial-sector third-party-risk regimes — OCC Third-Party
  Risk Management, EBA Outsourcing Guidelines, EU DORA, UK PRA
  SS2/21, HKMA and MAS technology-risk guidance — as they
  apply to AI assets acquired into a regulated financial-
  services entity (reinforced from MOD-407)
  <!-- needs-research: refresh current revisions and effective
  dates at time of use -->
- Primary-source FTC algorithmic-disgorgement orders (Everalbum,
  Rite Aid, WW/Kurbo and successors) and their consent-decree
  obligations as the pattern the acquirer may inherit
  <!-- needs-research: refresh the FTC algorithmic-disgorgement
  catalog at time of use -->
- Primary-source training-data litigation filings and rulings,
  read specifically for what-the-acquirer-inherits
  <!-- needs-research: refresh pending and decided AI
  training-data litigation at time of use -->

**Case Study:** Your organization is evaluating the acquisition
of a healthcare-adjacent AI company whose products are deployed
across the EU, the UK, Canada, and ten US states, whose
training data was assembled between 2019 and 2024 from a
mixture of licensed clinical corpora, publicly available
research, and vendor-supplied datasets (two of which have since
had vendor-side provenance disclosures), and whose open
regulatory interactions include one EU data-protection-authority
inquiry and one US state-attorney-general request for
information. Produce a two-page regulatory-and-trust-risk-
inheritance memo for the transaction committee, identifying
the three most material inheritance risks, the deal-term
consequences each implies, and the specific information
requests to the target before close.

**Deliverable:** A regulatory-and-trust-risk-inheritance report
(10-15 pages) covering:
- The EU AI Act role-carry-over analysis per production system
- The GDPR, sectoral, and US state AI law exposure analysis
- The open-regulatory-inquiry and litigation analysis
- The T&S incident-history and consent-decree footprint
- The deal-term consequences (reps, specific indemnity, escrow,
  closing conditions, walk-away)

---

### Week 5: Valuation, Deal Mechanics, and Negotiation (7 hours)

**Topics:**
- How diligence findings move the deal — purchase-price
  adjustment, R&W, R&W insurance, specific indemnity, escrow,
  earn-out structure, closing conditions, walk-away rights
- Deal-term vocabulary for AI-specific risk — fundamental vs.
  general reps and their survival periods, caps and baskets,
  specific-indemnity carve-outs, MAC and walk-away, reverse-
  termination and break-up fees, antitrust-and-regulatory-
  clearance allocation
- Deal mechanics and process — auction vs. negotiated vs.
  proprietary, document-room mechanics, counsel-mediated
  clean-room discipline, confirmatory diligence, antitrust and
  foreign-investment-review pre-work (HSR, EC, CMA, CFIUS,
  Japan / Korea / Germany / growing set)
- The AI-era R&W insurance market — the standard exclusions in
  2026 (AI-specific IP litigation, open regulatory inquiries,
  training-data litigation), and the way the exclusion set
  drives the escrow architecture
- Negotiation choreography — procurement, legal, security,
  trust-and-safety, business-unit, and executive sequencing;
  avoiding the "term-sheet signed before T&S reviewed it"
  failure mode (reinforced from MOD-407)

**Readings:**
- American Bar Association — *Model Stock Purchase Agreement
  with Commentary* and the equivalent *Model Asset Purchase
  Agreement* as the baseline template vocabulary
  <!-- needs-research: confirm current edition and any
  AI-specific supplements at time of use -->
- Published R&W insurance market reports on AI-asset coverage,
  standard exclusions, and premium trends
  <!-- needs-research: refresh current R&W insurance market
  posture on AI-asset coverage at time of use -->
- Primary-source HSR, EC merger control, CMA merger control,
  and CFIUS guidance on AI-sensitive transactions
  <!-- needs-research: refresh current AI-sensitive foreign-
  investment-review regimes and any AI-specific merger-
  notification thresholds at time of use -->
- Published AI-M&A deal tear-downs from major law firms (the
  "what moved in the merger agreement" summaries typically
  published quarterly) — read for AI-specific clause evolution
  <!-- needs-research: assemble a current short list of AI-M&A
  deal tear-downs at time of use -->
- Barbara Minto — *The Pyramid Principle* (reinforced from
  MOD-402 and MOD-407) for the deal-memo and investment-
  committee-paper structure

**Exercise:** Draft the acquirer's standing-position deal-term
set as a one-page internal reference — the AI-specific reps,
the specific-indemnity carve-outs, the standing escrow sizing,
the standing earn-out structure, and the walk-away triggers.
See `exercises/exercise-03-stakeholder-mapping.md` for a
structured version that also covers stakeholder sequencing.

**Deliverable:** A deal-mechanics playbook (12-15 pages) covering:
- The standing-position AI-specific reps with default /
  fallback / walk-away language
- The standing specific-indemnity carve-outs for identified
  AI-asset risks
- The standing R&W-insurance posture against the exclusion set
- The standing escrow and earn-out architecture
- The standing walk-away triggers (MAC, closing-condition
  failure, specifically-defined termination events)
- The named standing-position reviewer (typically General
  Counsel + Chief Trust Officer + CFO + Head of Corporate
  Development) and the review cadence

---

### Week 6: Integration, Separation, and Deal Governance (8 hours)

**Topics:**
- The 100-day post-close integration plan for AI assets — Day
  1 change-of-control choreography, 30-day diligence-finding
  closure and retention execution, 60-day integration-roadmap
  sign-off, 100-day first-integrated-release-cycle
- Model, data, and infrastructure integration — inventory
  consolidation, residency and lineage reconciliation,
  compute-commitment rationalization, evaluation-regime
  integration, deliberate ring-fence decisions
- Talent retention, cultural integration, and workforce
  communication — retention-grant sequencing, role / title /
  reporting-line clarity, compensation integration, equity
  exchange, public-position carry-over, workforce-communication
  cadence
- Customer, partner, regulator, and public communication —
  strategic-account pre-announce, public announcement, 30-day
  customer-success sweep, partner and vendor cascading,
  regulator briefings, industry-analyst engagement
- Divestiture and carve-out separation planning — separation-
  feasibility assessment, TSA scope, shared-infrastructure
  separation, data- and model-estate separation, talent and
  customer split
- Deal-lifecycle governance — pre-signing, signing-to-closing,
  post-closing, and 12-/24-month deal-review retrospective

**Readings:**
- Gary Klein, HBR — "Performing a Project Premortem"
  (reinforced from MOD-402, MOD-404, MOD-406, MOD-407;
  applied to the integration-plan and separation-plan
  scenario set)
- Published post-merger-integration literature — HBS cases on
  software and technology integrations, HBR practitioner
  articles on talent retention, consulting-firm reports on
  integration-value-capture
- Primary-source 10-K and 10-Q disclosures on integration
  progress and purchase-accounting adjustments for recent
  AI-sector acquisitions
  <!-- needs-research: refresh integration-disclosure examples
  at time of use -->
- Published TSA templates and practitioner guides for
  technology carve-outs, read specifically for the AI-era
  additions on inference services, evaluation infrastructure,
  and MLOps tooling
  <!-- needs-research: refresh the AI-era TSA norms at time
  of use -->
- Primary-source regulator guidance on change-of-control
  notification and succession (data-protection authorities,
  sectoral regulators, EU AI Act market-surveillance
  authorities as they come online)
  <!-- needs-research: refresh EU AI Act market-surveillance
  authority designations and change-of-control notification
  expectations at time of use -->

**Scenario:** On a Thursday afternoon, the acquirer's
transaction committee has approved a definitive agreement to
acquire a mid-sized AI company; the public announcement is
scheduled for the following Tuesday, with close targeted 90-
to-120 days out pending HSR, EC and CMA merger clearance, and
two customer-side change-of-control consents from strategic
accounts. The target's two most senior researchers are
unknown to the acquirer's own technical leadership and have
public profiles; the target has one open EU data-protection-
authority inquiry and one pending US class-action training-
data suit. Draft:
- 1-page transaction-committee approval memo (strategic
  rationale, diligence summary, material risks, deal terms,
  approval ask)
- 1-page board-briefing update on announcement day
- Day-1 workforce communication (acquirer and target, with
  shared and separate elements)
- Day-1 customer communication (public template and named-
  account scripts for the two change-of-control-sensitive
  customers)
- Regulator notification set (data-protection authority,
  sectoral regulator, EU AI Act market-surveillance authority
  equivalents in the target's operating jurisdictions)
- 100-day integration-plan outline with named owners and the
  three KPIs the board will see at the first readout
- Deal-review retrospective template to be used at 12 and 24
  months

**Exercise:** Board-level presentation on the acquirer's
current AI-M&A pipeline and the posture adjustments the
diligence program recommends for the next four quarters. See
`exercises/exercise-05-presentation.md`.

**Deliverable:** Board-ready deck (10-15 slides) on the
organization's AI-M&A program — pipeline, standing diligence
posture, standing deal-term posture, standing integration
posture — reviewed with a peer using the "so what?" test at
every slide.

---

## Case Studies

### Case Study 1: A Platform Acquisition of an AI-Native SaaS Company

**Background:**
- A large enterprise-software incumbent is acquiring an AI-
  native SaaS vendor with ARR in the low-hundreds-of-millions,
  a customer base concentrated in financial services and
  healthcare, a production model estate built partly from
  open-weights base models and partly from in-house training,
  and a talent base of roughly 150 people with heavy
  concentration in two research teams
- The target's data provenance is mixed — licensed corpora,
  vendor-supplied datasets with partial provenance disclosure,
  and a smaller but non-zero scraped-content layer
- The target's hyperscaler footprint is a multi-year commit
  with a single hyperscaler whose own enterprise discount
  program the acquirer also runs under
- The target has one open EU data-protection-authority inquiry
  (status: request for information, no finding), no pending
  US litigation, and a published trust posture that matches
  the acquirer's own

**Your Role:** Senior AI infrastructure architect leading the
technical diligence stream, reporting into the deal lead on
the acquirer side, with a dotted line to the CTO and the
transaction-committee chair.

**Assignment:**
1. Produce a current-state technical-diligence report across
   the eight dimensions — commercial, model, data,
   infrastructure and operations, talent, IP and OSS,
   regulatory and legal, security and trust
2. Identify the three dimensions on which the diligence
   findings are material to the deal, the specific deal-term
   consequences each implies (R&W, specific indemnity, escrow,
   earn-out, closing conditions, walk-away), and the
   confirmatory-diligence requests that remain open
3. Produce the 100-day integration plan — model-inventory
   consolidation, data-estate residency and lineage
   reconciliation, hyperscaler commit rationalization,
   retention execution, customer and workforce communication,
   regulator notification
4. Pre-wire the plan with CFO, CTO, CRO, CISO, Chief Trust
   Officer, General Counsel, Head of Corporate Development,
   and the business-unit leader who will own the acquired
   product line

**Deliverables:**
- Technical-diligence report (20-25 pages)
- Deal-term consequence memo (5-7 pages)
- 100-day integration plan (10-15 pages)
- Transaction-committee approval memo (1-2 pages)
- Board-briefing update deck for announcement day (6-8 slides)

**Success Criteria:**
- Diligence is defensible under an external post-close review,
  including the "what did we get wrong" retrospective at 12
  and 24 months
- Deal-term consequence memo is specific and testable
  (named escrow dollar figure, named earn-out gates, named
  specific-indemnity carve-outs), not "we recommend prudent
  protections"
- Integration plan has named owners and named KPIs the board
  will see at the first readout
- Retention program holds the top-three researchers through
  12 months at a defensible cost

---

### Case Study 2: An Acqui-Hire of a Research Team with a Partial Open-Weights Release

**Background:**
- A frontier-adjacent lab is being wound down by its lead
  investor; the acquirer has agreed to a structured acqui-
  hire of the lab's twelve core researchers and engineers,
  the lab's internal evaluation harness, and specific model
  checkpoints; the lab's public open-weights releases will
  remain public and the acquirer will not acquire them
- The twelve individuals are distributed across the US, the
  UK, Canada, and Germany; two are on employer-sponsored US
  visas; three have public profiles with active conference
  and policy engagements
- Non-competes are unavailable or unreliable in four of the
  relevant jurisdictions; non-solicits are enforceable to
  varying degrees in each
- The lab's evaluation harness contains third-party test
  sets whose licensing posture does not clearly permit the
  commercial use the acquirer intends
- The lab's public releases have been downloaded widely and
  have at least one known downstream commercial deployment;
  the responsibility for ongoing acceptable-use enforcement
  of those releases is a live question

**Your Role:** Senior AI infrastructure architect leading the
technical diligence for the acqui-hire, with a dotted line to
the Chief People Officer (on retention economics) and the
General Counsel (on IP and public-release legacy).

**Assignment:**
1. Produce a diligence report scoped to acqui-hire
   economics and IP transfer — retention, non-compete /
   non-solicit, invention-assignment cleanliness, evaluation-
   harness-license posture, acquired-checkpoint-license posture,
   public-release legacy responsibility
2. Identify the three dimensions on which the structure is
   most sensitive — retention, evaluation-harness-license,
   public-release-legacy — and the specific deal mechanics
   that address each (Day-1 and 90-day retention grants,
   license-re-acquisition plan, public-release governance
   statement)
3. Produce the integration plan for the twelve individuals —
   role, title, reporting line, compensation, equity exchange,
   visa support, and the first-30-days communication plan,
   including continuity of public engagements
4. Pre-wire the structure with CPO, CTO, General Counsel,
   Chief Trust Officer, and the research-leader who will
   receive the acqui-hired team

**Deliverables:**
- Acqui-hire diligence report (10-15 pages)
- Retention-economics plan with named grants and vesting
- Evaluation-harness and checkpoint license remediation plan
- Public-release legacy governance statement (1-2 pages)
- Integration plan for the twelve individuals (5-7 pages)
- Transaction-committee approval memo (1-2 pages)

**Success Criteria:**
- Retention program holds at least ten of the twelve
  through 12 months
- Evaluation-harness license remediation is complete within
  six months of close, with named replacement artifacts where
  re-licensing is not feasible
- Public-release legacy posture is explicit and defensible
  to the research community and to downstream deployers
- The structure survives a regulator question on non-compete
  reliance in any of the four relevant jurisdictions

---

### Case Study 3: A Carve-Out Divestiture of an AI Product Line from a Diversified Technology Company

**Background:**
- A diversified technology company is divesting its AI
  developer-tools product line to a private-equity-backed
  consolidator; the carve-out includes the product, the
  hosted-inference platform, the evaluation infrastructure,
  roughly 220 employees, and the product's customer book
- The product has been running on shared infrastructure
  with the seller's broader platform — a shared vector
  store, a shared observability stack, and a shared model-
  serving layer — none of which will transfer; separation
  will require a TSA on specific components for 18 months
- The product's training-data heritage includes contributions
  from the seller's broader data estate that will not
  transfer; the buyer will need either licensed replacement
  data or an engineering plan to operate without
- The product operates in the EU under a specific EU AI Act
  role allocation that will change on the carve-out; the
  seller's harmonized sub-processor list will fragment
- The seller's employees to be transferred include members
  of a shared research team whose work spans the product
  being divested and products being retained; the
  individual-level assignment must be negotiated
- The seller's customer contracts include change-of-control
  provisions of varying strength, several with strategic
  accounts who will need to be pre-wired

**Your Role:** Senior AI infrastructure architect on the
*seller* side, responsible for producing the technical
disclosures the buyer will diligence and for designing the
separation and TSA structure.

**Assignment:**
1. Produce the carve-out disclosure package — model inventory,
   data-estate inventory with the specific "transfers / does
   not transfer / needs replacement" tagging, infrastructure
   inventory with the "shared / dedicated / TSA" tagging,
   talent roster with the proposed individual-level assignment,
   customer-book summary with the change-of-control-sensitivity
   tagging, open-regulator-inquiry register, OSS-license audit
2. Produce the separation-feasibility assessment — the "can
   the product stand alone in 18 months" question across
   infrastructure, data, model, talent, and commercial axes —
   with the seller's defensible answer and the TSA scope that
   makes the answer honest
3. Produce the TSA proposal — the specific components,
   rates, terms, and sunset schedule; the EU AI Act role
   succession plan; the regulator and customer notification
   cadence
4. Pre-wire the carve-out with CFO, CTO, CRO, General Counsel,
   CPO, Chief Trust Officer, and the business-unit leader
   whose product line is being divested

**Deliverables:**
- Carve-out disclosure package (20-25 pages)
- Separation-feasibility assessment (10-15 pages)
- TSA proposal (10-15 pages)
- Regulator and customer notification pack
- Transaction-committee approval memo (on the seller side)
- Board-briefing update deck

**Success Criteria:**
- Disclosure package is complete enough that the buyer's
  confirmatory diligence does not produce a material
  surprise and a price re-cut
- Separation-feasibility assessment survives a buyer-side
  technical diligence challenge on whether the TSA scope
  is sufficient
- TSA proposal is operationally honest — the seller's team
  can actually deliver the services at the stated rate and
  schedule
- EU AI Act role succession plan is defensible to the
  market-surveillance authority
- Customer notification pack holds the two most change-of-
  control-sensitive customers through close

---

## Exercises and Activities

The five exercises in `exercises/` are structured so each one feeds
the next. Treat them as a sequence, not a menu.

### Exercise 1: Case Study Analysis (3 hours)
Find a published AI M&A transaction (an 8-K, merger filing,
primary-source joint announcement, or a regulator decision on
an AI-sector merger review). Summarize, critique trade-offs,
and apply three lessons to your own organization's prospective
M&A pipeline.
See `exercises/exercise-01-case-study.md`.

### Exercise 2: 1-Page Strategy Memo (3 hours)
Write a 1-page memo to your CEO, CFO, Chief Trust Officer, or
board chair on a specific M&A posture decision — e.g.,
"Acquire target X at the term sheet circulated, subject to the
three diligence-finding-driven deal-term adjustments described,"
or "Decline the acqui-hire opportunity in favor of a research-
collaboration structure with the team's institution," or
"Proceed with the carve-out divestiture of product-line Y on
the schedule and TSA scope described." TL;DR, current state,
recommendation, ask, risks, red-line commitments.
See `exercises/exercise-02-strategy-memo.md`.

### Exercise 3: Stakeholder Map + Influence Plan (4 hours)
Map sponsors, supporters, neutrals, and blockers across CEO,
CFO, CTO, CRO, CISO, CPO, General Counsel, Chief Trust Officer,
Chief Communications Officer, Head of Corporate Development,
Head of Third-Party Risk, business-unit leaders, worker
representation, and at least one external stakeholder (target-
side executive counterpart, strategic customer, regulator,
competition authority, investor). Convert to a 90-day
engagement plan with sequenced conversations through the
pre-signing, signing-to-closing, and post-close phases.
See `exercises/exercise-03-stakeholder-mapping.md`.

### Exercise 4: 3-Year M&A Program Roadmap (5 hours)
Draft a 3-year roadmap for the organization's AI-M&A program,
broken into quarterly milestones. Each phase: success metrics
(diligence coverage, deal-term-posture adherence, integration-
value-capture against the deal model, retention of named
individuals, regulator-inquiry burn-down), investment, key
deliverables, and the specific program delta over the prior
quarter.
See `exercises/exercise-04-roadmap.md`.

### Exercise 5: Board-Level Presentation (5 hours)
A 10-slide deck for a board (or board transaction / audit /
risk committee) on the current state and forward plan of the
enterprise AI-M&A program — pipeline, standing diligence
posture, standing deal-term posture, standing integration
posture — reviewed with a peer using the "so what?" test at
every slide.
See `exercises/exercise-05-presentation.md`.

---

## Assessment

### Module Quiz

Short strategic-thinking questions — no crisp right answers, defend
your position. See `quiz.md` for the full prompt list.

### Strategic AI-M&A Diligence Portfolio (8-10 hours)

A single coherent artifact set built around *one* AI-M&A
transaction you would lead for a real (or realistic composite)
organization:

1. **Technical-diligence report** (20-25 pages, CFO- and CRO-
   approvable), across the eight dimensions, with named evidence
   artifacts, named findings, and named deal-term consequences
2. **Deal-term playbook** (standing-position AI-specific reps,
   specific-indemnity carve-outs, R&W-insurance posture, escrow
   and earn-out architecture, walk-away triggers)
3. **Regulatory-and-trust-risk-inheritance report** (EU AI Act
   role carry-over, GDPR and sectoral exposure, US state AI law
   exposure, open-inquiry and litigation posture, consent-decree
   footprint)
4. **100-day integration plan** (model, data, infrastructure,
   talent, customer, regulator, workforce), with named owners
   and the three KPIs the board will see at the first readout
5. **Carve-out / separation plan** *or* **divestiture
   disclosure package** (depending on deal shape), if the
   chosen transaction is a carve-out or divestiture
6. **Transaction-committee approval memo** and **board-briefing
   update deck** (10-12 slides) for announcement day and the
   first post-close readout

All six artifacts must describe the *same* AI-M&A transaction
and must be internally consistent. A reviewer should be able
to spot-check any two and find the same named findings, the
same deal-term consequences, the same integration or
separation vocabulary, and the same named owners.

**Evaluation Criteria:**
- **Internal coherence** (25%) — diligence report, deal-term
  playbook, regulatory-inheritance report, integration /
  separation plan, and executive communication tell the same
  story at every altitude
- **Diligence rigor** (20%) — the eight-dimension coverage is
  specific and evidence-backed, not generic checklist narration;
  the "dimension that breaks the deal" analysis is explicit
- **Deal-term realism** (15%) — standing-position reps,
  specific indemnities, R&W-insurance posture, escrow and
  earn-out architecture are grounded in current market practice
  rather than invented
- **Regulatory-inheritance realism** (15%) — EU AI Act,
  GDPR, sectoral, and US state AI law exposure is treated as
  material and specific to the target's workload mix, not
  footnoted
- **Integration / separation realism** (15%) — the 100-day
  plan (or separation plan) is something a real integration
  committee can execute across time zones, leadership
  transitions, and competing priorities
- **Executive communication** (10%) — transaction-committee
  memo and board-briefing deck are answer-first, with the
  three material risks and the deal-term responses on the
  first page

---

## Resources

### Required Reading

1. **Primary frameworks, standards, and law**
   - EU Regulation 2024/1689 (EU AI Act) — Articles 1-6, 25
     (provider / deployer / distributor / importer / authorised
     representative obligations, including role succession on
     change of control), 50-55 (GPAI provider obligations and
     transparency), 85-99 (enforcement and fines)
     <!-- needs-research: confirm current application-date table
     and any delegated / implementing acts affecting Article 25
     role allocation at time of use -->
   - NIST AI 100-1 — *AI Risk Management Framework (AI RMF 1.0)*
   - NIST AI 600-1 — *Generative AI Profile*, with emphasis on
     third-party / supply-chain risk categories applied in
     diligence
   - ISO/IEC 42001 (AI management system) — data, model,
     and supplier-relationship clauses
     <!-- needs-research: confirm specific clause citations and
     any published implementation guides at time of use -->
   - NIST SP 800-161 (Cybersecurity Supply Chain Risk
     Management) applied to AI vendor and acquisition
     dependencies
   - US state AI laws with change-of-control implications —
     Colorado AI Act, California ADMT regulations, NYC Local
     Law 144, Illinois BIPA, and the growing state employment /
     insurance / lending AI laws
     <!-- needs-research: refresh US state AI law effective
     dates and private-right-of-action scope at time of use -->
   - Financial-sector third-party-risk regimes — OCC Third-
     Party Risk Management, EBA Outsourcing Guidelines, EU
     DORA, UK PRA SS2/21, HKMA and MAS technology-risk
     guidance — as they apply to AI assets acquired into a
     regulated financial-services entity
     <!-- needs-research: confirm current revisions and
     effective dates at time of use -->
   - HSR, EC merger control, CMA merger control, CFIUS, and
     equivalent foreign-investment-review regimes in Japan,
     Korea, and Germany — as they apply to AI-sensitive
     transactions
     <!-- needs-research: refresh AI-sensitive foreign-
     investment-review regimes and any AI-specific merger-
     notification thresholds at time of use -->

2. **Books and long-form references**
   - Robert Bruner — *Applied Mergers and Acquisitions*
     (foundational M&A text; background on deal structure,
     valuation, and process)
   - David Harding and Sam Rovit — *Mastering the Merger*
     (practitioner reference on integration and value capture)
   - Anu Bradford — *Digital Empires: The Global Battle to
     Regulate Technology* (reinforced from MOD-407; the
     regulatory frame in which AI M&A now operates)
   - Chris Miller — *Chip War: The Fight for the World's Most
     Critical Technology* (reinforced from MOD-406 and
     MOD-407; the supply-chain-as-asset frame as it enters the
     M&A diligence surface)
   - Barbara Minto — *The Pyramid Principle* (reinforced from
     MOD-402 and MOD-407) for transaction-committee and
     board-briefing memo structure

3. **Policy, industry, and technical reports**
   - Published strategic-AI-alliance announcements and 8-K
     filings (Microsoft-OpenAI structure and the commentary on
     its character; Amazon-Anthropic; Google-Anthropic;
     Oracle-OpenAI; NVIDIA investments in frontier labs;
     sovereign-vendor alliances) read as proto-M&A reference
     patterns
     <!-- needs-research: refresh the current list of major
     publicly disclosed AI alliances and their regulator
     characterizations at time of use -->
   - Published competition-authority reports on AI-industry
     partnerships and investments (FTC 6(b), DOJ, UK CMA,
     European Commission, BKartA)
     <!-- needs-research: assemble a current short list at time
     of use -->
   - Primary-source FTC algorithmic-disgorgement orders
     (Everalbum, Rite Aid, WW/Kurbo and successors) and their
     consent-decree obligations as the pattern the acquirer may
     inherit
     <!-- needs-research: refresh the FTC algorithmic-
     disgorgement catalog at time of use -->
   - Primary-source AI training-data litigation filings and
     dispositive rulings (NYT v. OpenAI, Getty v. Stability,
     Andersen v. Stability, GitHub Copilot class actions,
     music-label suits)
     <!-- needs-research: refresh pending and decided AI
     training-data litigation at time of use -->
   - Primary-source AI-vendor trust centers, sub-processor
     lists, model cards, system cards, and usage policies for
     counterparties in the organization's prospective target
     set

### Supplementary Resources

- American Bar Association — *Model Stock Purchase Agreement
  with Commentary* and the *Model Asset Purchase Agreement*
  with Commentary
  <!-- needs-research: confirm current edition and any
  AI-specific supplements at time of use -->
- Published R&W insurance market reports on AI-asset coverage,
  standard exclusions, and premium trends
  <!-- needs-research: refresh current R&W insurance market
  posture on AI-asset coverage at time of use -->
- Published AI-M&A deal tear-downs from major law firms —
  the "what moved in the merger agreement" summaries typically
  published quarterly
  <!-- needs-research: assemble a current short list of AI-M&A
  deal tear-downs at time of use -->
- Model-weight license primary sources — Llama Community
  License, Qwen License, Mistral AI License, DeepSeek License,
  Apache-2.0 model-weight releases, BSL variants, OpenRAIL
  descendants
  <!-- needs-research: refresh model-weight license landscape
  and the OSI OSAID state at time of use -->
- IAPP, Shared Assessments (SIG), and Cloud Security Alliance
  (CAIQ, CAIQ-AI) vendor-risk questionnaires as a floor for
  structured diligence
  <!-- needs-research: confirm current questionnaire versions
  at time of use -->
- Published 10-K risk factors on AI vendor and acquisition
  concentration, counterparty exposure, and integration risk
  from AI-heavy public companies
  <!-- needs-research: assemble a current short list -->
- AI Incident Database and Partnership on AI AI Incident Hub
  — transaction-adjacent incident patterns and diligence-
  surfaced risk precedents

See also `resources.md` in this module for the running reading list.

---

## Next Steps

Upon completing MOD-408, you will be prepared to:

1. **Produce and defend** an AI-technical-diligence report that
   a CFO, CRO, Chief Trust Officer, General Counsel, CISO, and
   board transaction committee can each sign
2. **Classify** any AI-era target on the deal-shape spectrum
   and lead the diligence emphasis the shape requires
3. **Translate** diligence findings into deal-term consequences
   — reps, specific indemnity, R&W insurance, escrow, earn-out,
   closing conditions, walk-away rights
4. **Diligence** AI-specific IP, data provenance, and derivative-
   model posture to a standard that survives a post-close
   dispute
5. **Diligence** AI-specific regulatory inheritance — EU AI Act
   role carry-over, GDPR joint-controller exposure, sectoral
   obligations, and US state AI law exposure — before the
   acquirer assumes it
6. **Design** a 100-day post-close integration plan, or a 12-
   to-24-month separation plan for a carve-out or divestiture,
   that accounts for infrastructure, model inventory, data
   boundaries, talent retention, trust and safety, and public
   communications
7. **Lead** the organization through a deal — pre-signing,
   signing-to-closing, post-closing, and 12- and 24-month
   deal-review retrospective — with the transaction-committee,
   board, regulator, customer, and workforce communications
   under time pressure
8. **Progress to MOD-409**: Thought Leadership and External
   Influence, where the discipline of defensible diligence
   and deal narrative extends into public writing, conference
   engagement, and industry-standard shaping

---

**Ready to begin?** Start with Week 1: The AI-M&A Landscape
and Deal-Shape Framework.

## Cross-references
- Engineering-level prerequisite: see ai-infra-engineer-learning + ai-infra-senior-engineer-learning
- Solutions repo: ai-infra-senior-architect-solutions/modules/mod-408-ma-due-diligence
