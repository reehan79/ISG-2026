# Communications and Turnkey Execution Architecture

**Status:** SOURCE OF TRUTH  
**Updated:** 2026-09-12  
**Scope:** execution/communications requirements for the two ISG Model Experiments only.

---

## 1. Core rule

Both Model Experiments must be **scientifically completable in Moscow without any live Pakistan–Moscow Internet connection**.

Live connectivity is valuable and should be used where available, but it is never a scientific single point of failure.

This requirement follows the programme's interpretation of the ISG "turnkey solution" requirement: the randomly assigned station crew must receive everything necessary to execute the experiment from the supplied package and instructions.

---

## 2. What must physically/logically be available in Moscow

The selected experiment package must include, as applicable:

- offline/local executable software;
- preloaded experiment/scenario files;
- experiment configuration and frozen condition assignments;
- crew role cards and instructions;
- unmeasured training scenario;
- automated telemetry/event/action logging;
- report/evidence export;
- printed fallback instructions;
- local copy of the frozen Earth-message script for MARS-LINK;
- USB/offline backup of software/configuration/materials;
- preconfigured developer-supplied laptop(s) if organizer arrangements require them.

The package must be able to start, execute, reset, record and export results without cloud services.

---

## 3. Two logically separate communications paths

### Path A — scientific / mission channel

Used for the controlled experiment.

Conceptual topology:

```text
IST Pakistan Mission Control
        |
 normal terrestrial Internet
        |
Moscow experiment gateway/package
        |
 controlled experiment queue
        |
 5-minute simulated Mars delay
        |
     Mars crew
```

The ordinary Internet path is only the **transport layer**. It does not represent Mars delay.

The experiment software controls:

- release time;
- one-way delay;
- acknowledgement timing;
- allowed message sequence;
- logged timestamps.

For measured MARS-LINK episodes, Earth-message content and timing are frozen before execution.

### Path B — operations / monitoring / media channel

Used for additive real-time activity:

```text
Moscow experiment / crew
        |
 real-time terrestrial link
        |
IST Ground Lab / Mission Control
        |
approved university / technical nodes
```

Possible uses:

- telemetry mirroring;
- run-state monitoring;
- parallel analysis;
- technical coordination;
- video conferencing;
- interviews/media;
- unmeasured showcase activity.

Path B must not contaminate measured scientific episodes.

---

## 4. MARS-LINK live operation

Preferred measured-run behavior:

1. IST sends the pre-authorized Earth message.
2. Moscow receives it over the normal Internet path.
3. The experiment gateway places it in the controlled queue.
4. The message is withheld for exactly the declared 5-minute one-way delay.
5. The crew receives it only after the delay expires.
6. Crew response/acknowledgement is timestamped and handled under the same experiment protocol.

This provides a real IST Earth-Mission-Control role without allowing ordinary Internet latency to substitute for Mars latency.

---

## 5. MARS-LINK link-failure fallback

If live Pakistan–Moscow connectivity fails:

- the Moscow package executes the local copy of the same frozen Earth-message script;
- message content does not change;
- protocol release time does not change;
- simulated 5-minute one-way delay does not change;
- the crew experience and scientific condition remain equivalent.

The run is marked with an evidence field identifying whether Earth messages originated from live IST transport or local deterministic fallback.

The origin field is operational metadata, not a change in the scientific condition.

---

## 6. TWIN-RESILIENCE live operation

TWIN-RESILIENCE does not require a live Earth-control loop.

Its scientific truth/fault assignment remains local in the experiment package.

IST and approved nodes may receive a real-time mirror of:

- relay telemetry;
- twin/reference state where disclosure does not compromise blinding;
- experiment/run status;
- post-decision evidence.

During a measured episode they must not reveal:

- whether the twin/reference is correct or intentionally wrong;
- the hidden ground-truth condition;
- the action the crew "should" take.

The crew's reliance decision must remain independent.

---

## 7. Distributed nodes

Nodes are additive to the scientific core.

During measured episodes they may:

- observe permitted telemetry;
- perform parallel analysis;
- record independent findings;
- support post-episode verification.

They may not:

- send uncontrolled advice to the crew;
- alter the frozen Earth-message script;
- reveal hidden TWIN-RESILIENCE condition truth;
- become required for experiment completion.

For showcase/unmeasured episodes, wider live interaction may be allowed subject to the final operating protocol.

---

## 8. Evidence requirements

Every measured run should record at minimum:

- run / experiment identifier;
- scenario / condition identifier;
- message origin: live IST or local fallback;
- message created time;
- message terrestrial-arrival time where applicable;
- simulated Mars-release time;
- crew receipt/acknowledgement time;
- crew decisions/actions;
- relevant telemetry/state;
- deviations/contamination flags;
- final evidence/report export.

This makes the distinction between **real network transport** and **simulated Mars communication delay** explicit and auditable.

---

## 9. HIL boundary

HIL / KidSat / TwinLink is not required for the scientific Moscow package.

If later used, it remains a separate supplementary physical-shadow activity. It must not change the rule that the selected Model Experiment is independently completable in Moscow.

---

## 10. Later implementation authority

This document defines **what the future implementation must satisfy**, not where code is written.

Implementation remains in the appropriate existing CubeSTEM repositories. The ISG-2026 repository remains the programme/experiment source of truth only.
