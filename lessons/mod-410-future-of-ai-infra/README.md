# MOD-410: The Future of AI Infrastructure

**Level**: Senior Architect (Strategic / Executive)
**Duration**: 35-50 hours
**Prerequisites**: Architect-level experience; mod-401 (Enterprise AI Strategy); mod-404 (Innovation and R&D), mod-405 (Responsible AI), mod-406 (Global Infrastructure), mod-407 (Strategic Partnerships), mod-408 (M&A Due Diligence), and mod-409 (Thought Leadership) recommended as the full prior arc

## Module Overview

This module is the capstone of the Senior AI Infrastructure
Architect curriculum (level 400). Focus: the future of AI
infrastructure — the discipline of reading, forecasting, and
positioning the organization against the compute, model, physical,
geopolitical, regulatory, and workforce trajectories that will
define AI infrastructure over the next three to ten years.

Senior-architect modules emphasize executive communication,
strategic thinking, and organizational influence — not hands-on
implementation. For hands-on technical material on related topics
(accelerator programming, inference serving, datacenter commissioning,
model-architecture research, evaluation harnesses), see the
engineer-level and senior-engineer-level repos.

### Executive Summary

Through MOD-401 to MOD-409, the senior architect learned to set
strategy, lead the executive conversation, operate the governance
program, run the R&D portfolio, embed responsible-AI practice,
deploy infrastructure globally, structure partnerships, diligence
acquisitions, and build a defensible external voice. MOD-410 asks
the question that sits over all of them: *which of these disciplines
will still work in three years, which will be obsolete, and which
will matter more than the organization currently thinks?* An
enterprise AI strategy that is internally coherent, externally
expressed, and operationally mature in 2026 is still only a current-
state artifact; the senior architect's distinctive contribution at
the top of the ladder is the ability to carry the organization
forward against uncertainties that are too large, too technical,
and too entangled with policy and geopolitics to be delegated.

At enterprise scale in 2026, "the future of AI infrastructure" is
not a speculative topic — it is a set of specific, named, and
partly dated trajectories that the organization either reads with
discipline or is overrun by. The compute roadmap (NVIDIA Hopper /
Blackwell / Rubin succession, AMD MI300 / MI325 / MI350 succession,
custom accelerators at AWS, Google, Microsoft, Meta, and sovereign
programs, the HBM3E / HBM4 memory ramp, 3nm-to-2nm-to-18A node
succession, advanced packaging, optical interconnect, co-packaged
optics) is public, cited in earnings calls, and encoded in
hyperscaler capex plans; the senior architect either knows how to
read it against the organization's workload mix or defers the
reading to a vendor. The physical-constraint roadmap (US and
European grid interconnection queues, nuclear and gas-plant-at-
the-meter siting, water cycles for dense cooling, land-use politics)
is similarly public and similarly consequential; the regulatory
roadmap (EU AI Act implementing acts, the AISI network, US state
AI law accretion, export-control evolution) is public but partial;
the model-architecture roadmap (test-time compute, agentic systems,
long-horizon tasks, embodied AI, multimodality, reasoning, memory
and context extension) is partially public and partially inside
the frontier labs. Reading each roadmap with discipline, mapping
each to the organization's workload mix, and identifying the no-
regret moves across them is the senior architect's capstone job.

At this level, "future of AI infrastructure" is a program with
six parts that must co-exist: a **forecasting-and-scenario
discipline** (the standing method by which the organization reads
trajectories, challenges its own forecasts, and documents the
uncertainties that remain), a **technology-trajectory stack**
(the compute, memory, networking, storage, model-architecture, and
system-architecture roadmaps the organization tracks and the named
owners of each), a **physical-and-economic-infrastructure
trajectory stack** (power, grid, siting, water, land, supply chain,
capital formation, project finance, and the industrial-policy
landscape that shapes each), a **policy-and-geopolitical
trajectory stack** (regulation, export control, sovereign AI,
decoupling, workforce migration, international standards), a
**workforce-and-organizational trajectory stack** (the automation
of engineering, researcher mobility, AI-native operating models,
the human-capital envelope that collapses or expands with each
model generation), and a **strategic-posture regime** (the
option-value discipline, the no-regret-moves catalog, the walk-
away triggers, and the executive and board communication that
makes all of it decidable). A program with five of the six works
until the sixth is tested, and then it does not.

By the end of this module, you will be able to:

- Design and run a forecasting-and-scenario discipline that
  translates public-and-adjacent evidence about AI-infrastructure
  trajectories into a standing set of scenarios, no-regret moves,
  and option-value decisions the organization can act on
- Read the compute-and-silicon roadmap — accelerator families,
  memory and bandwidth ramps, networking and packaging, custom
  ASICs, inference-specialized silicon, emerging post-digital
  compute (optical, neuromorphic, quantum) — against the
  organization's workload mix and multi-year capacity plan
- Read the physical-infrastructure roadmap — grid interconnection,
  on-site generation, water, land, climate exposure, siting,
  industrial policy — and connect each to the organization's
  capital plan, risk appetite, and sustainability commitments
- Read the model-and-system-architecture roadmap — scaling laws,
  test-time compute, reasoning models, agentic systems, long-
  horizon tasks, multimodality, embodied AI, world models, memory
  and context extension — and translate each into platform
  implications the organization must prepare for
- Read the policy, geopolitical, and economic trajectory stack —
  export control and chip-wars dynamics, sovereign AI
  programs, decoupling and re-coupling patterns, EU AI Act
  implementation, AISI network evolution, utility-model
  economics, capital formation and project finance for AI
  infrastructure — against the organization's international
  footprint and strategic position
- Read the workforce and organizational trajectory stack — the
  automation of software and research engineering, researcher
  and operator mobility, AI-native operating models, the
  organizational-form implications of substantially augmented
  teams — and connect each to the organization's talent,
  recruiting, and operating-model posture
- Govern the forecasting program as a program — the standing
  scenarios, the quarterly refresh, the "we were wrong about X"
  discipline, the executive and board communication, and the
  integration with the rest of the senior-architect program
- Communicate futures-level posture to the executive team, the
  board, the risk committee, the audit committee, the workforce,
  and the external surface (reinforced from MOD-409) with the
  same vocabulary, the same numbers, and the same honest treatment
  of what is known, what is forecast, and what is unresolved

---

## Learning Objectives

### Forecasting and Scenario Discipline

1. **Why the senior architect owns forecasting as a discipline**
   - Hyperscaler capex commitments are multi-year, non-cancellable,
     and public; the organization that defers reading them to its
     procurement function is positioned by vendors rather than
     positioning itself
   - Model-capability trajectories are the single largest driver
     of platform roadmaps; a "we will support the model families
     our customers want" posture is a posture only when the
     organization has an active view of which families will
     exist, how they will be served, and what the serving profile
     will cost — reinforced from MOD-401 and MOD-404
   - The regulatory and geopolitical surface changes faster than
     product cycles do; a quarterly scenario review is not
     futures work, it is current-state work with a wider
     aperture — reinforced from MOD-406 and MOD-409
   - The board asks "where will this industry be in three years"
     at every substantive review; silence or generality from the
     senior architect is itself a signal

2. **The forecasting-method vocabulary**
   - *Trend extrapolation* — the disciplined reading of public
     roadmaps, earnings calls, capex plans, and published scaling
     curves, with the "where this line goes under stated
     assumptions" discipline
   - *Scenario planning* — the Shell-pioneered discipline of
     naming a small set of coherent, internally consistent
     futures (not probabilities) and walking the organization
     through each, with named triggers for which one is becoming
     dominant
   - *Pre-mortem* — the Gary Klein discipline (reinforced from
     MOD-402, MOD-404, MOD-406, MOD-407, MOD-408, MOD-409)
     applied specifically to the organization's forward
     infrastructure plan ("it is three years from now; the
     plan has failed badly; why?")
   - *Delphi and structured expert judgment* — the discipline of
     eliciting, aggregating, and updating forecasts from the
     organization's own technical staff and from the external
     research community, with named-expert-source discipline
   - *Red-team and devil's-advocate* review of the organization's
     own forecasts — the standing requirement that the organization
     surface the strongest argument against its own forward view
   - *Forecast-of-record* discipline — the written, dated,
     signed forward view the organization actually commits to,
     distinct from the internal scenario set; the mechanism for
     updating it and the standing position on when the update
     requires executive or board communication

3. **The uncertainty-vocabulary discipline**
   - *Resolved uncertainty* — questions whose answer the
     organization now knows and has incorporated (e.g., HBM is a
     constrained input through the planning horizon)
   - *Dated uncertainty* — questions whose answer the
     organization will know at a specific future moment (e.g.,
     a named implementing act, a scheduled chip roadmap
     disclosure, a planned AI Safety Summit)
   - *Undated but bounded uncertainty* — questions whose answer
     is unknown but whose range is bounded (e.g., "a frontier
     model family at capability level X will or will not be
     available on open weights within the planning horizon")
   - *Deep uncertainty* — questions whose answer, range, and
     relevant mechanisms are all unresolved; the organization
     plans against the full scenario space rather than a point
     forecast, and the senior architect flags each one explicitly
     rather than letting it hide inside a confident forecast
   - *No-regret moves* — actions whose value is positive across
     every plausible scenario; the single most important
     product of the forecasting discipline
   - *Reversible-vs-irreversible* classification of forward
     commitments — long-dated power contracts, dense-cooling
     datacenter buildouts, and sovereign partnership commitments
     are irreversible on the planning horizon; software-stack and
     model-family commitments often are not

4. **The historical-track-record discipline**
   - The published "forecasts that were correct" and "forecasts
     that were wrong" register for the organization's own prior
     cycles — the discipline of actually keeping a journal that
     the organization and the board can inspect
   - Philip Tetlock's *Superforecasting* evidence base on what
     makes forecasters good — the "foxes beat hedgehogs" finding,
     the active-updating discipline, the "many small updates"
     posture, and the way that generalizes to institutional
     forecasting
   - The AI-specific track record of prior forecasts — the
     "AI will plateau at GPT-2 scale" and "AI will not do
     mathematics" and "AI will not do long-horizon coding"
     predictions, and what the organization learns from each
     having been wrong
   - The standing humility discipline — the organization
     publishes (internally and sometimes externally) its own
     forecasting track record, and treats the discipline as a
     measurable competence rather than an opinion-based one
     (reinforced from MOD-402 on the leadership posture and
     MOD-409 on the external-voice discipline)

### Compute, Memory, Networking, and the Silicon Roadmap

5. **The GPU and accelerator roadmap**
   - *NVIDIA* — the Hopper (H100/H200) → Blackwell (B100/B200/B300,
     GB200 NVL72) → Rubin succession, with the explicit per-
     generation jumps in FP8 / FP4 throughput, HBM capacity and
     bandwidth, NVLink generation, and NVSwitch topology; the
     DGX / HGX / MGX / NVL reference-design evolution
   - *AMD* — the MI300A / MI300X → MI325 → MI350 → MI400 succession;
     the ROCm software-stack trajectory and the frontier-customer
     adoption pattern
   - *Hyperscaler custom silicon* — Google TPU (v5e, v5p, Trillium,
     Ironwood and successors), AWS Trainium (Trainium2 and
     successors) and Inferentia, Microsoft Maia and Cobalt, Meta
     MTIA, Alibaba Hanguang and T-Head Yitian / Cross-Zen, Huawei
     Ascend 910B / 910C / successors; the trajectory of each
     against its parent's own workload mix
   - *Startup and merchant silicon* — Cerebras, Graphcore,
     SambaNova, Groq, Tenstorrent, Rebellions, Rain, Lightmatter,
     Celestial AI, Etched (Sohu), d-Matrix, Positron, FuriosaAI;
     the training-vs-inference specialization pattern and the
     merchant-market viability thesis for each
   - *Sovereign and regional silicon programs* — SMIC-fabricated
     accelerators, European Chips Act outputs (SiPearl, European
     Processor Initiative), Indian Semicon Mission outputs,
     Japanese Rapidus, Korean Samsung Foundry and Rebellions,
     Middle-Eastern programs; the industrial-policy context for
     each and the implications for sovereign-AI deployment
     (reinforced from MOD-406 and MOD-407)

6. **Memory, interconnect, and packaging**
   - *HBM* — the HBM3E / HBM4 / HBM4e succession, with explicit
     capacity-and-bandwidth per-stack trajectory, vendor roster
     (SK hynix, Samsung, Micron), and the merchant-vs-captive
     allocation pattern; the way HBM supply has become the
     binding constraint on frontier-model serving capacity
   - *Advanced packaging* — CoWoS (TSMC), SoIC, I-Cube / X-Cube
     (Samsung), Foveros / EMIB (Intel), the capacity roadmap
     and allocation pressure; the way packaging capacity has
     become the second binding constraint after HBM
   - *Node succession* — TSMC N3 / N3P / N3X → N2 → A16 → A14,
     Samsung SF2, Intel 18A / 14A, with the per-node density,
     performance, and yield trajectory; the customer-allocation
     pattern (leading-edge-first for frontier accelerators) and
     the geopolitical-friction surface
   - *Networking* — NVLink / NVSwitch generation, Infinity Fabric,
     UALink and Ultra Ethernet Consortium, InfiniBand NDR / XDR,
     800G / 1.6T Ethernet, co-packaged optics and silicon photonics,
     linear-pluggable optics; the rack-to-cluster-to-datacenter
     fabric trajectory
   - *Storage* — NVMe-oF, CXL-attached memory and storage, the
     NVMe / QLC flash trajectory, object-storage-for-training,
     and the memory-storage disaggregation posture; the way
     storage architecture has become a frontier-workload
     constraint rather than a solved problem
   - *CXL and composable infrastructure* — CXL 3.x / 4.x
     trajectory, the memory-pool and accelerator-attach
     implications, and the realistic timeline against the HBM
     and advanced-packaging constraints

7. **Inference-specialized silicon and the training-vs-inference bifurcation**
   - The *inference-only* silicon thesis — Groq LPU, Cerebras
     WSE-based inference, Etched Sohu, d-Matrix, FuriosaAI
     RNGD, Positron; the "generative decode throughput per
     watt" and "generative decode throughput per dollar"
     frontiers against general-purpose GPU/TPU inference
   - The *reasoning-and-test-time-compute* inference profile —
     the way O-style reasoning models shift the economics of
     inference silicon (long decodes, high memory bandwidth
     pressure, batch-size sensitivity) and the implications for
     the inference-silicon bet
   - The *edge and on-device* inference trajectory — Apple
     Neural Engine, Qualcomm Hexagon, MediaTek APU, Intel
     Lunar Lake / Panther Lake NPU, AMD Ryzen AI, and the
     consumer-AI-at-the-edge question; the implications for
     the organization's model-distribution and privacy posture
   - The *training-vs-inference bifurcation* — the specific
     organizational posture question of whether the organization
     uses the same silicon for both (NVIDIA-exclusive), different
     silicon within one vendor family, or mixed-vendor training
     and inference; the operational and economic implications
     of each

8. **Post-digital and emerging compute**
   - *Optical / photonic compute* — Lightmatter, Celestial AI,
     Ayar Labs photonics, Lightelligence; the "where optical
     wins" workload register (matrix multiply, interconnect,
     memory access) and the realistic deployment horizon
   - *Analog and in-memory compute* — Mythic, EnCharge AI,
     IBM research directions; the inference-specific
     applicability and the known precision-noise trade-offs
   - *Neuromorphic* — Intel Loihi, IBM TrueNorth and NorthPole,
     SpiNNaker and BrainScaleS research directions; the current
     "real workload where neuromorphic wins" register
   - *Quantum* — IBM, Google Quantum AI, IonQ, Quantinuum,
     Rigetti, PsiQuantum, QuEra, Pasqal, Atom Computing, D-Wave;
     the fault-tolerance and error-correction roadmap, the
     NISQ-vs-FTQC distinction, and the realistic "where quantum
     intersects AI infrastructure" register (likely very
     limited through the planning horizon); the specific
     discipline of not letting quantum-marketing noise displace
     actual-workload reasoning
   - *Biological, molecular, and exotic compute* — the "worth
     a watchlist, not a budget line" category, kept visible
     for completeness

