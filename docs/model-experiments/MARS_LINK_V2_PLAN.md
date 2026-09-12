# MARS-LINK v2 Experiment Plan

**Working title:** Crew-Coordinated Delay-Tolerant Mission Operations under Compound Mars Anomalies  
**Status:** PRIMARY / MODIFY-THEN-GO  
**ISG area:** settlement automation, fault-tolerant communications, crew operations  
**Execution style:** software-first, offline-capable, crew-executed turnkey package

---

## 1. Scientific question

Under a fixed Mars-like communication delay, do structured onboard procedures and a transparent priority-aware procedure aid reduce critical mission/resource violations compared with Earth-dependent operation when action is required before an Earth response can arrive?

This is a pilot/technical study under the tested crew and scenario conditions. It is not intended to establish population-level human-performance causality.

---

## 2. Hypothesis

For time-critical compound anomalies in which the safe-action deadline is shorter than the Earth round-trip communication delay:

- Earth-dependent operation will incur more critical constraint violations;
- structured onboard procedures will reduce those violations; and
- a deterministic priority-aware procedure aid may further reduce prioritization/omission errors.

The priority aid is deterministic and published. No ML result is required for experiment completion.

---

## 3. Independent variable

**Operational support mode**

### Mode A — Earth-dependent

Crew is expected to seek/await Earth guidance for non-preauthorized decisions according to the supplied protocol.

### Mode B — structured onboard procedures

Crew uses a pre-authorized, printed/in-software procedure set and acts locally within declared limits.

### Mode C — priority-aware procedure aid

Crew uses Mode B procedures plus a deterministic local aid that:

- ranks hazards using declared severity/resource/time-to-threshold rules;
- identifies mandatory immediate actions;
- separates “act now” from “await Earth” items;
- never directly commands hardware.

Rules are versioned and included in the experiment package.

---

## 4. Communication profile

Planning baseline:

- one-way Earth-Mars delay: **5 minutes**
- round trip: **10 minutes**

The link may additionally include a declared acknowledgement impairment or brief scheduled outage in designated scenarios, but these are scenario conditions, not separate hypotheses.

The numeric profile must be frozen in the final Appendix 1 submission.

---

## 5. Scenario families

Use matched-difficulty variants so the crew does not replay the same script.

### Family R — Resource / energy emergency

Example structure:

- decreasing energy reserve / power-generation derate;
- one mandatory mission task competes for power;
- a critical threshold will be crossed before Earth guidance can return unless local action is taken.

### Family C — Communications / relay degradation

Example structure:

- intermittent/acknowledgement-degraded link;
- competing priority messages;
- one critical operational message must be identified and acted upon locally.

### Family S — Systems / mission conflict

Example structure:

- remote subsystem anomaly or resource leak;
- telemetry contains one distracting non-critical anomaly;
- local crew must protect the critical resource while preserving as much mission value as possible.

Each family must have equivalent variants with different parameter values/event ordering so learning does not explain mode differences.

---

## 6. Crew configuration

Nominal functions: **6**

| Role | Responsibility |
|---|---|
| Mission Commander | final crew decision; episode start/end authority |
| Communications Specialist | Earth queue, acknowledgements, priority traffic |
| Operations / Flight-Control Engineer | executes permitted operational actions |
| Systems / Resource Engineer | watches thresholds and reports state |
| Data / Verification Officer | verifies resets/logging and exports evidence |
| Independent Observer / Evidence Recorder | manual timestamps, deviations, photo/video evidence |

Fallback minimum: 3 crew, using a published role-merge map.

Any additional assigned crew are used as observers/evidence recorders, not uncontrolled advisers.

---

## 7. Episode matrix

Planning target:

- Training: 1 unmeasured episode.
- Measured: 9 episodes = 3 modes × 3 scenario families/variants.
- Optional final control: one repeated baseline-class episode to expose learning/order effects.

The mapping of modes to matched scenario variants is frozen before the run using a reproducible counterbalancing/randomization record.

**Prohibited:** fixed A -> B -> C order on identical scenarios.

---

## 8. Duration target

Planning target: approximately **5–6 hours cumulative**, inclusive of briefing, training, measured episodes, resets and evidence export.

Working estimate:

- setup/briefing: 20 min;
- training: 20 min;
- 9 measured episodes at about 25 min: 225 min;
- controlled resets/short breaks: about 45–60 min;
- final export/debrief: 30 min;
- optional learning-control episode: +25 min if crew allocation permits.

Final numbers must close arithmetically in Appendix 1.

A reduced contingency protocol may be defined, but must explicitly state which episodes/overheads are removed.

---

## 9. Primary endpoint

**Critical mission/resource constraint violations**

Record:

- count per episode;
- cumulative duration where meaningful;
- affected constraint;
- whether violation was reversible/recovered.

Primary analysis compares episode-level outcomes across operating modes within the limits of the small pilot sample.

---

## 10. Secondary evidence

- mandatory mission objective completion;
- crew-internal deliberation time (forced link delay excluded);
- unsafe/incorrect actions;
- message-priority/acknowledgement errors;
- recovery time;
- procedural deviation count;
- final mission/resource state;
- crew-level workload observation/questionnaire only if organizer/institutional requirements permit.

Configured communication latency is descriptive, not an outcome.

---

## 11. Earth-side control

Measured runs use a **frozen Earth-message script**.

Preferred operational implementation:

- IST Pakistan Mission Control transmits the standardized messages at protocol-defined times;
- content/timing cannot be improvised;
- if the external link is unavailable, the same script executes locally without changing the scientific condition;
- all messages carry source and timestamp.

University/SUPARCO nodes may run parallel analysis but cannot alter measured crew decisions.

A separate unmeasured showcase episode may use live node input.

---

## 12. Turnkey package

Required before deployment:

- offline local installer/runtime;
- preconfigured environment or supplied machines as agreed with organizers;
- USB backup;
- scenario/episode bundle;
- deterministic mode/scenario assignment manifest;
- English master instructions;
- Russian quick-start/role cards where feasible;
- per-role one-page cards;
- built-in training episode;
- guided step validation;
- experiment report form;
- evidence export package;
- printed emergency/fallback procedure.

---

## 13. Safety / data handling

Software-only execution is the default.

Crew-performance evidence is treated as experiment/protocol evidence, not individual competence scoring by the development team.

Any research/publication use should use de-identified crew/episode-level data and comply with organizer/institutional consent/data requirements.

---

## 14. CubeSTEM technology boundary

MARS-LINK uses CubeSTEM MissionLab / Digital Twin infrastructure for scenario execution, controlled impairments and evidence.

It must not claim:

- autonomous Mars habitat control;
- flight-qualified AI;
- measured physical evidence unless separately captured;
- a high-fidelity “digital twin of a Mars habitat” unless the implemented model actually satisfies that claim.

---

## 15. Optional physical-shadow extension

Not part of the measured ISG result.

One selected scenario may be replayed locally at IST on a representative cyber-physical resource through TwinLink/Edge, preserving experiment/scenario identity and evidence schema.

Primary artifact: recorded evidence/video, not a live cross-border dependency.
