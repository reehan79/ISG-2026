# ISG 2026 Programme Source of Truth

**Status:** CONSOLIDATED PLANNING BASELINE  
**Updated:** 2026-09-12  
**Purpose:** single programme-level authority for the ISG model experiment, Pakistan Ground Laboratory, CubeSTEM reference deployment, optional HIL evidence, and December MissionLab Challenge continuity.

---

## 1. Programme objective

Use ISG 2026 to establish and demonstrate an **IST-led Pakistan MissionLab Network** in which a common engineering experiment package can be executed through:

1. deterministic Digital Twin / mission simulation;
2. declared communication and telemetry impairment campaigns;
3. structured crew operating procedures and a transparent priority-aware decision aid;
4. reproducible run identity and evidence export;
5. distributed Pakistan Ground-Laboratory support under IST coordination; and
6. an optional, non-critical simulation-to-physical/HIL shadow replay through TwinLink on representative hardware.

The October outcome should be an **internationally witnessed reference deployment**, not merely a booth/demo. The same experiment/scenario/evidence infrastructure must then flow into the Pakistan MissionLab Challenge instead of creating a second project.

---

## 2. Institutional architecture

### 2.1 National hub

**IST / SSTRL / NCGSA** is the Pakistan Reference University / National Ground-Laboratory hub.

IST remains:

- sole organizer-facing Pakistan interface;
- central Pakistan Mission Control / Ground-Lab hub;
- experiment integration authority;
- evidence archive;
- accreditation/coordination authority for Pakistan nodes;
- primary national media/operations location.

### 2.2 Distributed nodes

The ISG Ground-Lab requirements explicitly allow a distributed national laboratory across other organizations inside Pakistan.

Node classes:

- **Operational University Nodes:** bounded specialist functions, non-critical to measured experiment execution.
- **National Technical Node:** SUPARCO may be invited for a bounded independent telemetry/link-analysis or evidence-validation function, subject to written acceptance.
- **Associate / Observer Institutions:** parallel analysis, outreach and December pipeline; no critical experiment function.
- **International Collaborator:** SQU/Oman may be invited only as a separately disclosed observer/collaborator, not as part of the Pakistan national Ground Laboratory unless organizers explicitly approve.

### 2.3 Single-voice rule

During all organizer-facing operations:

- IST is the single Pakistan voice to the host MCC / crew.
- External-node outputs route through IST.
- No external node may introduce uncontrolled advice into a measured episode.

---

## 3. CubeSTEM positioning

CubeSTEM is the **technology/platform contributor**, not the scientific subject of the ISG experiment.

The technical narrative is:

> one experiment definition -> deterministic simulation -> declared fault/impairment campaign -> evidence -> optional physical-shadow replay.

CubeSTEM should be visible because the infrastructure is used, not because the experiment is written as a product demonstration.

For ISG-facing forms, the preferred institutional partner identity is **IST / SSTRL / NCGSA**. CubeSTEM can be credited accurately in the development-team experience, software/equipment description and technology-platform attribution.

---

## 4. Model Experiment strategy

### 4.1 Primary experiment

**MARS-LINK v2 — Crew-Coordinated Delay-Tolerant Mission Operations under Compound Mars Anomalies**

Status: **PRIMARY / MODIFY-THEN-GO**

Scientific question:

> Under a fixed Mars-like communication delay, do structured onboard procedures and a transparent priority-aware decision aid reduce critical mission/resource violations compared with Earth-dependent operation when the crew must act before an Earth response can return?

Three operating modes:

- **Mode A — Earth-dependent operation**
- **Mode B — structured onboard procedures**
- **Mode C — deterministic priority-aware decision aid**

The delay is an environmental constraint, not the outcome being “proved.”

Measured episodes must use matched scenario variants and a pre-declared counterbalancing assignment. IST may execute the frozen Earth-message script, but message content/timing is standardized. External nodes may observe/analyse in parallel but may not influence measured crew decisions.

### 4.2 Secondary / alternate experiment

**TWIN-RESILIENCE v2 — Calibrated Crew Trust in Digital-Twin-Assisted Remote Asset Operations under Degraded Telemetry**

Status: **HOLD / MODIFY BEFORE SUBMISSION**

The earlier “twin helps diagnose faults” version is too close to a product demonstration. The revised question must include cases where the twin/reference model is intentionally inaccurate, stale or incomplete.

Scientific question:

> Can a crew calibrate trust correctly when raw telemetry is degraded and the Digital Twin/reference estimate may itself be wrong?

This tests automation bias / calibrated trust, not merely whether a Digital Twin is useful.

Submission decision is conditional on:
- organizer preference for multiple proposals;
- sufficient differentiation from MARS-LINK;
- the revised protocol being fully turnkey.

### 4.3 No third experiment

MARTA / AI is not a standalone proposal. Automated Mission Planner is deferred to the later Challenge.

---

## 5. MARS-LINK v2 scientific baseline

### 5.1 Nominal crew design

Nominal measured configuration: **6 crew functions**

1. Mission Commander / Crew Lead
2. Communications Specialist
3. Operations / Flight-Control Engineer
4. Systems / Resource Engineer
5. Data / Verification Officer
6. Independent Observer / Evidence Recorder

If fewer people are assigned, roles merge according to the published fallback map. If more are assigned, surplus crew are evidence observers rather than uncontrolled advisers.

The exact ISG crew size/role structure is not yet treated as verified programme truth.

### 5.2 Communication constraint

Planning baseline:

- **5 minutes one-way**
- **10 minutes round trip**