### Physical Infrastructure, Energy, and Siting

9. **The power and grid trajectory**
   - *Datacenter load forecasts* — the EIA and IEA published
     load forecasts, the ERCOT / PJM / MISO / SPP / CAISO / NYISO
     interconnection-queue status, the equivalent European TSO
     queues (TenneT, 50Hertz, RTE, National Grid ESO), and the
     Asian-utility queues (TEPCO, KEPCO, TNB, EGAT, CLP)
   - *Interconnection queue dynamics* — the multi-year wait
     time in several US ISOs, the "fast-track" and "shovel-
     ready" programs, the queue-reform FERC orders (Order 2023
     and subsequent), and the implications for datacenter
     siting timelines
   - *Behind-the-meter and on-site generation* — the natural-
     gas-turbine-at-the-meter trend, the solar-plus-storage
     posture, the fuel-cell option, and the distinct economic
     and regulatory profile of each
   - *Nuclear-for-AI* — the small modular reactor (SMR)
     deployment timeline (NuScale, X-energy, TerraPower,
     Oklo, Kairos, GE Hitachi BWRX-300, Westinghouse AP300),
     the nuclear-restart and nuclear-expansion programs, the
     hyperscaler PPA posture (Microsoft-Constellation, AWS-
     Talen, Google-Kairos and others), the realistic
     deployment horizon against stated capacity needs
   - *Grid curtailment and demand response* — the use of
     interruptible load, demand response, and curtailment
     agreements as capacity-access instruments; the implications
     for inference-vs-training workload placement
   - *Transmission buildout* — the inter-regional transmission
     queue, the HVDC project pipeline, and the implications for
     when stranded generation can serve AI load

10. **Water, land, and climate exposure**
    - *Water* — the dense-cooling water-use profile against
      regional water availability, the Southwest-US and
      Mediterranean-European water-stress intersection with
      AI-datacenter growth, the direct-liquid-cooling and
      immersion-cooling trajectory, the recycled-water and
      closed-loop options
    - *Land* — the hyperscaler-campus land-acquisition
      pattern, the industrial-park vs. greenfield posture, the
      community-and-zoning friction surface, and the specific
      state-and-local-politics discipline required for a
      multi-gigawatt siting
    - *Climate exposure* — the physical-climate-risk discipline
      (flood, wildfire, heat-stress, hurricane, grid-outage-
      from-extreme-weather) applied to the datacenter footprint,
      with the TCFD / IFRS S2 / CSRD disclosure vocabulary
      (reinforced from MOD-406)
    - *Reporting and sustainability commitments* — the
      scope 1/2/3 carbon posture, the water-use disclosure,
      the "AI emissions" discipline that has emerged as a
      distinct sustainability category; the implications for
      the organization's own stated commitments and the
      hyperscaler counterparty commitments

11. **Cooling, power delivery, and datacenter architecture**
    - *Rack density* — the 50 kW → 100 kW → 250 kW → 500 kW+
      rack trajectory, with the implications for cooling
      architecture, power-delivery architecture, and retrofit
      vs. greenfield posture
    - *Direct-liquid cooling and immersion* — the single-phase
      vs. two-phase posture, the coolant-chemistry question
      (PFAS regulatory exposure, fluid-vendor lock-in), the
      operational-complexity delta against air-cooled
      baselines
    - *Power delivery* — the 48 V DC / 400 V DC trends, the
      medium-voltage rack busbar question, the solid-state
      transformer and advanced power-electronics trajectory
    - *Modular and prefabricated construction* — the
      prefabricated power-and-cooling pod, the modular
      datacenter deployment model, the implications for build-
      to-suit vs. speculative buildout
    - *The datacenter-as-industrial-plant transition* — the
      recognition that an AI-training datacenter has the
      physical, operational, and regulatory profile of a
      small industrial site rather than a traditional
      commercial computing facility; the implications for
      organizational capability (in-house vs. outsourced
      operations) and for the executive-risk conversation
      (reinforced from MOD-406)

### Model and System Architecture Trajectories

12. **The scaling-and-capability trajectory**
    - *Pre-training scaling* — the public scaling curves
      (Chinchilla, compute-optimal, and subsequent updates),
      the data-wall question (high-quality human text as a
      finite resource), the synthetic-data trajectory, and
      the realistic "next 2-3 pre-training generations"
      capacity profile
    - *Test-time compute scaling* — the O-style reasoning-model
      trajectory (OpenAI o-series, DeepSeek-R1 / V3, Anthropic
      extended-thinking, Google Gemini deep-think, Qwen QwQ,
      and successors), the "spend compute at inference time
      instead of training time" thesis, and the serving-economics
      implications
    - *Mixture-of-experts and sparse-activation* — the trajectory
      from dense through MoE through finer-grained routing, the
      memory-footprint-vs-activation-footprint trade-off, and
      the serving implications
    - *State-space, hybrid, and attention-alternative*
      architectures — Mamba, RWKV, Griffin, Jamba, hybrid
      transformer-SSM architectures; the realistic deployment
      profile against transformer baselines
    - *Multimodal and omnimodal* architectures — the trajectory
      from text-only through text+image through text+image+
      audio+video through full omnimodal; the serving, training,
      and evaluation implications

13. **Agentic systems and long-horizon tasks**
    - *Tool use and function calling* — the trajectory from
      single-call tool use through structured multi-call
      pipelines through long-horizon agentic trajectories;
      the serving-infrastructure implications (sticky
      sessions, memory, retry, rate-limit management)
    - *Computer-use and browser-use agents* — the Operator,
      Computer Use, Project Mariner-style agent pattern, the
      "the agent drives a general-purpose operating environment"
      model, and the implications for sandboxing, observability,
      and incident-response posture (reinforced from MOD-405)
    - *Multi-agent and agent-swarm* patterns — the practical
      realistic deployment pattern against the "autonomous
      swarm" marketing claim, the specific coordination-and-
      conflict-resolution surface, and the operational-
      discipline requirement
    - *Agent evaluation and reliability* — the shift in
      evaluation from single-turn correctness to multi-turn
      robustness, the "agentic benchmark" landscape (SWE-bench,
      SWE-Lancer, OSWorld, WebArena, GAIA, and successors),
      and the gap between benchmark success and production
      reliability
    - *Long-horizon-task economics* — the "how many dollars
      and minutes does the agent take to complete a half-day
      knowledge-worker task, and how reliably" question, as
      the single operational question that determines whether
      agentic deployment moves from pilot to production

14. **Memory, context, and long-horizon state**
    - *Context-window extension* — the 1M-token and multi-
      million-token context trajectory, the KV-cache
      architecture implications, the "effective context" vs.
      "advertised context" distinction, and the retrieval-
      vs-long-context posture question
    - *Agent memory* — the trajectory from stateless agents
      through session-scoped memory through long-term
      persistent memory, with the privacy, provenance, and
      consent implications (reinforced from MOD-405)
    - *Retrieval-augmented generation* — the maturation of
      RAG from an early-generation pattern to a baseline
      pattern, the hybrid retrieval-plus-long-context
      pattern, the GraphRAG and knowledge-graph variants, and
      the ongoing architectural debate
    - *Continual learning and online adaptation* — the
      practical deployment profile against the research
      literature, the "model weights update in production"
      question, and the governance posture (reinforced from
      MOD-405)

15. **World models, embodied AI, and the robotics and scientific-discovery adjacencies**
    - *World models* — the Genie / DreamerV3 / Sora / Veo-style
      world-model trajectory, the "video and simulation as
      training signal" thesis, and the implications for
      compute, storage, and dataset infrastructure
    - *Robotics and embodied AI* — the vision-language-action
      (VLA) model trajectory (RT-2, OpenVLA, Pi-0,
      Helix, and successors), the humanoid-robot commercial
      trajectory, the industrial-robotics AI integration
      pattern, and the implications for the organization's
      "are we in robotics or not" decision
    - *Scientific-discovery AI* — AlphaFold / AlphaProteo /
      AlphaMissense / AlphaGenome / AlphaEvolve, the
      materials-and-chemistry AI trajectory, the bioinformatics
      AI stack, and the implications for the organization's
      sector exposure
    - *Mathematical reasoning and formal verification* —
      the AlphaProof, AlphaGeometry, Lean-and-Rocq-integrated
      systems trajectory, and the implications for software-
      engineering and research-infrastructure workloads

