# TWIN-RESILIENCE v2 — Submission Source of Truth

**Final working title:** TWIN-RESILIENCE — Calibrated Crew Trust in Digital-Twin-Assisted Remote Asset Operations under Degraded Telemetry  
**Status:** READY FOR APPENDIX 1 SUBMISSION BASELINE

## 1. Purpose

Test whether a crew can correctly calibrate trust between degraded raw telemetry and a Digital Twin/reference estimate when either information source may be incomplete or misleading.

## 2. Mars asset

The experiment uses a **Mars Surface Communications and Power Relay** as a bounded remote mission asset.

Observable state includes:

- energy reserve;
- power generation/load;
- communication-link health;
- relay availability;
- thermal/status indicators;
- command acknowledgement.

## 3. Hypothesis

Digital-Twin/reference information will improve diagnosis when raw telemetry is degraded **only when the crew appropriately verifies consistency**. When the twin/reference itself is stale or wrong, crews that seek corroborating evidence should make fewer unsafe reliance decisions than crews that follow either source uncritically.

The experiment therefore tests calibrated trust, not simply whether a Digital Twin is useful.

## 4. Controlled evidence conditions

### Condition 1 — nominal agreement
Raw telemetry is healthy and the twin/reference is consistent.

### Condition 2 — degraded telemetry, correct twin
Raw telemetry is degraded; the twin/reference remains accurate/useful.

### Condition 3 — degraded telemetry, wrong/stale twin
Raw telemetry is degraded and the twin/reference is intentionally stale or incorrect.

### Condition 4 — ambiguous/unmodelled case
Neither raw telemetry nor twin/reference alone is sufficient; the crew must obtain corroborating evidence before acting.

The crew is not told which condition is active.

## 5. Crew

Five crew members:

1. Mission / Operations Lead
2. Systems Engineer
3. Communications / Telemetry Specialist
4. Data / Verification Officer
5. Independent Observer / Evidence Recorder

## 6. Run structure

- 20 min briefing;
- 20 min unmeasured training episode;
- 8 measured episodes, approximately 20 min each;
- controlled 5 min reset between measured episodes;
- one 15 min short break;
- 30 min final evidence review/report.

Planned total: **4 h 45 min**.

The eight measured episodes are four evidence-quality conditions × two matched variants. Condition assignment is deterministic but concealed from the crew until after the episode.

## 7. Primary endpoint

**Incorrect reliance decision count**

An incorrect reliance decision is recorded when the crew:

- accepts an erroneous/stale twin estimate over stronger corroborating evidence and takes the unsafe action; or
- rejects a correct/useful twin indication without justified contrary evidence and takes the unsafe action.

The evaluator scoring rule is deterministic and fixed before execution.

## 8. Secondary measures

- fault-recognition correctness;
- recovery correctness;
- time to recognize disagreement;
- inappropriate twin reliance;
- corroborating-evidence actions taken;
- mission/resource violations;
- final relay state.

## 9. Turnkey concept

Crew receives:

- offline/local experiment package;
- preloaded remote-asset scenarios;
- role-specific instructions;
- one training scenario;
- concealed condition assignment;
- evidence/logging package;
- crew report form;
- printed fallback instructions.

## 10. Safety/data boundary

Software-only crew experiment. No hazardous equipment or invasive procedure.

Crew results are reported at crew/episode level for evaluation of the procedure/system. Individual competence is not presented as an experiment outcome.

## 11. HIL boundary

Physical/HIL replay is not required and is not part of the Model Experiment completion criteria. Any later replay on representative cyber-physical hardware is supplementary only.

## 12. Non-claims

The proposal does not claim:

- that the simulated relay is flight-qualified Mars hardware;
- that the Digital Twin is always correct;
- autonomous physical control;
- flight-qualified AI/ML;
- physical/HIL evidence as part of the crew experiment.
