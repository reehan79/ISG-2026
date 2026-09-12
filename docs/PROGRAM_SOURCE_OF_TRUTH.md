# ISG 2026 Model Experiment Submission Source of Truth

**Status:** SUBMISSION BASELINE  
**Updated:** 2026-09-12  
**Current scope:** only the two Model Experiment proposals.

---

## 1. Governing ISG constraints

The current regulation requires each Model Experiment to:

- be implemented by the Martian-station crew according to supplied instructions;
- be scientifically/technically relevant to a Martian expedition;
- account for constrained resources/energy/operations;
- be feasible within the 1–2 day expedition period;
- be delivered as a turnkey experiment with instructions;
- state crew count, total duration/repetitions, hypothesis, expected result, equipment/materials, step-by-step procedure, verification criteria, reporting form, skills and safety.

Current dates in the supplied regulation:

- application: 12 September 2026;
- organizer review / 5-minute clarification: by 21 September 2026;
- equipment delivery, if required: by 1 October 2026.

Ms. Lada's direct communication invited Pakistan to submit 1–3 proposals. The current plan is to submit **two distinct proposals**.

---

## 2. Proposal 1 — MARS-LINK v2

**Submission title:**  
**MARS-LINK — Crew-Coordinated Delay-Tolerant Mission Operations under Compound Mars Anomalies**

### Scientific question

Under a fixed Mars-like communication delay, do structured onboard procedures and a transparent priority-aware procedure aid reduce critical mission/resource violations compared with Earth-dependent operation when safe action is required before an Earth response can return?

### Experimental modes

- **Mode A:** Earth-dependent operation.
- **Mode B:** structured onboard procedures.
- **Mode C:** deterministic priority-aware procedure aid.

Mode C is rule-based, transparent and advisory. It is not presented as AI/ML and does not autonomously command hardware.

### Communication profile

- 5-minute one-way delay;
- 10-minute round trip.

At least one anomaly in each scenario family requires a safe local decision before the round-trip Earth response can arrive.

### Scenario families

1. resource/energy emergency;
2. communications/relay degradation;
3. systems/mission conflict.

Matched variants are used so the crew does not simply repeat identical scenario scripts.

### Crew

**6 crew members**

1. Mission Commander / Crew Lead;
2. Communications Specialist;
3. Operations / Flight-Control Engineer;
4. Systems / Resource Engineer;
5. Data / Verification Officer;
6. Independent Observer / Evidence Recorder.

### Run structure

- 1 unmeasured training episode;
- 9 measured episodes = 3 operating modes × 3 matched scenario families;
- mode/scenario ordering is pre-declared and counterbalanced rather than fixed A->B->C.

### Duration

Target total: **5 hours 15 minutes** including briefing, training, nine measured episodes, controlled resets, one short break and final evidence/reporting.

### Primary endpoint

**Critical mission/resource constraint violations** — count and, where meaningful, cumulative duration.

Secondary measures:

- mandatory mission-objective completion;
- crew-internal decision time excluding forced communication delay;
- incorrect/unsafe actions;
- message-priority or acknowledgement errors;
- recovery time;
- procedural deviations;
- final mission/resource state.

### Earth-side control and Pakistan–Moscow link

MARS-LINK uses a **hybrid communications architecture**:

- the complete scientific experiment is shipped/provided as an offline/local turnkey package in Moscow;
- IST Pakistan Mission Control may act as the real Earth side over an ordinary terrestrial Internet link;
- the real Internet link is only the transport path;
- the experiment software applies the declared **5-minute one-way Mars delay** before an Earth message becomes available to the crew;
- message content and release timing remain frozen for measured episodes;
- if the Pakistan–Moscow link fails, the local Moscow package generates the same pre-scripted Earth message with the same delay, so the scientific condition does not change.

The measured experiment therefore never depends on live cross-border connectivity.

A separate real-time operations/media path may mirror telemetry to IST and approved nodes for monitoring, analysis and showcase activity. That path must not inject uncontrolled advice into measured episodes.

See [Communications and Turnkey Execution Architecture](COMMUNICATIONS_AND_TURNKEY_ARCHITECTURE.md).

### HIL / physical hardware

Not required for the crew experiment and not part of the scientific completion criteria.

---

## 3. Proposal 2 — TWIN-RESILIENCE v2

**Submission title:**  
**TWIN-RESILIENCE — Calibrated Crew Trust in Digital-Twin-Assisted Remote Asset Operations under Degraded Telemetry**

### Scientific question

When raw telemetry is degraded and the Digital Twin/reference estimate may itself be correct, stale, incomplete or wrong, can the crew calibrate trust correctly and choose the safer operational response?

### Remote asset

A **Mars Surface Communications and Power Relay** is used as the remote mission asset.

The asset has bounded operational state such as:

- battery/energy reserve;
- power generation/load;
- communication-link state;
- thermal/status indicators;
- relay availability;
- command acknowledgement.

### Controlled evidence conditions