### Geopolitics, Industrial Policy, and the Economic Structure of AI

16. **Export control and the chip-wars dynamics**
    - *US export-control trajectory* — the October-2022 /
      October-2023 / March-2024 / January-2025 and subsequent
      BIS rule progression, the "AI Diffusion" framework and
      its country tiers, the commerce-licensing posture, and
      the extraterritorial Foreign Direct Product Rule
      application
      <!-- needs-research: refresh the BIS export-control
      rule set, the country tiering, and the enforcement
      posture at time of use -->
    - *China response* — SMIC and YMTC capacity, Huawei Ascend
      and Kunpeng, Biren and Moore Threads, the "DUV at
      advanced nodes" path, the domestic HBM and packaging
      programs, and the realistic frontier-silicon profile
      inside the controlled perimeter
      <!-- needs-research: refresh the Chinese domestic
      semiconductor-and-accelerator program status at time
      of use -->
    - *Allied coordination* — Japan METI chip-equipment
      controls, Netherlands ASML licensing, Korea semiconductor-
      export posture, EU Dual-Use Regulation, UK export-
      control regime; the multilateral coordination mechanism
      and its gaps
      <!-- needs-research: refresh allied export-control
      coordination at time of use -->
    - *Entity listings and sanctions* — the OFAC and BIS
      Entity-List surface, the counterparty-screening discipline
      the organization must run (reinforced from MOD-406 and
      MOD-407), and the specific exposure of hyperscaler and
      model-vendor commercial engagements with listed entities

17. **Sovereign AI programs and industrial policy**
    - *US industrial policy* — the CHIPS and Science Act
      allocation, the AI R&D funding programs (DARPA, NSF, DOE,
      NIH), the national-labs-as-AI-infrastructure trajectory
      (Aurora, Frontier, El Capitan, Venado and successors),
      the AI-infrastructure-of-national-significance framing
      <!-- needs-research: refresh US industrial-policy AI
      programs at time of use -->
    - *EU industrial policy* — the European Chips Act
      implementation, the AI Factories and Gigafactories
      program, the Important Projects of Common European
      Interest (IPCEI) AI projects, the EuroHPC JU AI
      Supercomputers, the ongoing-and-evolving European
      Sovereign AI Fund
      <!-- needs-research: refresh EU AI industrial policy
      at time of use -->
    - *Asian industrial policy* — Japan Rapidus and METI AI
      compute program, Korea K-Chip Act and AI compute fund,
      Singapore IMDA National AI Strategy 2.0, Taiwan's
      TSMC-centric industrial base, India's Semicon Mission
      and IndiaAI Mission, Malaysia's semiconductor-and-DC
      corridor
      <!-- needs-research: refresh Asian AI industrial
      policy at time of use -->
    - *Middle Eastern and other sovereign programs* — UAE
      (G42, MGX, Core42, Khazna), Saudi Arabia (HUMAIN, PIF
      compute program), Qatar, Kuwait; the sovereign-AI-fund
      posture that has become a substantial AI-infrastructure
      capital source
      <!-- needs-research: refresh Middle Eastern sovereign-
      AI programs at time of use -->
    - *Decoupling, re-coupling, and friendshoring* — the
      realistic trajectory of supply-chain decoupling against
      the counter-pressure of comparative advantage, with
      the implications for the organization's multi-regional
      posture (reinforced from MOD-406)

18. **Capital formation and the economic structure of AI infrastructure**
    - *Hyperscaler capex trajectory* — the published and
      analyst-projected capex arc for the major hyperscalers
      (Microsoft, Google, Amazon, Meta, Oracle, Alibaba,
      Tencent, Baidu, ByteDance), the depreciation-schedule
      and useful-life question, and the implications for
      the vendor-pricing trajectory
      <!-- needs-research: refresh the hyperscaler capex
      landscape and the useful-life accounting posture at
      time of use -->
    - *AI-infrastructure project finance* — the emerging
      independent AI-datacenter developer category (CoreWeave,
      Lambda, Crusoe, Nebius, Applied Digital, Vultr, Voltage
      Park, Oracle Cloud Infrastructure for AI), the project-
      finance and private-credit structures, the "GPU-as-
      collateral" question, and the implications for the
      organization's buy-or-lease posture
      <!-- needs-research: refresh the AI-datacenter-
      developer landscape and the project-finance posture
      at time of use -->
    - *Utility-model economics* — the thesis that AI inference
      compute moves toward a utility-pricing model (per-token,
      per-request, with regulated or quasi-regulated access),
      and the realistic trajectory against the ongoing
      merchant-pricing model
    - *Model-pricing trajectory* — the published per-million-
      token price curves, the "cost per intelligence unit"
      vocabulary, the realistic expectation for the planning
      horizon, and the implications for the organization's
      budget and pricing posture
      <!-- needs-research: refresh the model-pricing curves
      and the per-million-token economic-profile landscape
      at time of use -->
    - *Private-market valuation and M&A trajectory* — the
      ongoing AI-company private-market dynamics, the
      strategic-vs-financial acquirer posture, and the
      implications for the organization's partnership and
      M&A program (reinforced from MOD-407 and MOD-408)

19. **Regulatory futures and the compliance envelope**
    - *EU AI Act implementation trajectory* — the implementing-
      act and delegated-act schedule, the European AI Office
      enforcement posture, the general-purpose-AI-model (GPAI)
      Code of Practice evolution, the national competent-
      authority designation, the standards harmonization
      (CEN-CENELEC JTC 21) trajectory
      <!-- needs-research: refresh EU AI Act implementation
      and the European AI Office enforcement posture at time
      of use -->
    - *US federal AI regulation trajectory* — the AISI and
      NIST evolution, the FTC AI enforcement posture, the
      sectoral-regulator AI guidance (SEC, FDA, CFPB, OCC,
      HHS OCR, DOT), the "sectoral + state" US model vs. the
      counterfactual federal legislation
      <!-- needs-research: refresh US federal AI regulation
      trajectory at time of use -->
    - *US state AI law accretion* — the Colorado AI Act, New
      York ADMT, California AB 2013 / SB 942 / SB 1047-style
      proposals, Texas TRAIGA, and the ongoing proliferation;
      the "patchwork compliance" posture and the realistic
      expectation for federal preemption
      <!-- needs-research: refresh US state AI law effective
      dates and the preemption posture at time of use -->
    - *UK, Japan, Korea, Singapore, India, Canada, Australia
      regulatory trajectory* — the UK AISI and "principles-
      based plus sectoral" posture, Japan's AI Bill and
      guidelines, Korea's AI Act, Singapore's IMDA AI
      governance, India's DPDP Act and IndiaAI, Canada's
      AIDA posture, Australia's AI safety-and-guardrails
      process
      <!-- needs-research: refresh the non-EU, non-US AI
      regulatory landscape at time of use -->
    - *The AISI network and frontier-model-evaluation
      regime* — the AISI (US), AISI UK, EU AI Office, and
      counterpart evaluation-and-disclosure obligations;
      the voluntary-to-mandatory transition trajectory
      (reinforced from MOD-405 and MOD-409)
    - *Content provenance and authenticity* — C2PA
      implementation, watermarking mandates (California AB
      3211 and successors, EU AI Act Article 50), the realistic
      trajectory of synthetic-content disclosure
      <!-- needs-research: refresh content-provenance
      regulation and C2PA deployment status at time of use -->
    - *Liability and litigation trajectory* — the training-data
      litigation (NYT v. OpenAI and successors), the output-
      liability docket, the competition-authority AI docket,
      and the realistic exposure envelope for the planning
      horizon (reinforced from MOD-407 and MOD-408)
      <!-- needs-research: refresh the AI-industry litigation
      docket at time of use -->

### Workforce, Organization, and the Human-Capital Future

20. **The automation of engineering and research work**
    - *Software engineering automation* — the trajectory of
      coding agents (Claude Code, Cursor, Windsurf, Cline,
      Aider, Devin, Codex-style agents), the SWE-bench and
      SWE-Lancer progress, the realistic "what fraction of
      a senior-engineer workday is automatable in year 1 /
      year 2 / year 3" register
      <!-- needs-research: refresh the coding-agent landscape,
      SWE-benchmark progress, and real-production-adoption
      evidence at time of use -->
    - *Research-engineering automation* — the trajectory of
      AI-driven research-engineering tooling (experiment
      design, ablation management, result interpretation,
      literature synthesis), the "AI research assistant"
      and "AI scientist" research programs, and the
      realistic deployment profile
    - *Infrastructure-engineering automation* — the trajectory
      of AI-driven SRE, incident-response, capacity-planning,
      and config-generation tooling; the SOX and auditability
      implications of agentic infrastructure change (reinforced
      from MOD-403)
    - *The "AI-augmented workforce" discipline* — the
      organization's explicit position on how its own engineering
      and research staff use AI tooling, the measurement regime,
      and the implications for team structure, compensation,
      and headcount trajectory
    - *The disclosure and trust question* — the specific
      question of what the organization discloses to customers,
      regulators, workforce, and investors about the AI
      augmentation of its own output (reinforced from MOD-405
      and MOD-409)

21. **Researcher, operator, and executive mobility**
    - *Researcher mobility* — the ongoing frontier-lab talent
      cycle, the acqui-hire mechanism (reinforced from MOD-408),
      the non-compete and retention-economics discipline, the
      "a specific team of twelve is the asset" thesis
      <!-- needs-research: refresh the frontier-researcher
      mobility landscape and the public cycle of lab transitions
      at time of use -->
    - *Operator mobility* — the AI-infrastructure operator and
      SRE labor market, the specific scarcity of people who
      have deployed frontier-scale training, the realistic
      cost-of-capability profile
    - *Executive mobility* — the AI-industry CEO, CTO, CSO,
      and senior-architect market, the board-level sourcing
      pattern, and the implications for the organization's
      talent and succession planning (reinforced from MOD-402)
    - *Sovereign and policy-adjacent mobility* — the growing
      AISI, NIST, EU AI Office, UK AISI, and equivalent
      public-sector AI-infrastructure roster; the "govtech
      exit" as a new standing-career-path within the AI
      workforce

22. **AI-native operating models and organizational form**
    - *The "AI-native organization" thesis* — the possibility
      that a greenfield organization built around AI
      augmentation achieves meaningfully smaller headcount and
      higher throughput than a classical peer; the realistic
      evidence base vs. the marketing claim
    - *Team-structure implications* — the "small senior team
      with heavy AI augmentation" pattern, the "AI operator"
      and "AI product-manager" and "AI engineer" role
      emergence, the specific operating-model experiments
      the organization will run
    - *The compensation-and-equity question* — the
      compensation structure when individual contribution is
      substantially AI-augmented, the equity structure when
      organizational output grows faster than headcount, and
      the implications for the organization's talent-strategy
      (reinforced from MOD-402)
    - *Governance implications* — the audit, control, and
      segregation-of-duties posture when agentic systems
      execute tasks that were previously human-executed; the
      specific SOX, SOC 2, ISO 27001, and regulated-industry
      control-environment implications (reinforced from
      MOD-403)
    - *The human-in-the-loop posture* — the organization's
      standing position on which categories of action the
      organization requires a human in the loop for, the
      review cadence, and the specific "trust boundaries"
      the organization is willing to cross and not cross
      (reinforced from MOD-405)

### Strategic Posture and the Capstone Synthesis

