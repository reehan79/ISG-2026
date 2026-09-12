# October Build Plan and Cross-Repository Work Packages

**Status:** planning baseline  
**Principle:** build only what is necessary to make the selected ISG experiment turnkey, scientifically controlled, reproducible and reusable in December.

This repository owns programme plans and experiment artifacts. Numerical/physical implementations should be made in their authoritative repositories rather than forked here.

---

## 1. Cross-repository authority

### ISG-2026 repository

Owns:

- experiment protocol;
- scenario/fault specifications at programme level;
- role cards/instructions;
- Ground-Lab/node scopes;
- submission artifacts;
- rehearsal/evidence checklists;
- programme status.

### digital-twin repository

Owns:

- numerical mission/scenario behaviour;
- G3 Experiment / Scenario / FaultCampaign / ExecutionPlan integration;
- deterministic simulation/replay;
- RunManifest / EvidenceEnvelope integration;
- evidence export;
- MissionLab UI/experiment runner.

### cubestem-twinlink repository

Owns:

- physical-resource session/transport boundary;
- telemetry/command transport;
- optional physical-shadow path.

### cubestem-edge-node repository

Owns:

- local physical authority/safety boundary;
- representative hardware integration where accepted.

No ISG-specific shortcut may redefine these boundaries.

---

## 2. Work-package map

### WP0 — Protocol freeze

**Priority:** P0  
**Repository:** ISG-2026

Deliverables:

- MARS-LINK v2 hypothesis;
- numeric delay;
- scenario families;
- crew roles;
- primary/secondary endpoints;
- episode matrix;
- deterministic Mode C rule set;
- measured/showcase boundary;
- Appendix 1 final content.

Acceptance:

- every Appendix 1 field can be answered without “TBD” on a scientific variable;
- duration arithmetic closes;
- procedure is coherent under the configured delay.

---

### WP1 — Mars operations scenario pack

**Priority:** P0  
**Implementation:** digital-twin

Build a bounded, reduced-order operations environment sufficient for the experiment.

Required scenario families:

- resource/energy emergency;
- communications/relay degradation;
- systems/mission conflict.

Requirements:

- matched-difficulty variants;
- known ground truth;
- deterministic seeds/configuration;
- safe reset;
- no arbitrary browser physics changes;
- scenario IDs/version hashes.

Do not claim a full high-fidelity Mars-habitat twin.

---

### WP2 — Communication / telemetry impairment layer

**Priority:** P0  
**Implementation:** digital-twin / existing FaultCampaign seams

Required first vocabulary:

- fixed one-way delay;
- delayed acknowledgement;
- brief scheduled outage;
- dropout;
- freeze;
- staleness;
- bounded bias.

For MARS-LINK, communication delay is frozen as an experimental environmental condition.

For TWIN-RESILIENCE v2, twin/reference mismatch is a separate controlled condition.

---

### WP3 — Experiment runner

**Priority:** P0  
**Implementation:** digital-twin

Functions:

- experiment ID / version;
- scenario ID / variant;
- mode assignment;
- deterministic reset;
- training-vs-measured flag;
- start/end timestamps;
- crew-action log;
- Earth-message log;
- contamination/deviation flag;
- primary endpoint calculation;
- secondary metric export;
- evidence/package export.

Acceptance:

- identical configuration can be replayed;
- run identity/evidence lineage is preserved;
- scenario order is not manually improvised during execution.

---

### WP4 — Frozen Earth script and Mode C rules

**Priority:** P0  
**Implementation:** protocol in ISG-2026 + runtime representation in digital-twin

Earth script:

- message text;
- release time;
- expected acknowledgement;
- allowed fallback;
- no live improvisation in measured episodes.

Mode C:

- deterministic priority categories;
- severity/time-to-threshold rules;
- action-vs-await-Earth recommendation;
- human-readable rationale;
- no automatic physical action.

---

### WP5 — Turnkey packaging

**Priority:** P0  
**Implementation:** deployment/documentation

Deliverables:

- offline local runtime/installer;
- dependency lock;
- USB backup;
- supplied/preconfigured workstation plan if required;
- self-paced training scenario;
- guided step validation;
- English instructions;
- Russian quick-start / role cards where feasible;
- printed fallback instructions;
- result/report template.

Acceptance:

- fresh operator can execute training and one sample episode without developer intervention.

---

### WP6 — Evidence and reporting

**Priority:** P0

Required outputs:

- run manifest / identity;
- evidence envelope or equivalent accepted evidence object;
- event timeline;
- Earth-message timeline;
- crew actions;
- primary endpoint result;
- secondary metrics;
- manual observer/deviation log;
- export bundle hash;
- final crew report form.

This is the key commercial/research artifact.

---

### WP7 — Ground-Lab / node console

**Priority:** P1

Minimum:

- read-mostly mission state;
- timestamped telemetry/events;
- scoped access;
- parallel-analysis export;
- no measured-episode command path for external nodes.

A public/media wallboard may be a separate read-only projection.

---

### WP8 — Optional physical-shadow/HIL proof

**Priority:** P2 / non-critical  
**Implementation:** TwinLink + Edge + representative hardware

One scenario only.

Acceptance:

- same experiment/scenario identity vocabulary;
- representative hardware labelled honestly;
- local IST execution succeeds repeatedly before event;
- evidence/video recorded;
- failure does not affect ISG scientific experiment.

Do not build production-wide HIL infrastructure merely for October.

---

### WP9 — Post-ISG analysis / December extension

**Priority:** after October

May include:

- offline ML analysis over collected evidence;
- Automated Mission Planner challenge track;
- broader TwinLink/HIL tasks;
- school/junior MissionLab track;
- MissionLab Node packaging;
- December scoring/ranking layer.

These are explicitly not P0 October requirements.

---

## 3. Development stop rules

Stop adding features if any P0 item is not yet turnkey.

Do not trade:

- reproducibility for visuals;
- offline reliability for live cloud dependency;
- scientific control for node/media interaction;
- evidence export for AI features;
- rehearsed instructions for extra scenarios.

---

## 4. October acceptance demonstration

The minimum successful programme demonstration is:

```text
frozen ExperimentDefinition / protocol
 -> matched scenario variant
 -> declared impairment campaign
 -> deterministic run
 -> standardized IST Earth messages
 -> crew action
 -> evidence export
 -> repeat/replay
 -> second-institution execution
 -> optional local physical-shadow replay
```

That chain is the October product proof.
