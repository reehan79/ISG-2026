# TWIN-RESILIENCE v2 Alternate Experiment Plan

**Working title:** Calibrated Crew Trust in Digital-Twin-Assisted Remote Asset Operations under Degraded Telemetry  
**Status:** HOLD / MODIFY BEFORE SUBMISSION  
**Role in programme:** distinct alternate/secondary proposal; strongest concepts may also inform MARS-LINK fault design

---

## 1. Why v1 was not sufficient

The earlier question — “does a Digital Twin help diagnose degraded telemetry?” — risks becoming a technology demonstration with a largely predetermined answer.

The v2 experiment must test a genuinely uncertain question: **can the crew know when not to trust the twin/reference estimate?**

---

## 2. Scientific question

When raw telemetry is degraded and the Digital Twin/reference estimate may itself be inaccurate, stale or incomplete, can the crew calibrate trust correctly and select the safer operational response?

---

## 3. Experimental contrast

Conditions should include matched cases where:

1. raw telemetry is healthy and twin reference is consistent;
2. raw telemetry is degraded and twin reference is correct/useful;
3. raw telemetry is degraded and twin reference is intentionally stale or wrong;
4. an unmodelled condition makes both the raw signal and twin reference individually insufficient.

The crew must inspect evidence, identify disagreement, seek corroboration and make a bounded operational decision.

---

## 4. Candidate remote asset

The final proposal must name one concrete Mars-relevant remote asset.

Preferred working concept:

**remote Mars communications / power relay asset**

Rationale:

- directly relevant to settlement operations and fault-tolerant communications;
- supports power, link, thermal/status and availability telemetry;
- naturally allows degraded telemetry and model-reference mismatch;
- keeps the optional KidSat replay clearly representative rather than pretending KidSat is Mars hardware.

The exact asset must be frozen before any submission.

---

## 5. Primary endpoint

Candidate primary endpoint:

**incorrect reliance decision count**

An incorrect reliance decision occurs when the crew:

- accepts an erroneous/stale twin estimate over stronger corroborating evidence; or
- rejects a correct/useful twin indication without justified contrary evidence and takes the unsafe action.

The exact scoring rule must be deterministic and inspectable.

Secondary evidence may include:

- fault-recognition correctness;
- recovery correctness;
- time to recognize disagreement;
- inappropriate automation/twin reliance;
- mission/resource violations;
- corroborating-evidence actions taken.

---

## 6. Crew roles

Nominal engineering configuration:

- Mission/Operations Lead;
- Systems Engineer;
- Communications/Telemetry Specialist;
- Data/Verification Officer;
- optional Independent Observer/Evidence Recorder.

No role is allowed to become an uncontrolled source of hints about which episodes contain a wrong twin.

---

## 7. Turnkey and blinding requirement

The crew must not know in advance whether the twin is correct in a given episode.

The experiment package therefore needs:

- deterministic but concealed episode assignment;
- scenario variants of matched difficulty;
- explicit evidence sources available to the crew;
- frozen “ground truth” known to the experiment package/evaluator;
- post-episode reveal and evidence export.

---

## 8. HIL boundary

The optional KidSat/TwinLink activity is **not part of the scientific claim**.

If used:

- one scenario is replayed locally at IST;
- KidSat is labelled a representative cyber-physical mission asset;
- same experiment/scenario/evidence identity is preserved;
- evidence is used to show simulation-to-physical continuity only.

---

## 9. Submission gate

Submit TWIN-RESILIENCE only if all are true:

- organizer welcomes more than one Pakistan/IST proposal;
- v2 is demonstrably distinct from MARS-LINK;
- concrete asset is frozen;
- misleading/stale-twin conditions are implemented;
- turnkey package can be delivered without competing dangerously with MARS-LINK build effort.

Otherwise keep it as the alternate for the review discussion and later Challenge.