23. **Option value, no-regret moves, and the irreversibility discipline**
    - *Option-value* vocabulary — the recognition that
      investment in a capability now creates the option to
      use it later, and that the value of the option can
      dominate the expected value of the commitment under
      uncertainty; the specific application to compute,
      model-family, and partnership commitments
    - *No-regret moves* — the explicit catalog of actions the
      organization takes because they are positive across
      every plausible scenario (e.g., invest in evaluation
      harness capability, invest in data-provenance
      discipline, invest in sovereign-partnership optionality,
      invest in researcher-and-operator depth); the senior
      architect's standing catalog
    - *Irreversibility* classification — the explicit sorting
      of forward commitments by reversibility, with the
      "long-dated and irreversible" bucket receiving the
      most decision-weight; the specific implications for
      power contracts, datacenter buildouts, sovereign
      partnerships, and executive commitments
    - *Real-options* framing — the formal decision-under-
      uncertainty vocabulary applied to the AI-infrastructure
      portfolio, with the "stage gate", "milestone-based
      investment", and "walk-away trigger" discipline
    - *Portfolio* discipline — the recognition that forward
      bets cannot all pay off, the deliberate diversification
      across compute-vendor, model-family, deployment-region,
      and scenario commitments, and the explicit anti-
      "concentrate on the single highest-probability scenario"
      discipline

24. **Walk-away triggers and the strategic-discontinuity discipline**
    - *Walk-away triggers* — the explicit, dated, pre-committed
      conditions under which the organization abandons a
      major commitment (a vendor, a region, a model family,
      a product line); the senior architect's standing
      documentation of each
    - *Strategic-discontinuity* recognition — the explicit
      watch list of events that would force the organization
      into a different strategy (e.g., a sovereign AI
      program that the organization chooses to join or
      compete with; a frontier-capability threshold that
      makes a capability commercially irrelevant; a
      regulatory development that forces a geographic
      withdrawal); the specific governance mechanism for
      recognizing each as it occurs
    - *Pre-committed response* — the standing "if X happens,
      we do Y within Z days" register, so the organization
      moves on its forecasting rather than on its surprise
    - *"We were wrong"* discipline — the explicit mechanism
      for abandoning a forecast and re-planning, with the
      executive-and-board communication that honors the
      scale of the pivot without masking it
    - *Succession and continuity* — the discipline of ensuring
      that the forecasting and strategic-posture program
      survives the departure of individuals, including the
      senior architect; the institutional-memory discipline
      that protects against the "oral tradition" failure
      mode (reinforced from MOD-402)

25. **Integration with the rest of the senior-architect program**
    - *Strategy* (MOD-401) — the forward-view input into the
      annual strategy refresh, the alignment with the
      business-strategy horizon, the "a strategy without a
      scenario set is a wish" discipline
    - *Executive leadership* (MOD-402) — the way senior-
      architect forecasting becomes an executive-leadership
      capability, with the executive-and-board communication
      and the succession-planning discipline
    - *Governance* (MOD-403) — the integration of forecasting
      into the enterprise risk register, the audit-committee
      and risk-committee readout, the control-environment
      implications of agentic-system adoption
    - *R&D* (MOD-404) — the way the forecasting program
      drives the R&D portfolio allocation, the explicit
      alignment of research bets with the scenario set, the
      "which bets are the organization uniquely positioned
      to make" discipline
    - *Responsible AI* (MOD-405) — the way forecasting
      exposes the near-horizon responsible-AI risks the
      organization must prepare for (agentic-system
      incidents, autonomy escalation, high-stakes-decision
      deployments), with the proactive rather than reactive
      posture
    - *Global infrastructure* (MOD-406) — the way forecasting
      shapes the multi-regional footprint, the power and
      siting strategy, the sovereign-AI partnership posture
    - *Strategic partnerships* (MOD-407) — the way forecasting
      shapes the vendor, hyperscaler, and sovereign-partnership
      portfolio, with the walk-away and option-value
      discipline applied explicitly
    - *M&A* (MOD-408) — the way forecasting shapes the
      acquisition pipeline, the carve-out posture, and the
      minority-investment program
    - *Thought leadership* (MOD-409) — the way forecasting
      becomes the standing input into the external-voice
      program, with the "we said this three years ago and
      here is what happened" track-record discipline

26. **Executive, board, and workforce communication about the future**
    - *Executive-team readout* — the standing cadence
      (typically quarterly) at which the senior architect
      presents the forecasting program, the scenario set,
      the no-regret moves, and the walk-away triggers
    - *Board readout* — the annual board-level future-of-
      AI-infrastructure review, framed in the business-
      outcome vocabulary the board recognizes; the risk-
      committee and audit-committee adjuncts that address
      the forecasting-program risks (over-confidence, under-
      investment, concentrated bets, succession)
    - *Risk-committee readout* — the explicit treatment of
      the forecasting program's failure modes, the standing
      red-team posture, and the "where we are most
      confidently wrong" register
    - *Workforce communication* — the standing explanation
      to the workforce of what the organization believes
      about the trajectory, how it affects the workforce
      directly, and the specific commitments the organization
      makes on workforce transition (reinforced from MOD-402
      and MOD-405)
    - *External communication* — the forecasting program's
      output as an input into the thought-leadership stack
      (MOD-409), with the explicit discipline of what the
      organization will and will not say publicly about its
      own forward view

27. **The capstone posture — what the senior architect owns at the top of the ladder**
    - The *forecasting program* as a program, not an
      opinion — standing scenarios, named owners, review
      cadence, red-team discipline, track-record register,
      executive and board communication, integration with
      the rest of the senior-architect program
    - The *strategic-posture* register — the organization's
      explicit stated posture across every major technology,
      physical-infrastructure, policy, geopolitical, and
      workforce trajectory; the dated commitments and the
      walk-away triggers
    - The *no-regret moves catalog* — the standing list of
      investments the organization makes because they are
      positive across every plausible scenario, with the
      explicit "not pet projects, not uncertainty-reducing
      noise" discipline
    - The *"what the organization believes"* document — the
      senior architect's standing synthesis, updated on a
      defined cadence, cited from every strategic
      conversation; the artifact that outlasts any individual
      executive or board member
    - The *succession-and-continuity* discipline — the
      recognition that the forecasting program and the
      strategic-posture register are institutional assets
      that must survive personnel transitions, including
      the senior architect's own

---

## Module Structure