1. healthy telemetry + consistent twin/reference;
2. degraded telemetry + accurate/useful twin/reference;
3. degraded telemetry + intentionally stale/wrong twin/reference;
4. unmodelled/ambiguous condition requiring corroboration rather than blind reliance on either source.

The crew is not told which condition is active.

### Crew

**5 crew members**

1. Mission / Operations Lead;
2. Systems Engineer;
3. Communications / Telemetry Specialist;
4. Data / Verification Officer;
5. Independent Observer / Evidence Recorder.

### Run structure

- 1 unmeasured training episode;
- 8 measured episodes = 4 evidence-quality conditions × 2 matched variants;
- concealed deterministic condition assignment;
- post-episode reveal only after crew decision and evidence capture.

### Duration

Target total: **4 hours 45 minutes** including briefing, training, eight measured episodes, resets, one short break and final evidence/reporting.

### Primary endpoint

**Incorrect reliance decisions** — cases in which the crew accepts an erroneous/stale twin estimate over stronger corroborating evidence, or rejects a correct/useful twin indication without justified contrary evidence and takes the unsafe action.

Secondary measures:

- fault-recognition correctness;
- recovery correctness;
- time to recognize telemetry/twin disagreement;
- inappropriate twin reliance;
- corroborating-evidence actions taken;
- mission/resource violations.

### Ground-side visibility and communications

The TWIN-RESILIENCE scientific package remains local/offline-capable in Moscow. IST and approved nodes may receive mirrored telemetry/evidence over a real-time terrestrial link for observation or parallel analysis, but during measured episodes they must not tell the crew whether the raw telemetry or Digital Twin/reference is correct.

Loss of the Pakistan–Moscow link must not stop or alter the experiment.

### HIL / physical hardware

Not required for the crew experiment and not part of the scientific completion criteria. Any later physical-shadow replay on representative hardware is supplementary only.

---

## 4. Shared submission principles

Both proposals use the same submission discipline:

- Partner/institution field: **Institute of Space Technology (IST) / SSTRL / NCGSA, Pakistan**.
- CubeSTEM may be credited factually as the technology/platform contributor in team experience and software description, not as the scientific subject of the experiment.
- Software package is designed to be locally executable/offline for a turnkey crew experiment.
- Live Pakistan–Moscow connectivity is additive: useful for real Ground-Control presence, telemetry mirroring, distributed observation and media, but never a scientific single point of failure.
- The Mars communications delay is imposed deterministically by the experiment software, not by the ordinary Internet transport.
- Crew instructions should be concise and role-specific.
- Results evaluate the experiment/procedure, not individual crew competence.
- Any later research/publication use should de-identify individual performance and follow applicable organizer/institutional consent requirements.
- No proposal claims flight qualification, autonomous Mars control, validated Mars AI, or Mars-qualified hardware.

---

## 5. Out of scope for the current repository baseline

The following are deliberately **not current planning targets here**:

- software development work packages;
- Ground-Lab/node rollout;
- SUPARCO/university outreach;
- sponsorship/media strategy;
- IST minute-sheet revision;
- December Challenge planning;
- TwinLink/HIL implementation;
- AI-Alpha implementation.

Those topics may be planned elsewhere after the two Model Experiment submissions are frozen.


---

## 6. Current institutional status

As of 12 September 2026:

- The two Model Experiment proposals have been prepared and sent to Ms. Lada / the ISG organizers.
- The Vice Chancellor is being kept informed through a short status note rather than a decision-seeking paper.
- International travel and personal participation expenses for Dr. Rehan Mahmood and the travelling students are planned to be borne by the participants themselves; no IST international travel funding is being requested for the delegation.
- Pakistan-side Ground Laboratory / local activity expenditure is intended to be handled from the available SSTRL share within NCGSA, subject to normal institutional procedures.
- A formal extension/revision of the already-approved minute sheet is planned for the next working session; that revision will capture the enlarged IST Ground-Lab / national-node activity and the later larger national follow-on.
- The immediate external-coordination priority is **node partners**, not sponsorship.

The repository remains a source-of-truth repository. It does not become the implementation repository for Digital Twin, TwinLink, Edge, Ground-Lab software or HIL.

---

## 7. Node-partner strategy

The first external outreach should focus on building a small, credible network of technical nodes around IST rather than asking for money.

Priority order:

1. **IST / SSTRL / NCGSA** — national hub and organizer-facing Pakistan interface.
2. **Two strong university operational nodes** — selected for concrete technical capability and committed faculty ownership.
3. **SUPARCO** — approached as a national technical / strategic node for a bounded specialist role.
4. **Additional universities / organizations** — associate or observer nodes feeding the later larger national activity.
5. **Sponsors (Ignite, PARS, corporate partners, etc.)** — approached only after the technical node network and event structure are clear.

Commercially, a successful multi-institution node deployment is valuable future evidence for CubeSTEM MissionLab / Digital Twin adoption. The outreach itself must remain institution-first and technical, not sales-oriented.
