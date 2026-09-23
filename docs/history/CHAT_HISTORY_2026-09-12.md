# Chat / Decision History — ISG 2026 Model Experiments

**Date covered:** 12 September 2026  
**Purpose:** preserve the reasoning, alternatives, critiques and final decisions that led to the current two-experiment source of truth.

This is a structured reconstruction of the visible working conversation in this chat. It is not an implementation plan. Where ideas were later rejected or changed, that evolution is recorded explicitly.

---

## 1. Starting objective

The discussion began from a broader strategic question: how to use Pakistan/IST participation in International Space Games 2026 to create simultaneous value for:

- IST / SSTRL / NCGSA;
- Pakistan's national Ground Laboratory;
- participating students/universities;
- sponsors/media;
- CubeSTEM and its Digital Twin / TwinLink platform;
- future international funding, sales and reference deployments.

The user emphasized three desired outcomes:

1. participate credibly in ISG and secure/organize the broader international activity;
2. use the opportunity as a large national/media event involving other universities;
3. intentionally prove CubeSTEM / Digital Twin / TwinLink capability in a way that could later support international funding, partnerships and sales.

A recurring constraint was that the technical experiment must remain real and credible rather than becoming a marketing stunt.

---

## 2. First architecture discussion

The early consolidation proposed one umbrella programme with three layers:

1. ISG Model Experiment in Moscow;
2. Pakistan/IST Ground Laboratory and distributed university nodes;
3. later Pakistan MissionLab Challenge using the same infrastructure.

The strategic idea was that October/ISG should become an **international reference deployment**, while the later Challenge would reuse and expand the same platform.

The initial strongest Model Experiment direction was a communications/autonomy experiment combining:

- Mars-Earth communication delay;
- limited bandwidth/intermittent connectivity;
- emergency message prioritization;
- structured procedures;
- decision support.

This evolved into the working name **MARS-LINK**.

A second experiment direction explored Digital-Twin-assisted fault diagnosis and simulation-to-hardware continuity, which evolved into **TWIN-RESILIENCE**.

---

## 3. AI discussion

The existing CubeSTEM AI work was reviewed conceptually:

- AI-Alpha-1 had accepted analysis-only ML workflow capability;
- AI-Alpha-2 was not complete and should not be treated as production-ready autonomous intelligence.

The discussion initially considered whether to accelerate AI to strengthen the ISG story.

The final direction changed after critique:

- no standalone MARTA/AI experiment;
- no dependency on ML for October;
- MARS-LINK Mode C becomes a **deterministic, transparent, priority-aware procedure aid**;
- any ML can later be used in shadow/offline/post-hoc analysis, not as required scientific control authority.

Reason: transparency, reproducibility and scientific defensibility are more valuable than an "AI" label.

---

## 4. HIL / TwinLink / KidSat discussion

The user wanted HIL to remain visible because it could strengthen funding, product credibility and later sales.

The discussion considered several possibilities:

- putting hardware directly into every Model Experiment;
- using KidSat as a physical extension;
- using TwinLink to switch between simulated and physical providers.

The final boundary became:

- **HIL is strategically valuable but optional**;
- no Moscow scientific result depends on live hardware;
- KidSat is never described as Mars hardware or a Mars analogue;
- any later HIL use is a representative cyber-physical physical-shadow replay;
- one scenario can later be replayed locally at IST with the same experiment/scenario/evidence identity.

This preserves the simulation-to-physical narrative without creating a fragile international dependency.

---

## 5. Ground-Lab and node architecture discussion

The ISG Ground-Based Laboratory requirements were read and found to explicitly allow a **distributed national laboratory**, with participants working remotely or from other organizations inside the participating country.

This led to the node concept:

- IST/SSTRL/NCGSA remains the Pakistan Reference University / national hub;
- selected universities can be specialist nodes;
- SUPARCO can conceptually be a national technical node because the document does not restrict nodes to universities;
- external nodes must not dilute IST's authority;
- IST remains the sole organizer-facing Pakistan interface / Mission Control.

Potential node roles discussed included:

- communications / SDR analysis;
- controls / ROS;
- AI/fault analysis;
- independent telemetry/evidence review;
- media/science communication.

The discussion also considered SQU/Oman. Because the national Ground Laboratory is required to be inside the participating country, SQU should not be represented as part of the Pakistan national Ground Lab unless ISG explicitly approves that status. It may later be an international observer/collaborator.

The node concept was considered commercially valuable because a distributed MissionLab deployment can later support a "MissionLab Node" institutional product model.

---

## 6. SUPARCO discussion

The user asked specifically whether SUPARCO could be a node.

The conclusion was:

- yes, in principle, under the "other organizations" wording of the Ground-Lab rules;
- it is better positioned as a bounded **National Technical Node / Partner** than merely another university node;
- possible roles include link/telemetry analysis, independent evidence validation, technical observation or ground-segment expertise;
- SUPARCO must not be described publicly as confirmed until written agreement exists;
- it should not be placed on the scientific critical path.

---

## 7. Original MissionLab Challenge / funding context

The existing approved Pakistan CubeSat MissionLab Challenge minute sheet and annexures were ingested.

They already contained the basic progression:

Digital Twin -> remote real hardware -> telemetry/anomaly/autonomy -> final demonstration.

They also already contemplated:

- universities and STEM institutions;
- SUPARCO/SEAD/RESOLVE/NASTP/NICAT;
- industrial-partner technical support;
- MissionLab Arena;
- outreach/media;
- remote hardware access.

The broader discussion explored how ISG could enhance the original concept and how later funding/sponsorship might be structured transparently.

Important decision for the current repository: those financial/approval/outreach topics are **not part of the current two-experiment source-of-truth scope** and were subsequently removed from this repository.

---

## 8. ISG Model Experiment regulation review

The later/current ISG regulation clarified:

- no more than three scientific studies/technical tests under the regulation wording;
- selected experiments are carried out by Martian-station crews;
- experiments must be Mars-relevant and scientifically justified;
- they must be feasible in the 1–2 day expedition period;
- they must be turnkey;
- current application deadline: 12 Sep 2026;
- organizer review / short clarification: 21 Sep 2026;
- equipment delivery if necessary: 1 Oct 2026.

Appendix 1 requires:

1. experiment name;
2. partner institution;
3. developers;
4. development-team experience;
5. concise experiment description;
6. crew count;
7. total duration and repetitions;
8. Mars relevance, hypothesis and expected result;
9. equipment/materials;
10. step-by-step procedure;
11. completion/verification criteria;
12. crew reporting form;
13. skills;
14. safety.

This caused the conversation to narrow from the broad programme into two submission-quality scientific experiments.

---

## 9. Initial two-experiment plan

The initial submission strategy was:

### MARS-LINK
Delay-tolerant and priority-aware Mars operations.

Initial contrast:

- Earth-command dependence;
- preplanned/structured procedures;
- AI/rule-assisted decision support.

### TWIN-RESILIENCE
Digital-Twin-assisted diagnosis/recovery under degraded telemetry.

The first drafts used smaller crew counts and relatively short experiment structures.

---

## 10. Crew-role critique

The user then raised an important concern: if ISG crews contain multiple specialists and experiments are randomly assigned, an experiment using only two people may underuse the operational setting.

The technical-specification example was considered.

The experiment design was revised toward crew-level roles.

MARS-LINK evolved to use:

- Mission Commander;
- Communications Specialist;
- Operations / Flight-Control Engineer;
- Systems / Resource Engineer;
- Data / Verification Officer;
- Independent Observer / Evidence Recorder.

TWIN-RESILIENCE uses a smaller engineering team but still includes independent evidence recording.

The exact official ISG crew size was not treated as verified solely from the supplied rules.

---

## 11. Claude independent critique

A detailed independent-review pack was created and shared with Claude.

Claude's critique identified several important weaknesses:

- unspecified communication delay;
- fixed A->B->C order creates a major learning confound;
- too many co-primary outcomes;
- turnkey claim needed stronger offline packaging;
- live Earth-side participation could contaminate measured conditions;
- TWIN-RESILIENCE risked being a product demonstration;
- crew-performance data needed a clearer ethics/data boundary;
- extra crew could be used as independent evidence observers;
- node inputs should be separated from measured scientific conditions.

Claude recommended one experiment only, but that recommendation partly relied on an ambiguity in the regulation wording. The broader chat retained the fact from direct organizer correspondence that Ms. Lada had invited Pakistan to submit **1–3 proposals**, so the final direction remained two distinct proposals.

---

## 12. MARS-LINK v2 realignment

After critique, MARS-LINK was substantially changed.

Final working design:

**MARS-LINK — Crew-Coordinated Delay-Tolerant Mission Operations under Compound Mars Anomalies**

Scientific question:

Does structured local operation reduce critical mission/resource violations compared with Earth-dependent operation when Mars delay makes an Earth response arrive too late?

Frozen communication constraint:

- 5 minutes one way;
- 10 minutes round trip.

Operating modes:

- Mode A: Earth-dependent;
- Mode B: structured onboard procedures;
- Mode C: deterministic priority-aware procedure aid.

Scenario families:

- resource/energy emergency;
- communications/relay degradation;
- systems/mission conflict.

Design:

- matched variants;
- no repeated identical scenario under fixed A->B->C order;
- counterbalanced sequence;
- one unmeasured training episode;
- 9 measured episodes;
- 6 crew roles;
- total target 5 h 15 min.