```
mod-410-future-of-ai-infra/
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

### Week 1: Forecasting and Scenario Discipline (6 hours)

**Topics:**
- Why "future of AI infra" is a strategic discipline the senior
  architect owns — the hyperscaler capex and model-capability
  trajectories as decision inputs, the regulatory and
  geopolitical surface as current-state-with-wider-aperture
  work, and the board-level demand for a stated forward view
- The forecasting-method vocabulary — trend extrapolation,
  scenario planning, pre-mortem, structured expert judgment,
  red-team review, forecast-of-record, and the way the
  methods complement rather than compete with each other
- The uncertainty vocabulary — resolved, dated, undated-but-
  bounded, deep; no-regret moves; reversible-vs-irreversible;
  the explicit discipline of flagging each type rather than
  letting them hide behind confident forecasts
- The historical-track-record discipline — the organization's
  own prior forecasts graded against outcomes, the
  *Superforecasting* evidence base, the AI-specific
  "forecasts that were wrong" register, and the standing
  humility posture

**Readings:**
- Pierre Wack — "Scenarios: Uncharted Waters Ahead" and
  "Scenarios: Shooting the Rapids" (*Harvard Business Review*,
  1985), as the foundational references on scenario planning
  from the Shell program that established the discipline
- Peter Schwartz — *The Art of the Long View* (the enduring
  practitioner reference on scenario planning)
- Philip Tetlock — *Superforecasting: The Art and Science of
  Prediction* (the empirical evidence base on what makes
  forecasters good; the "fox vs. hedgehog" distinction and
  the active-updating discipline)
- Gary Klein, HBR — "Performing a Project Premortem"
  (reinforced from MOD-402, MOD-404, MOD-406, MOD-407,
  MOD-408, MOD-409; applied here to the forecasting program's
  own failure modes)
- Nassim Taleb — *The Black Swan* and *Antifragile* (the
  vocabulary for the deep-uncertainty regime and the
  "robust-to-surprise" posture)
- Daniel Kahneman — *Thinking, Fast and Slow* (reinforced
  from MOD-402; the overconfidence, anchoring, and
  availability biases that forecasting programs must
  defend against)
- Published AI-forecast track records — the Metaculus AI
  benchmark forecasts, the Good Judgment Open AI questions,
  the Manifold AI-related markets, the Open Philanthropy
  AI timelines work; read for the specific discipline of
  how forecasts are stated, graded, and updated
  <!-- needs-research: refresh the state of AI-forecast
  track-record platforms at time of use -->
- Carl Sagan — *The Demon-Haunted World* (the enduring
  reference on the discipline of distinguishing claim,
  evidence, and warrant — applied here to AI-trajectory
  evidence)

**Exercise:** Produce a one-page internal note to the CTO
on the organization's current forecasting posture — the
standing scenarios (if any), the forecasting method actually
in use, the track-record register (if any), and the three
most material gaps between current state and the operating
model above. See `exercises/exercise-01-case-study.md` for
a structured version.

---

### Week 2: Compute, Memory, Networking, and the Silicon Roadmap (8 hours)

**Topics:**
- The GPU and accelerator roadmap — NVIDIA Hopper / Blackwell /
  Rubin, AMD MI300 / MI325 / MI350 / MI400, hyperscaler custom
  silicon, startup and merchant silicon, sovereign and
  regional silicon programs
- Memory, interconnect, and packaging — HBM3E / HBM4, advanced
  packaging (CoWoS, SoIC, I-Cube, Foveros, EMIB), node
  succession (TSMC N3/N2/A16, Samsung SF2, Intel 18A/14A),
  AI fabrics (NVLink, UALink, Ultra Ethernet, InfiniBand, 800G/
  1.6T Ethernet, silicon photonics, co-packaged optics), storage
  (NVMe, CXL, QLC flash, object-storage-for-training)
- Inference-specialized silicon and the training-vs-inference
  bifurcation — Groq, Cerebras, Etched, d-Matrix, FuriosaAI,
  Positron, SambaNova; on-device NPUs (Apple, Qualcomm, Intel,
  AMD, MediaTek); the organizational-posture question
- Post-digital and emerging compute — optical/photonic, analog
  and in-memory, neuromorphic, quantum, exotic; the
  "watchlist-vs-budget-line" discipline

**Readings:**
- NVIDIA, AMD, Intel, Google, AWS, Microsoft, Meta, Oracle,
  Alibaba most-recent earnings calls and investor-day
  presentations — read for the stated capex, accelerator
  roadmap, and workload mix
  <!-- needs-research: refresh the hyperscaler and silicon-
  vendor earnings-and-investor-day corpus at time of use -->
- TSMC, Samsung Foundry, Intel Foundry most-recent earnings
  calls and technology-symposium presentations — read for
  the node, packaging, and capacity trajectory
  <!-- needs-research: refresh the fab-earnings and
  technology-symposium corpus at time of use -->
- SemiAnalysis, The Information, Stratechery, Bloomberg
  Supply Lines, Nikkei Asia semiconductor coverage — read
  for the current trajectory against the stated roadmap
  <!-- needs-research: confirm the current reputable
  semiconductor-analyst corpus at time of use -->
- ISSCC, Hot Chips, Hot Interconnects, VLSI Symposium
  published proceedings — read for the technical substance
  behind the vendor marketing
  <!-- needs-research: refresh the technical-conference
  proceedings relevant to the planning cycle at time of use -->
- MLCommons MLPerf Training, Inference, HPC, and Storage
  result sets — read for the realistic workload performance
  against vendor claims (reinforced from MOD-404 and MOD-409)
  <!-- needs-research: refresh the MLPerf result-set
  landscape at time of use -->
- Clayton Christensen — *The Innovator's Dilemma* and *The
  Innovator's Solution* (reinforced from MOD-404 and MOD-409;
  applied here to the merchant-silicon-vs-custom-silicon
  trajectory)

**Case Study:** The organization's current accelerator
footprint is heavily NVIDIA-weighted (H100 and H200), with a
two-year commitment to Blackwell deployment and an unresolved
question on whether to commit to Rubin at the stated
hyperscaler price. A competitor-vendor custom accelerator
has just been shown at Hot Chips with a claimed 1.6x FP8
training throughput at 0.7x the stated power envelope, with
the specific caveat that the software stack is unproven at
frontier scale. A hyperscaler partner has independently
announced a fourth-generation internal accelerator at a
substantially lower per-token inference cost, with the caveat
that it requires model-specific optimization. Produce:
- A one-page executive memo on the implications for the
  organization's accelerator strategy over the next 18
  months
- A scenario set (base, upside, downside) on the realistic
  accelerator portfolio in 24 and 36 months
- The named forecasting-review mechanism the organization
  will run quarterly on this question
- The walk-away triggers that would move the organization
  from NVIDIA-exclusive to mixed-vendor or to a specific
  custom-silicon commitment

**Deliverable:** A compute-and-silicon roadmap document
(15-20 pages) covering:
- The organization's standing forecast on the accelerator,
  memory, interconnect, and packaging roadmap through the
  planning horizon
- The vendor-portfolio-and-exposure register, with the
  specific exposure to HBM supply, advanced packaging
  capacity, and leading-edge node availability
- The scenario set with named triggers for each
- The no-regret moves across the scenarios
- The walk-away triggers for the current vendor commitments
- The quarterly forecasting-review cadence and the named
  owners

---

### Week 3: Physical Infrastructure, Energy, and Siting (6 hours)

**Topics:**
- The power and grid trajectory — datacenter load forecasts,
  ISO interconnection queues, behind-the-meter and on-site
  generation, nuclear-for-AI and SMR deployment, grid
  curtailment and demand response, transmission buildout
- Water, land, and climate exposure — dense-cooling water
  profile, regional water-stress intersection, land
  acquisition and community-and-zoning friction, physical-
  climate-risk discipline, sustainability-disclosure regime
- Cooling, power delivery, and datacenter architecture —
  rack-density trajectory (50 kW → 500 kW+), direct-liquid-
  cooling and immersion, power-delivery evolution (48 V,
  400 V DC, medium-voltage busbar), modular and
  prefabricated construction
- The datacenter-as-industrial-plant transition and the
  organizational-capability question (in-house vs.
  outsourced), reinforced from MOD-406

**Readings:**
- EIA *Short-Term Energy Outlook* and *Annual Energy
  Outlook*, IEA *World Energy Outlook* and *Electricity
  Outlook* — read for the published datacenter-load
  forecasts and the broader electricity trajectory
  <!-- needs-research: refresh the EIA and IEA published
  forecasts at time of use -->
- ERCOT, PJM, MISO, SPP, CAISO, NYISO, ISO-NE published
  interconnection-queue reports and capacity-market
  outlooks; equivalent published materials from TenneT,
  50Hertz, RTE, National Grid ESO; TEPCO, KEPCO
  <!-- needs-research: refresh the ISO interconnection-
  queue and capacity-market reports at time of use -->
- FERC Order 2023 (interconnection-queue reform) and
  subsequent FERC orders relevant to large-load
  interconnection — read for the regulatory trajectory
  on datacenter grid access
  <!-- needs-research: refresh FERC large-load
  interconnection posture at time of use -->
- NRC published materials on SMR licensing, the NuScale,
  X-energy, Kairos, GE Hitachi BWRX-300, Westinghouse AP300,
  TerraPower Natrium, Oklo, and other SMR vendor status,
  the hyperscaler-nuclear PPA announcements (Microsoft-
  Constellation Three Mile Island, Amazon-Talen Susquehanna,
  Google-Kairos)
  <!-- needs-research: refresh the SMR licensing posture,
  the hyperscaler-nuclear PPA landscape, and the realistic
  commercial-operation timelines at time of use -->
- Uptime Institute *Global Data Center Survey* and related
  annual publications — read for the sector-practice
  trajectory and the realistic deployment pattern
  <!-- needs-research: refresh the Uptime Institute survey
  corpus at time of use -->
- WRI Aqueduct and UN WWAP water-stress-mapping materials
  — read specifically for datacenter-siting implications
  (reinforced from MOD-406)
  <!-- needs-research: refresh the water-stress-mapping
  corpus at time of use -->
- IFRS S1 / S2 (climate-related disclosures), CSRD and
  ESRS E1 (EU corporate sustainability reporting on
  climate), US SEC climate-disclosure rule status — read
  as the disclosure envelope the organization operates in
  (reinforced from MOD-406)
  <!-- needs-research: refresh the climate-disclosure
  regime status at time of use -->
- Daniel Yergin — *The New Map* (background on the
  intersection of energy, geopolitics, and industrial
  strategy as it applies to AI-infrastructure siting)

**Exercise:** For a specific proposed multi-gigawatt
datacenter site (choose a US ISO, a European market, or
an Asian market), produce:
- The grid-interconnection feasibility assessment, with
  the realistic commercial-operation timeline
- The water-and-climate-exposure assessment, with the
  mitigation posture
- The nuclear-and-on-site-generation option assessment,
  with the realistic deployment horizon
- The community-and-zoning engagement plan
- The sustainability-disclosure impact
- The go/no-go recommendation with named conditions

See `exercises/exercise-02-strategy-memo.md` for a
structured version.

**Deliverable:** A physical-infrastructure-and-siting
roadmap document (10-12 pages) covering:
- The organization's forward power, siting, cooling, and
  construction posture through the planning horizon
- The regional footprint plan with the specific risk
  register per region
- The nuclear, on-site-generation, and demand-response
  option register
- The sustainability-disclosure posture
- The specific walk-away conditions at which the
  organization withdraws from a region or commitment

---

### Week 4: Model and System Architecture Trajectories (7 hours)

**Topics:**
- The scaling-and-capability trajectory — pre-training
  scaling, data-wall and synthetic data, test-time compute
  and reasoning models, mixture-of-experts and sparse
  activation, state-space and hybrid architectures,
  multimodal and omnimodal architectures
- Agentic systems and long-horizon tasks — tool use and
  function calling, computer-use and browser-use agents,
  multi-agent patterns, agent evaluation and reliability,
  the long-horizon-task economics question
- Memory, context, and long-horizon state — context-window
  extension, agent memory, RAG maturation and hybrids,
  continual learning
- World models, embodied AI, and the robotics and
  scientific-discovery adjacencies — world-model
  trajectory, VLA models and humanoids, AI for science,
  mathematical reasoning and formal verification

**Readings:**
- Public frontier-lab research blogs and research papers
  — Anthropic, OpenAI, Google DeepMind, Meta FAIR / GenAI,
  Microsoft Research AI, Mistral, Cohere, xAI, DeepSeek,
  Qwen / Alibaba, Hugging Face, AI2 — read for the stated
  trajectory on scaling, reasoning, agentic systems, and
  evaluation (reinforced from MOD-404 and MOD-409)
  <!-- needs-research: refresh the frontier-lab research-
  blog corpus at time of use -->
- NeurIPS, ICML, ICLR, FAccT, ACL most-recent accepted
  papers on scaling laws, test-time compute, reasoning,
  agentic systems, memory and context — read for the
  academic baseline against the industry stated trajectory
  <!-- needs-research: refresh the academic-conference
  paper corpus at time of use -->
- Chip Huyen — *AI Engineering* (the practitioner reference
  on the full engineering stack for the current and near-
  horizon model generation)
  <!-- needs-research: confirm current edition at time of
  use -->
- Lilian Weng — *Lil'Log* essays on reasoning, agents,
  evaluation, and the research-trajectory landscape
- Jason Wei, Andrej Karpathy, Eugene Yan, Nathan Lambert,
  Simon Willison, Chip Huyen essays on the current-
  generation model behavior and the realistic serving
  profile — read for the "what is happening vs. what is
  claimed" discipline
- SWE-bench, SWE-Lancer, OSWorld, WebArena, GAIA,
  ARC-AGI, MMLU-Pro, HLE, and successor-benchmark
  publications — read as the operational evaluation
  corpus (reinforced from MOD-404 and MOD-409)
  <!-- needs-research: refresh the agentic-and-reasoning-
  benchmark landscape at time of use -->
- AISI (US) and AISI-UK published evaluations and
  methodology notes — read as the public-sector evaluation
  baseline (reinforced from MOD-405)
  <!-- needs-research: refresh AISI published materials at
  time of use -->

**Case Study:** The organization's product roadmap over
the next 18 months depends on two specific capability
assumptions: (a) that a frontier-class reasoning model can
be served at a target per-token price and per-request
latency, and (b) that an agentic coding and infrastructure-
operations stack reaches a target reliability floor on a
named benchmark before the organization commits to deploy
it into production change windows. Produce:
- A one-page CTO-briefing memo on the capability-trajectory
  evidence base behind each assumption
- A scenario set on each assumption (base, upside, downside)
- The specific external evidence the organization will
  track quarterly to update the forecast
- The product-roadmap contingency plan if one or both
  assumptions fails to hold
- The specific "we were wrong" communication the
  organization will deliver internally and externally if
  the contingency is triggered

**Deliverable:** A model-and-system-architecture roadmap
document (10-12 pages) covering:
- The organization's standing forecast on the scaling,
  reasoning, agentic, and multimodal trajectory through
  the planning horizon
- The named model-family exposure register (frontier-lab
  closed, frontier-lab open-weights, open-weights-only,
  domestic-specialized)
- The capability-trajectory assumption register, with each
  assumption stated, dated, and tied to a specific
  external-evidence tracker
- The product-and-platform implications of the forecast
- The specific no-regret investments across the scenarios
  (evaluation infrastructure, data-provenance infrastructure,
  agentic observability, memory infrastructure)

---

### Week 5: Geopolitics, Industrial Policy, and the Economic Structure of AI (8 hours)

**Topics:**
- Export control and the chip-wars dynamics — US BIS
  trajectory, China response, allied coordination, entity-
  listing and sanctions surface
- Sovereign AI programs and industrial policy — US industrial
  policy (CHIPS and Science Act, national-labs), EU industrial
  policy (Chips Act, AI Factories, EuroHPC JU, Sovereign AI
  Fund), Asian industrial policy, Middle Eastern sovereign
  programs, decoupling and re-coupling patterns
- Capital formation and the economic structure of AI
  infrastructure — hyperscaler capex trajectory, AI-
  infrastructure project finance (CoreWeave, Lambda, Crusoe,
  Nebius, Applied Digital, OCI for AI), utility-model
  economics, model-pricing trajectory, private-market
  valuation and M&A
- Regulatory futures — EU AI Act implementation, US federal
  and state AI regulation, UK/Japan/Korea/Singapore/India/
  Canada/Australia trajectory, AISI network, content-
  provenance regime, AI-industry litigation docket

**Readings:**
- Chris Miller — *Chip War* (reinforced from MOD-406 and
  MOD-407; the foundational narrative on the semiconductor
  supply chain and its geopolitical structure)
- Anu Bradford — *Digital Empires* (reinforced from MOD-407,
  MOD-408, and MOD-409; the regulatory-sphere vocabulary
  that shapes AI governance)
- Dan Wang — annual letter and ongoing writing on Chinese
  industrial policy — read for the "what the state-driven
  development model actually produces" discipline
  <!-- needs-research: refresh the state of Dan Wang's and
  equivalent industrial-policy writing at time of use -->
- Daniel Yergin — *The New Map* (reinforced from Week 3;
  the energy-and-geopolitics frame)
- BIS most-recent AI-and-advanced-computing rules and
  commentary; OFAC AI-adjacent sanctions materials; EU
  Dual-Use Regulation; UK Export Control Joint Unit
  guidance; METI materials
  <!-- needs-research: refresh the export-control rule
  corpus at time of use -->
- EU Regulation 2024/1689 (EU AI Act) implementing-act
  and delegated-act consultations, European AI Office
  published materials, CEN-CENELEC JTC 21 published
  materials
  <!-- needs-research: refresh the EU AI Act implementation
  landscape at time of use -->
- NIST AI 100-1 and 600-1, AISI (US) and AISI-UK published
  materials, OECD AI Policy Observatory corpus, G7
  Hiroshima AI Process documents, Council of Europe AI
  Framework Convention, UN AI Advisory Body final report
  and successor outputs (reinforced from MOD-405 and
  MOD-409)
  <!-- needs-research: refresh the international AI-
  governance corpus at time of use -->
- US state AI law primary sources (Colorado AI Act, Texas
  TRAIGA, California AB 2013 / SB 942 / ADMT, Illinois
  BIPA, NYC Local Law 144) and the sector-specific state-
  regulator corpora (reinforced from MOD-405 and MOD-409)
  <!-- needs-research: refresh the US state AI law
  effective-date and rulemaking docket at time of use -->
- Published hyperscaler earnings calls, 10-K/10-Q filings,
  investor-day presentations, and equity-analyst notes on
  AI capex and depreciation posture
  <!-- needs-research: refresh the hyperscaler financial
  disclosure corpus at time of use -->
- AI-industry litigation docket primary sources — NYT v.
  OpenAI, Authors Guild v. OpenAI, Andersen v. Stability AI
  and equivalents, Getty v. Stability AI, EU music-publisher
  training-data cases, the competition-authority AI docket
  (FTC, DOJ, EC, CMA, BKartA)
  <!-- needs-research: refresh the AI-industry litigation
  docket at time of use -->

**Scenario:** A new US administration announces a
substantial expansion of the BIS AI-diffusion framework
that places the organization's two largest sovereign-
customer markets into a "Tier 2" licensing regime, while
simultaneously the EU AI Office issues an implementing-
act decision that imposes a new provider-and-deployer
documentation obligation on general-purpose AI models the
organization serves. A hyperscaler partner publicly
announces a 40% capex increase for the following 18 months,
and two of the organization's merchant-silicon suppliers
file for bankruptcy within a week of each other, citing
HBM allocation and advanced-packaging capacity shortfall.
Produce:
- A one-page CEO-briefing memo on the aggregate
  implications
- A revised 18-month strategy memo that incorporates all
  four developments
- The specific no-regret moves the organization makes
  immediately
- The walk-away triggers the organization adopts for the
  two sovereign markets and the merchant-silicon exposure
- The thought-leadership plan for communicating the
  organization's revised posture externally (reinforced
  from MOD-409)

**Exercise:** For an open AI-regulation consultation or
rulemaking (select from the then-current docket), produce:
- The one-page internal decision memo on how the
  organization's forward view aligns with (or diverges
  from) the proposed regulation
- The scenario set on the realistic implementation
  trajectory and its implications for the organization
- The specific contingency plan if the regulation is
  adopted as proposed vs. in a materially modified form

See `exercises/exercise-03-stakeholder-mapping.md` for a
structured version.

**Deliverable:** A geopolitics-policy-economics roadmap
document (12-15 pages) covering:
- The organization's standing forward view on the
  export-control, sovereign-AI, industrial-policy, and
  regulatory trajectory
- The named exposure register per region, with the
  specific commitments (customer, partner, datacenter,
  workforce) at risk
- The capital-formation and vendor-exposure register
- The scenario set with named triggers and no-regret
  moves
- The integration with the thought-leadership stack
  (MOD-409) on external communication of the forward
  posture

---

### Week 6: Workforce, Organization, and the Capstone Synthesis (10 hours)

**Topics:**
- The automation of engineering and research work — coding
  agents, research-engineering automation, infrastructure-
  engineering automation, the AI-augmented workforce
  discipline, the disclosure-and-trust question
- Researcher, operator, and executive mobility — the
  frontier-researcher talent cycle, the acqui-hire mechanism,
  the operator and executive labor markets, sovereign and
  policy-adjacent mobility
- AI-native operating models and organizational form — the
  "small senior team heavily augmented" pattern, the
  compensation-and-equity question, governance implications
  (SOX, SOC 2, control environment), the human-in-the-loop
  posture
- Strategic posture and the capstone synthesis — option
  value, no-regret moves, irreversibility, real-options
  framing, portfolio discipline, walk-away triggers, pre-
  committed response, succession and continuity
- Integration with the rest of the senior-architect program
  — the way forecasting feeds and is fed by strategy
  (MOD-401), executive leadership (MOD-402), governance
  (MOD-403), R&D (MOD-404), responsible AI (MOD-405),
  global infrastructure (MOD-406), partnerships (MOD-407),
  M&A (MOD-408), and thought leadership (MOD-409)
- Executive, board, and workforce communication about the
  future — the standing cadence, the risk-committee and
  audit-committee posture, the workforce-communication
  discipline, the external-communication integration

**Readings:**
- Karl Weick — *Managing the Unexpected* and *Sensemaking
  in Organizations* (the foundational references on
  high-reliability organization and the organizational
  discipline of recognizing weak signals early)
- Charles Perrow — *Normal Accidents: Living with High-
  Risk Technologies* (the system-safety baseline against
  which agentic-system deployment is read)
- Nassim Taleb — *Antifragile* (reinforced from Week 1;
  the organizational-posture vocabulary for operating in
  the deep-uncertainty regime)
- Daron Acemoglu and Simon Johnson — *Power and Progress*
  (background on the historical interaction of general-
  purpose technologies with workforce structure and
  distributive outcomes)
- Erik Brynjolfsson, Andrew McAfee, and co-author
  publications on AI-and-labor-market dynamics; the NBER
  Economics of Artificial Intelligence conference corpus
  — read for the empirical baseline on AI augmentation
  and automation
  <!-- needs-research: refresh the AI-and-labor-economics
  corpus at time of use -->
- OECD, World Economic Forum, McKinsey Global Institute,
  Goldman Sachs, Anthropic Economic Index publications on
  the AI-workforce trajectory — read critically for the
  "what is evidence vs. what is extrapolation" distinction
  <!-- needs-research: refresh the AI-workforce-trajectory
  publication corpus at time of use -->
- Published organization-form experiments from AI-native
  companies — the "small team, heavy augmentation"
  pattern as described publicly by frontier-lab and AI-
  tooling-company leadership
  <!-- needs-research: refresh the AI-native-organizational-
  form public-writing landscape at time of use -->
- Gary Klein, HBR — "Performing a Project Premortem"
  (reinforced from MOD-402, MOD-404, MOD-406, MOD-407,
  MOD-408, MOD-409, and Week 1 of this module; applied
  here to the capstone forward-strategy plan)
- Peter Drucker — *The Essential Drucker* and *Managing in
  a Time of Great Change* (the enduring reference on the
  senior-executive discipline of leading an organization
  through structural change)

**Scenario:** The organization's board has asked the senior
architect to produce a capstone forward-strategy document
for a five-year planning horizon. The document must cover:
(a) the technology-trajectory posture across compute, model,
agentic, and physical infrastructure; (b) the geopolitical-
and-regulatory posture across export control, sovereign AI,
and the compliance envelope; (c) the workforce and
organizational-form posture; (d) the explicit no-regret
moves and walk-away triggers; (e) the integration with the
rest of the senior-architect program; (f) the measurement
and governance regime. The document will be reviewed by the
executive team, the board strategy committee, the risk
committee, and the audit committee, and will become the
standing input to the annual strategic planning cycle.
Produce:
- The capstone forward-strategy document (20-30 pages)
- The board-strategy-committee briefing deck (12-15 slides)
- The risk-committee briefing deck (6-8 slides)
- The audit-committee briefing deck (6-8 slides)
- The all-hands workforce-communication outline
- The external-communication plan (reinforced from
  MOD-409)

**Exercise:** Board-level presentation on the organization's
capstone forward strategy — the scenario set, the no-regret
moves, the walk-away triggers, the integration with the
rest of the senior-architect program, and the governance
and measurement regime. See `exercises/exercise-05-
presentation.md`.

**Deliverable:** Board-ready capstone forward-strategy
deck (15-20 slides) covering the full scope above,
reviewed with a peer using the "so what?" test at every
slide.

---

## Case Studies

### Case Study 1: Setting the Capstone Forward Strategy from a Blank Page

**Background:**
- A large enterprise AI-platform vendor has grown rapidly
  over the past three years and now operates frontier-scale
  training infrastructure, a multi-region inference footprint,
  a sovereign-AI partnership program, a formal M&A pipeline,
  and a defensible external voice — the full MOD-401 to
  MOD-409 stack is mature
- The board has asked the senior architect to produce a
  five-year forward strategy that integrates the technology,
  physical-infrastructure, geopolitical, regulatory, and
  workforce trajectories into a single standing document;
  the document will be reviewed annually and will serve
  as the standing input to the strategic planning cycle
- The organization has never run a forecasting program as
  a program; forward views have been produced ad hoc by
  individual executives and have varied substantially from
  quarter to quarter
- The organization operates a Tier-2 international footprint
  (US, EU, UK, Japan, Korea, Singapore, India, UAE), with
  meaningful exposure to export-control, sovereign-AI, and
  regional-regulation trajectories

**Your Role:** Senior AI infrastructure architect, acting
as the owner of the forecasting program and the capstone
forward strategy, reporting into the CTO with dotted lines
to the CEO, CFO, CRO, Chief Research Officer, General
Counsel, Chief Communications Officer, Chief Trust Officer,
and the board strategy committee chair.

**Assignment:**
1. Produce a forecasting program — the standing scenarios,
   the named owners, the quarterly review cadence, the red-
   team discipline, the track-record register, and the
   executive-and-board communication
2. Produce the capstone forward-strategy document — the
   technology, physical-infrastructure, geopolitical,
   regulatory, and workforce trajectories; the no-regret
   moves; the walk-away triggers; the integration with the
   rest of the senior-architect program
3. Produce the governance regime — how the forecasting
   program interacts with the enterprise risk register, the
   strategic planning cycle, the capital-planning cycle,
   the R&D portfolio allocation, and the external-voice
   program
4. Produce the measurement regime — the inputs (scenarios
   produced, review cadence delivered, red-team sessions
   completed), the outputs (no-regret moves executed,
   walk-away triggers that did and did not fire), the
   outcomes (strategic decisions attributable to the
   forecasting program, forecast-track-record accuracy),
   and the explicit anti-vanity-metric discipline
5. Pre-wire the program with CEO, CFO, CTO, CRO, Chief
   Research Officer, General Counsel, Chief Communications
   Officer, Chief Trust Officer, Head of Public Affairs,
   Head of Investor Relations, and the business-unit
   leaders whose plans the forecasting program will
   substantially shape

**Deliverables:**
- Forecasting-program operating model (15-20 pages)
- Capstone forward-strategy document (25-35 pages)
- Governance-regime document (5-7 pages)
- Measurement-regime document (3-5 pages)
- Board strategy-committee briefing deck (12-15 slides)
- Risk-committee and audit-committee briefing packs (8-10
  slides each)
- Board approval memo (2-3 pages)

**Success Criteria:**
- Forecasting program produces at least four quarterly
  scenario updates in the first year without a single
  material "the scenario missed the development" incident
- The capstone forward-strategy document survives the
  first annual review with no material board-level
  objection to the scenario set, the no-regret moves, or
  the walk-away triggers
- At least two strategic decisions in the first year are
  explicitly attributed to the forecasting program (a
  vendor commitment reshaped, a region withdrawn from, a
  partnership structured differently, an R&D bet made or
  not made)
- The forecasting program produces a credible track record
  — stated forecasts, dated outcomes, and an honest
  "where we were wrong" register — within the first 12
  months

---

### Case Study 2: A Discontinuity Event That Forces a Mid-Cycle Pivot

**Background:**
- A mid-size AI-platform vendor has a stated two-year
  strategy built around three specific technology-trajectory
  assumptions: (a) a specific accelerator-vendor roadmap
  will deliver on stated per-generation performance-and-
  cost improvements; (b) a specific model-family capability
  trajectory will reach a target capability threshold within
  18 months; (c) a specific regulatory-trajectory posture
  (in the EU and in two US states) will permit a specific
  deployment model
- Within a four-week window, three material developments
  have occurred: the accelerator vendor has announced a
  substantial delay and performance-shortfall against the
  stated roadmap; a new entrant has published open-weights
  models that materially outperform the model family the
  organization's product depends on, at substantially lower
  cost; the EU AI Office has issued an implementing-act
  decision that changes the compliance envelope for the
  organization's primary EU deployment
- The organization's board strategy committee has called
  an emergency review, scheduled for 10 business days from
  the third event
- The organization has a mature forecasting program (unlike
  Case Study 1), but the discontinuity is beyond the
  scenario set the program had committed to

**Your Role:** Senior AI infrastructure architect, co-
owning the pivot with the CEO, CFO, CTO, CRO, Chief
Research Officer, General Counsel, and Chief Communications
Officer, reporting into the board strategy committee.

**Assignment:**
1. Produce the pivot memo — the honest "we were wrong
   about X" acknowledgement, the revised scenario set,
   the revised no-regret moves, the revised walk-away
   triggers, and the specific strategic decisions the
   organization is making now
2. Produce the forecasting-program retrospective — the
   specific scenario gaps that caused the surprise, the
   red-team posture adjustments, the review-cadence
   changes
3. Produce the stakeholder-communication plan — the
   executive-team pivot briefing, the board-strategy-
   committee emergency review, the risk-committee readout,
   the workforce all-hands, the customer-and-partner
   briefing, the external-voice adjustment (reinforced
   from MOD-409)
4. Produce the 90-day execution plan — the specific
   vendor, product, deployment, workforce, and
   communication changes the organization will make
5. Pre-wire the pivot with CEO, CFO, CTO, CRO, Chief
   Research Officer, General Counsel, Chief Communications
   Officer, Chief Trust Officer, Head of Public Affairs,
   Head of Investor Relations, the business-unit leaders,
   and the board strategy committee chair

**Deliverables:**
- Pivot memo (5-7 pages)
- Forecasting-program retrospective (3-5 pages)
- Stakeholder-communication plan (5-7 pages)
- 90-day execution plan (7-10 pages)
- Board strategy-committee emergency-review deck (10-12
  slides)
- CEO talking-points pack for the first 72 hours (2-3
  pages)

**Success Criteria:**
- The pivot is executed without a material customer,
  partner, or regulator incident attributable to the
  pivot communication
- The forecasting program is explicitly retained and
  reinforced (rather than disbanded) by the board, on
  the strength of the honest retrospective and the
  specific posture adjustments
- The 90-day execution plan meets or exceeds its stated
  commitments without a subsequent credibility-damaging
  walk-back
- The external-voice communication preserves the
  organization's thought-leadership standing (MOD-409)
  through the pivot — including the explicit "we said this
  three months ago and here is what changed" track-record
  posture

---

### Case Study 3: The Capstone Executive Transition and Institutional Continuity

**Background:**
- A large AI-platform vendor's current senior AI
  infrastructure architect has announced a planned
  departure within six months to take a senior public-
  sector AI role (an AISI-equivalent leadership position);
  the departure is amicable, well-publicized, and
  substantively unavoidable
- The board has asked the architect to design the
  transition in a way that preserves the forecasting
  program, the capstone forward-strategy document, and
  the integration with the rest of the senior-architect
  program; the organization has deliberately not
  designated a successor at the same level and intends
  to run a 90-day search while the transition is in
  flight
- The architect has also been invited to continue a
  consulting relationship and board-advisory role with
  the organization after the departure, with the
  explicit expectation that the consulting relationship
  will be publicly disclosed and subject to the
  organization's thought-leadership and conflict-of-
  interest discipline (reinforced from MOD-409)
- The architect's forecasting program, capstone forward-
  strategy document, and external-voice posture have
  been the organization's standing institutional
  position for the past three years; the transition
  must preserve the institutional voice without
  freezing it

**Your Role:** The departing senior AI infrastructure
architect, co-owning the transition with the CEO, CTO,
Chief Research Officer, Chief Communications Officer, and
the board chair, with a six-month handover window.

**Assignment:**
1. Produce the transition plan — the forecasting-program
   handover (standing scenarios, named owners, review
   cadence, red-team discipline, track-record register),
   the capstone forward-strategy handover, the external-
   voice handover (reinforced from MOD-409), the
   relationship handover with hyperscaler, sovereign,
   M&A, and policy counterparties
2. Produce the institutional-continuity document — the
   "what the organization believes" written synthesis
   that outlasts the departing architect, with the
   explicit "my views are no longer the organization's
   views" discipline and the standing update cadence for
   the next incumbent
3. Produce the public-communication plan — the departure
   announcement, the external-voice succession statement,
   the ongoing consulting-and-board-advisory disclosure,
   and the standing conflict-of-interest discipline for
   the new public-sector role (reinforced from MOD-409
   on personal-vs-corporate-brand and clearance
   discipline)
4. Produce the search-and-interim-operation plan — the
   named interim owner for the forecasting program, the
   interim-governance regime, the search-committee
   composition, the specific institutional positions
   the interim regime is authorized to update and the
   positions it is not
5. Pre-wire the transition with CEO, CFO, CTO, CRO, Chief
   Research Officer, General Counsel, Chief Communications
   Officer, Chief Trust Officer, Head of Public Affairs,
   the board chair, the board strategy committee chair,
   the board risk committee chair, and the hyperscaler,
   sovereign, and policy counterparties with whom the
   architect has standing relationships

**Deliverables:**
- Transition plan (10-15 pages)
- Institutional-continuity document ("what the
  organization believes," 20-30 pages)
- Public-communication plan (5-7 pages)
- Search-and-interim-operation plan (5-7 pages)
- Board-briefing deck on the transition (10-12 slides)
- Departure memo to the workforce (2-3 pages)

**Success Criteria:**
- The forecasting program and capstone forward-strategy
  document continue producing quarterly updates through
  the interim-and-search period without a material
  institutional-continuity incident
- The institutional-continuity document is cited by the
  interim regime, the search-committee, and the eventual
  successor as the standing institutional position; the
  successor does not need to rebuild the "what the
  organization believes" artifact from scratch
- The public-voice succession is executed without a
  loss of thought-leadership standing (MOD-409) or a
  regulator-or-customer-visible confusion about who
  speaks for the organization
- The conflict-of-interest discipline for the departing
  architect's new public-sector role is executed
  without a disclosure or clearance incident

---

## Exercises and Activities

The five exercises in `exercises/` are structured so each one feeds
the next. Treat them as a sequence, not a menu.

### Exercise 1: Case Study Analysis (3 hours)
Find a published forward-view artifact from a senior AI-
industry executive or researcher — a CEO letter with a
substantial forward section, a research-lab five-year
agenda, a national-AI-strategy document, a hyperscaler
investor-day presentation, or a published "how I think
about the next five years" essay. Summarize the forward
view, grade the forecasting discipline against the
*Superforecasting* criteria, and extract three lessons for
your own organization's prospective forecasting program.
See `exercises/exercise-01-case-study.md`.

### Exercise 2: 1-Page Strategy Memo (3 hours)
Write a 1-page memo to your CEO, CFO, CTO, CRO, or board
strategy committee chair on a specific forward-strategy
decision — e.g., "Commit to a mixed-vendor accelerator
portfolio starting in year 2 on the specific scenarios
below," or "Withdraw from a named sovereign-AI market on
the specific trigger below," or "Establish a standing
forecasting program with the named owners, cadence, and
measurement regime below." TL;DR, current state,
recommendation, ask, risks, red-line commitments.
See `exercises/exercise-02-strategy-memo.md`.

### Exercise 3: Stakeholder Map + Influence Plan (4 hours)
Map sponsors, supporters, neutrals, and blockers across
CEO, CFO, CTO, CRO, CISO, CPO, General Counsel, Chief
Communications Officer, Chief Trust Officer, Chief Research
Officer, Head of Public Affairs, Head of Investor Relations,
business-unit leaders, worker representation, and at least
one external stakeholder (a regulator, a hyperscaler
counterpart, a sovereign counterpart, a strategic customer,
a board strategy committee member, a research counterpart).
Convert to a 90-day engagement plan for standing up the
forecasting program and the capstone forward strategy,
sequenced through the pre-launch, launch, and sustained-
cadence phases. See `exercises/exercise-03-stakeholder-
mapping.md`.

### Exercise 4: 3-Year Forecasting-Program Roadmap (5 hours)
Draft a 3-year roadmap for the organization's forecasting
program and capstone forward strategy, broken into
quarterly milestones. Each phase: success metrics
(forecasts produced and dated, no-regret moves executed,
walk-away triggers active, forecast-track-record accuracy,
strategic decisions attributable to the program),
investment, key deliverables, and the specific program
delta over the prior quarter.
See `exercises/exercise-04-roadmap.md`.

### Exercise 5: Board-Level Presentation (5 hours)
A 10-slide deck for a board (or board strategy / risk /
audit committee) on the current state and forward plan of
the enterprise forecasting program and capstone forward
strategy — the scenario set, the no-regret moves, the
walk-away triggers, the integration with the rest of the
senior-architect program, and the measurement regime —
reviewed with a peer using the "so what?" test at every
slide. See `exercises/exercise-05-presentation.md`.

---

## Assessment

### Module Quiz

Short strategic-thinking questions — no crisp right answers, defend
your position. See `quiz.md` for the full prompt list.

### Strategic Capstone Forward-Strategy Portfolio (10-12 hours)

A single coherent artifact set built around *one* capstone
forward strategy you would own for a real (or realistic
composite) organization:

1. **Forecasting-program operating model** (15-20 pages,
   CEO- and board-approvable), with standing scenarios,
   named owners, review cadence, red-team discipline,
   track-record register, and executive-and-board
   communication
2. **Capstone forward-strategy document** (25-35 pages)
   covering the technology, physical-infrastructure,
   geopolitical, regulatory, and workforce trajectories;
   the no-regret moves; the walk-away triggers; the
   integration with the rest of the senior-architect
   program
3. **Scenario set** — at least three internally consistent
   scenarios (base, upside, downside, and optionally a
   deep-discontinuity scenario), each with named triggers,
   no-regret moves, and walk-away implications
4. **No-regret-moves catalog** — the standing list of
   investments the organization makes because they are
   positive across every plausible scenario, with the
   explicit "not pet projects, not uncertainty-reducing
   noise" discipline
5. **Walk-away trigger register** — the explicit, dated,
   pre-committed conditions under which the organization
   abandons a major commitment
6. **Measurement regime** — inputs, outputs, outcomes,
   reputational and risk metrics, the anti-vanity-metric
   discipline, the board-and-audit-committee readout
   format
7. **Discontinuity-and-pivot playbook** — the standing
   response patterns when a discontinuity event forces a
   mid-cycle pivot, including the stakeholder-communication
   plan and the thought-leadership-integration posture
   (reinforced from MOD-409)
8. **Board readout deck** (12-15 slides) for the executive
   team and the board, answer-first, with the three
   material risks and the standing responses on the first
   page

All eight artifacts must describe the *same* capstone
forward strategy and must be internally consistent. A
reviewer should be able to spot-check any two and find the
same scenario set, the same no-regret moves, the same walk-
away triggers, and the same measurement regime.

**Evaluation Criteria:**
- **Internal coherence** (25%) — forecasting program, forward
  strategy, scenario set, no-regret moves, walk-away
  triggers, measurement regime, pivot playbook, and board
  readout tell the same story at every altitude
- **Strategic realism** (20%) — the forecasts, scenarios,
  and no-regret moves are specific, time-bound, and
  grounded in the actual compute, physical-infrastructure,
  geopolitical, regulatory, and workforce landscape rather
  than generic placeholder language
- **Forecasting discipline** (15%) — the scenarios, the
  uncertainty vocabulary, the red-team posture, and the
  track-record register are specific and testable, not
  "the organization will monitor developments"
- **Risk discipline** (15%) — the discontinuity, walk-away,
  succession-and-continuity, and over-confidence failure
  modes are addressed at specific rather than reassuring
  altitude
- **Integration** (15%) — the forward strategy demonstrably
  feeds and is fed by MOD-401 through MOD-409; a reviewer
  can trace specific strategic decisions to the forecasting
  program and specific forecasting inputs to the strategy,
  partnership, M&A, and thought-leadership programs
- **Executive communication** (10%) — the board readout is
  answer-first, with the three material risks and standing
  responses on the first page

---

## Resources

### Required Reading

1. **Forecasting, scenario planning, and decision under uncertainty**
   - Pierre Wack — "Scenarios: Uncharted Waters Ahead" and
     "Scenarios: Shooting the Rapids" (*Harvard Business Review*)
   - Peter Schwartz — *The Art of the Long View*
   - Philip Tetlock — *Superforecasting*
   - Nassim Taleb — *The Black Swan* and *Antifragile*
   - Daniel Kahneman — *Thinking, Fast and Slow* (reinforced
     from MOD-402)
   - Gary Klein, HBR — "Performing a Project Premortem"
     (reinforced from MOD-402, MOD-404, MOD-406, MOD-407,
     MOD-408, MOD-409)
   - Carl Sagan — *The Demon-Haunted World*
   - Karl Weick — *Managing the Unexpected* and *Sensemaking
     in Organizations*
   - Charles Perrow — *Normal Accidents*

2. **Technology and industry primary sources**
   - NVIDIA, AMD, Intel, Google, AWS, Microsoft, Meta,
     Oracle, Alibaba most-recent earnings calls and
     investor-day presentations; TSMC, Samsung Foundry,
     Intel Foundry most-recent earnings calls and
     technology-symposium presentations
     <!-- needs-research: refresh the hyperscaler, silicon,
     and fab earnings and investor-day corpus at time of
     use -->
   - ISSCC, Hot Chips, Hot Interconnects, VLSI Symposium,
     NeurIPS, ICML, ICLR, FAccT, ACL most-recent accepted
     proceedings
     <!-- needs-research: refresh the technical-conference
     proceedings relevant to the planning cycle at time of
     use -->
   - SemiAnalysis, The Information, Stratechery, Bloomberg
     Supply Lines, Nikkei Asia semiconductor coverage —
     read for the current trajectory against the stated
     roadmap
     <!-- needs-research: confirm the current reputable
     semiconductor-analyst corpus at time of use -->
   - MLCommons MLPerf Training, Inference, HPC, Storage, and
     AILuminate result sets
     <!-- needs-research: refresh the MLPerf result-set
     landscape at time of use -->
   - Frontier-lab research blogs and research papers from
     Anthropic, OpenAI, Google DeepMind, Meta FAIR / GenAI,
     Microsoft Research AI, Mistral, Cohere, xAI, DeepSeek,
     Qwen / Alibaba, Hugging Face, AI2 (reinforced from
     MOD-404 and MOD-409)
     <!-- needs-research: refresh the frontier-lab research-
     blog corpus at time of use -->

3. **Physical-infrastructure primary sources**
   - EIA *Short-Term Energy Outlook* and *Annual Energy
     Outlook*, IEA *World Energy Outlook* and *Electricity
     Outlook*
     <!-- needs-research: refresh the EIA and IEA published
     forecasts at time of use -->
   - ERCOT, PJM, MISO, SPP, CAISO, NYISO, ISO-NE published
     interconnection-queue and capacity-market reports;
     TenneT, 50Hertz, RTE, National Grid ESO; TEPCO, KEPCO
     equivalents
     <!-- needs-research: refresh the ISO interconnection-
     queue and capacity-market reports at time of use -->
   - FERC Order 2023 and successor orders on large-load
     interconnection
     <!-- needs-research: refresh FERC large-load
     interconnection posture at time of use -->
   - NRC SMR licensing materials; NuScale, X-energy, Kairos,
     GE Hitachi BWRX-300, Westinghouse AP300, TerraPower
     Natrium, Oklo vendor status; hyperscaler-nuclear PPA
     announcements
     <!-- needs-research: refresh the SMR licensing and
     hyperscaler-nuclear PPA landscape at time of use -->
   - Uptime Institute *Global Data Center Survey* and
     related annual publications
     <!-- needs-research: refresh the Uptime Institute
     survey corpus at time of use -->
   - WRI Aqueduct and UN WWAP water-stress-mapping
     materials
     <!-- needs-research: refresh the water-stress-mapping
     corpus at time of use -->
   - IFRS S1 / S2, CSRD and ESRS E1, US SEC climate-
     disclosure rule status
     <!-- needs-research: refresh the climate-disclosure
     regime status at time of use -->

4. **Geopolitics, industrial policy, and regulatory primary sources**
   - Chris Miller — *Chip War* (reinforced from MOD-406 and
     MOD-407)
   - Anu Bradford — *Digital Empires* (reinforced from
     MOD-407, MOD-408, MOD-409)
   - Daniel Yergin — *The New Map*
   - BIS AI-and-advanced-computing rules; OFAC AI-adjacent
     sanctions materials; EU Dual-Use Regulation; UK
     Export Control Joint Unit guidance; METI materials
     <!-- needs-research: refresh the export-control rule
     corpus at time of use -->
   - EU Regulation 2024/1689 (EU AI Act) and the ongoing
     implementing-act and delegated-act consultations;
     European AI Office published materials; CEN-CENELEC
     JTC 21 materials
     <!-- needs-research: refresh the EU AI Act
     implementation landscape at time of use -->
   - NIST AI 100-1 and 600-1, AISI (US) and AISI-UK
     published materials, OECD AI Policy Observatory,
     G7 Hiroshima AI Process, Council of Europe AI
     Framework Convention, UN AI Advisory Body
     (reinforced from MOD-405 and MOD-409)
     <!-- needs-research: refresh the international AI-
     governance corpus at time of use -->
   - US state AI law primary sources (Colorado AI Act,
     Texas TRAIGA, California AB 2013 / SB 942 / ADMT,
     Illinois BIPA, NYC Local Law 144) and sector-
     specific state-regulator corpora
     <!-- needs-research: refresh the US state AI law
     effective-date and rulemaking docket at time of use -->
   - AI-industry litigation docket primary sources — NYT
     v. OpenAI, Authors Guild v. OpenAI, Andersen v.
     Stability AI and equivalents, Getty v. Stability AI,
     EU music-publisher training-data cases, competition-
     authority AI docket (FTC, DOJ, EC, CMA, BKartA)
     <!-- needs-research: refresh the AI-industry
     litigation docket at time of use -->

5. **Workforce, organization, and the human-capital frontier**
   - Daron Acemoglu and Simon Johnson — *Power and Progress*
   - Erik Brynjolfsson, Andrew McAfee, and co-author
     publications on AI-and-labor dynamics; NBER Economics
     of Artificial Intelligence conference corpus
     <!-- needs-research: refresh the AI-and-labor-economics
     corpus at time of use -->
   - OECD, WEF, McKinsey Global Institute, Goldman Sachs,
     Anthropic Economic Index publications on the AI-
     workforce trajectory
     <!-- needs-research: refresh the AI-workforce-
     trajectory publication corpus at time of use -->
   - Peter Drucker — *The Essential Drucker* and *Managing
     in a Time of Great Change*

### Supplementary Resources

- Metaculus AI benchmark forecasts, Good Judgment Open AI
  questions, Manifold AI-related markets, Open
  Philanthropy AI timelines work — as reference forecast-
  track-record corpora
  <!-- needs-research: refresh the AI-forecast-track-record
  landscape at time of use -->
- AI Index (Stanford HAI), State of AI Report (Air Street
  Capital), Epoch AI publications — as reference annual
  landscape documents
  <!-- needs-research: refresh these annual landscape
  documents at time of use -->
- Published senior-executive and senior-researcher essays
  on the future of AI infrastructure (reinforced from
  MOD-409) — Paul Graham, Benedict Evans, Simon Willison,
  Lilian Weng, Chip Huyen, Andrej Karpathy, Eugene Yan,
  Jason Wei, Nathan Lambert, Horace He; Anthropic research,
  OpenAI research, Google DeepMind research, Meta FAIR /
  GenAI, Microsoft Research AI
  <!-- needs-research: refresh the senior-executive and
  senior-researcher essay-and-research-blog landscape at
  time of use -->
- Primary-source national AI strategy documents — US (NSCAI,
  National AI R&D Strategic Plan, Executive Orders on AI),
  EU (EU AI Strategy, European AI Office roadmap), UK (AI
  Opportunities Action Plan, AISI publications), Japan (AI
  Strategy 2022+), Korea (K-AI), Singapore (National AI
  Strategy 2.0), India (IndiaAI Mission), Canada (Pan-
  Canadian AI Strategy), Australia (Safe and Responsible
  AI)
  <!-- needs-research: refresh the national AI strategy
  corpus at time of use -->
- McKinsey, BCG, Bain, Deloitte, PwC, EY, KPMG AI-industry
  publications — read critically, with the explicit
  anti-"consulting-report-as-forecast" discipline
  <!-- needs-research: refresh the consulting-firm AI
  publication corpus at time of use -->
- Industry-analyst thought-leadership frameworks — Gartner
  AI Hype Cycle, Forrester AI Wave, IDC AI MarketScape —
  read for how analyst firms encode trajectory into
  evaluations (reinforced from MOD-409)
  <!-- needs-research: refresh analyst-firm methodology
  publications at time of use -->

See also `resources.md` in this module for the running reading list.

---

## Next Steps

Upon completing MOD-410, you will be prepared to:

1. **Design and run** a forecasting program that translates
   public-and-adjacent evidence into standing scenarios,
   no-regret moves, and option-value decisions the
   organization can act on
2. **Read** the compute, memory, interconnect, packaging,
   and inference-silicon roadmap against the organization's
   workload mix and multi-year capacity plan
3. **Read** the physical-infrastructure roadmap — grid
   interconnection, nuclear and on-site generation, water,
   land, climate exposure, siting, industrial policy —
   against the organization's capital plan and risk appetite
4. **Read** the model-and-system-architecture roadmap —
   scaling, test-time compute, agentic systems, long-
   horizon tasks, multimodality, world models, embodied AI
   — against the organization's product and platform
   roadmap
5. **Read** the policy, geopolitical, and economic
   trajectory stack — export control, sovereign AI,
   industrial policy, regulation, capital formation,
   utility-model economics — against the organization's
   international footprint and strategic position
6. **Read** the workforce and organizational-form
   trajectory — the automation of engineering and research
   work, researcher and operator mobility, AI-native
   operating models — against the organization's talent,
   compensation, and operating-model posture
7. **Govern** the forecasting program as a program —
   standing scenarios, named owners, review cadence, red-
   team discipline, track-record register, executive-and-
   board communication, integration with the rest of the
   senior-architect program
8. **Produce** the capstone forward-strategy document —
   the standing synthesis that outlasts any individual
   executive and becomes the organization's institutional
   position on the future of AI infrastructure

As the capstone of the senior-architect curriculum, MOD-410
does not open onto another module in this series. It opens
onto the senior architect's ongoing institutional practice:
the quarterly forecasting review, the annual capstone
forward-strategy refresh, the board strategy-committee
readout, and the standing integration with the strategy
(MOD-401), executive-leadership (MOD-402), governance
(MOD-403), R&D (MOD-404), responsible-AI (MOD-405), global-
infrastructure (MOD-406), partnership (MOD-407), M&A
(MOD-408), and thought-leadership (MOD-409) programs the
previous nine modules established. The senior architect at
the top of the ladder is defined not by any single artifact
but by the discipline of running this integrated program
quarter after quarter, year after year, through every
discontinuity the AI-infrastructure landscape produces.

---

**Ready to begin?** Start with Week 1: Forecasting and Scenario Discipline.

## Cross-references
- Engineering-level prerequisite: see ai-infra-engineer-learning + ai-infra-senior-engineer-learning
- Solutions repo: ai-infra-senior-architect-solutions/modules/mod-410-future-of-ai-infra