At least one scenario must require a safe local decision before the round trip can complete. That is the Mars-relevant operational constraint.

### 5.3 Episode design

Planning target:

- 1 unmeasured training episode;
- 9 measured episodes = 3 operating modes × 3 matched scenario families/variants;
- optional terminal baseline/control episode to expose learning effects;
- total experiment package target: approximately **5–6 hours**, subject to organizer crew-time allocation.

The exact ordering is frozen before execution using a reproducible counterbalancing scheme. A fixed A->B->C progression is prohibited.

### 5.4 Primary endpoint

One primary endpoint:

**critical mission/resource constraint violations** (count and, where applicable, cumulative duration).

Secondary endpoints may include:

- mandatory mission-objective completion;
- crew-internal deliberation time, excluding forced communication delay;
- incorrect or unsafe actions;
- message-priority errors / missed acknowledgements;
- recovery time;
- deviation count;
- episode-level workload/coordination observations where ethically and operationally appropriate.

Configured link latency is descriptive context, not a primary finding.

### 5.5 Mode C

Mode C is **not an unvalidated ML controller**.

It is a deterministic, inspectable **Priority-Aware Procedure Aid** with a frozen and published rule set. Any ML work before/after ISG remains shadow/offline analysis unless separately validated and approved.

---

## 6. Experiment-control boundary

### 6.1 Measured episodes

Measured episodes must be scientifically controlled.

- Earth-message content/timing is frozen.
- IST may operate the Earth-side script to preserve real Ground-Lab participation.
- External university/SUPARCO nodes may perform parallel analysis.
- External-node recommendations cannot change the measured crew condition.
- All inbound/outbound messages are logged with source and timestamp.
- If protocol contamination occurs, the affected episode is flagged/excluded rather than silently treated as valid.

### 6.2 Demonstration episode

A separate unmeasured operational/showcase episode may allow:

- live IST Mission Control interaction;
- university-node analysis;
- SUPARCO technical participation if agreed;
- media-safe wallboard;
- broader distributed-MissionLab demonstration.

This keeps media/network value without corrupting the scientific dataset.

---

## 7. HIL / KidSat / TwinLink boundary

HIL is strategically valuable but must remain non-critical.

Allowed October proof:

- one representative scenario;
- same experiment/scenario identity and evidence schema;
- replay against a representative cyber-physical resource at IST through TwinLink/Edge where validated;
- recorded locally before the event;
- used as evidence of simulation-to-physical continuity.

Hard non-claims:

- KidSat is not Mars hardware and not a Mars analogue;
- HIL is not part of the primary ISG scientific result unless specifically accepted;
- no measured episode depends on live Pakistan-Moscow hardware control;
- no unvalidated physical path is a single point of failure.

---

## 8. Turnkey package requirement

A selected Model Experiment must be executable by a randomly assigned crew from supplied instructions.

The planned package therefore includes:

- offline/local executable deployment;
- preconfigured runtime or developer-supplied machines if organizers require;
- USB/offline backup;
- one unmeasured self-paced training scenario;
- role-specific quick cards;
- guided step/progress validation;
- English master instructions;
- Russian quick-start / role-card support where feasible;
- scenario pack and frozen assignment;
- reporting form;
- evidence export;
- printed fallback instructions.

“Browser-based or locally hosted” is not sufficient as a final turnkey definition.

---

## 9. Human-performance data boundary

The experiment evaluates the protocol/system, not individual competence.

Programme baseline:

- report crew/episode-level results;
- de-identify individual performance in any research/publication use;
- do not represent experiment metrics as competition scoring unless organizers explicitly define that;
- follow organizer/institutional consent and data-handling requirements;
- state sample size and avoid broad causal/generalization claims.

---

## 10. Ground-Lab capability baseline

The Pakistan Ground Laboratory should be provisioned against the capabilities named in the ISG Ground-Lab requirements:

- computers and robust Internet (document states from 50 Mb/s);
- design engineering / 3D modelling / circuit tools where relevant;
- control software / ROS access;
- communications / GNURadio / SDR# access;
- information/media recording and publishing tools;
- advantageous access to fabrication / soldering / experiment hardware.

These are capability requirements, not necessarily one separate person per tool category.

Node selection should fill capability gaps, not maximize logos.

---

## 11. October -> December continuity

October and December are one programme if the artifacts are reused.

October artifacts to become December assets:

- experiment/scenario pack;
- impairment/fault campaign;
- experiment runner;
- evidence schema;
- reporting/export;
- node console;
- role/training materials;
- optional physical-shadow path.

December adds challenge missions, qualification/scoring and wider participation; it must not rebuild the platform.

---

## 12. Success criteria for October

October counts as a strong CubeSTEM/IST reference if:

1. a randomly assigned external/international crew can execute the package from instructions;
2. experiment runs are reproducible and evidence lineage is preserved;
3. a second institution can execute the same pack independently and produce compatible evidence;
4. null/negative outcomes are captured honestly;
5. one bounded simulation-to-physical evidence-continuity proof exists without overclaim;
6. IST visibly operates the distributed Pakistan Ground-Lab network.

---

## 13. Hard boundaries

Do not:

- claim “Mars AI” for the rule-based aid;
- claim autonomous physical control that is not validated;
- call KidSat Mars hardware;
- name SUPARCO/RESOLVE/SQU as confirmed partners before written acceptance;
- present SQU as part of Pakistan's national Ground Lab without organizer approval;
- let node inputs alter measured episodes;
- state unverified ISG crew structure or event dates as settled;
- create a second physics/execution authority in this repository.