Primary endpoint:

**critical mission/resource constraint violations**.

The delay itself is context, not the scientific outcome.

---

## 13. TWIN-RESILIENCE v2 realignment

Claude's strongest criticism of the original TWIN-RESILIENCE concept was accepted: "the Digital Twin helps fault diagnosis" has an almost predetermined answer and reads like a product demo.

The experiment was redesigned around **calibrated trust**.

Final working design:

**TWIN-RESILIENCE — Calibrated Crew Trust in Digital-Twin-Assisted Remote Asset Operations under Degraded Telemetry**

Concrete remote asset:

**Mars Surface Communications and Power Relay**.

Controlled conditions include:

1. healthy telemetry + correct twin/reference;
2. degraded telemetry + correct/useful twin;
3. degraded telemetry + stale/wrong twin;
4. ambiguous/unmodelled case requiring corroboration.

The crew is blinded to the active condition.

Primary endpoint:

**incorrect reliance decisions**.

This tests whether the crew can determine when the twin should and should not be trusted.

Run structure:

- one training episode;
- 8 measured episodes;
- 5 crew roles;
- total target 4 h 45 min.

---

## 14. CubeSTEM positioning decision

The discussion repeatedly emphasized that CubeSTEM visibility should come from **actual use**, not excessive branding.

Final submission discipline:

- Partner/institution field: IST / SSTRL / NCGSA;
- CubeSTEM may be credited factually as the MissionLab / Digital Twin technology/platform contributor in team experience/software description;
- the scientific experiment is not framed as a CubeSTEM product validation exercise.

The desired longer-term reference is that an international crew used a CubeSTEM-enabled experiment package successfully, not that CubeSTEM had the largest logo.

---

## 15. Repository-scope correction

A dedicated `reehan79/ISG-2026` repository was created.

An initial mistake expanded it into Ground-Lab/development work packages.

The user corrected the scope explicitly:

> the repository is not for development; development remains in the Digital Twin and other existing repositories; the ISG repository is source of truth only; the immediate target is the two Model Experiments.

The repository was then refocused.

Current repository role:

- experiment source of truth;
- submission protocol;
- hypotheses;
- crew roles;
- measurements;
- communication/execution constraints;
- decision history.

It is not an implementation repository.

---

## 16. Final question: what goes to Moscow and what runs live?

The user then asked whether the Moscow experiment should be an offline pack or run in real time with Pakistan, and how the communications links should work.

The final answer was **hybrid with offline scientific independence**.

### Moscow package

The selected experiment must be independently executable from a complete local package:

- offline/local software;
- scenarios;
- role cards/instructions;
- training scenario;
- telemetry/event logging;
- evidence/report export;
- local Earth-message script for MARS-LINK;
- USB/printed fallback material;
- preconfigured machines if required by organizer arrangements.

### MARS-LINK live Earth side

IST may act as the real Earth Mission Control.

But:

- Pakistan-Moscow ordinary Internet is only the transport layer;
- the experiment software imposes the 5-minute simulated Mars delay;
- measured Earth-message content/timing remains frozen;
- if the live link fails, Moscow locally generates the exact same scripted Earth message with the exact same simulated delay.

Therefore live IST participation does not become a scientific dependency.

### TWIN-RESILIENCE live Earth side

The experiment truth/fault assignment remains local in Moscow.

IST/nodes may receive mirrored telemetry for observation/parallel analysis, but during measured episodes they must not reveal whether the raw telemetry or twin/reference is correct.

### Two-path architecture

**Path A — scientific/mission channel**

Controlled messages, simulated Mars delay, deterministic scientific condition.

**Path B — operations/monitoring/media channel**

Real-time telemetry mirroring, coordination, video/media, node analysis and unmeasured showcase activity.

This architecture was then added to the repository as source of truth.

---

## 17. Current state at end of this history

The current source-of-truth position is:

### Proposal 1
**MARS-LINK v2 — READY submission baseline**

Core idea: decision-making under Mars communication delay.

### Proposal 2
**TWIN-RESILIENCE v2 — READY submission baseline**

Core idea: calibrated trust in Digital Twin/reference information under uncertain telemetry.

### Shared execution rule
Both are fully local/offline-capable in Moscow.

### Live Pakistan role
Useful and desired, but never a scientific single point of failure.

### Nodes
Useful for distributed Ground-Lab support/parallel analysis, but must not contaminate measured conditions.

### HIL
Supplementary only; not needed for ISG scientific completion.

### AI
No ML dependency in the formal experiment; Mode C is deterministic.

### Repository
Source of truth only. Later implementation belongs in the existing technical repositories.
