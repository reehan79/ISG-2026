# MARS-LINK v2 — Submission Source of Truth

**Final working title:** MARS-LINK — Crew-Coordinated Delay-Tolerant Mission Operations under Compound Mars Anomalies  
**Status:** READY FOR APPENDIX 1 SUBMISSION BASELINE

## 1. Purpose

Test whether structured local operating procedures and a transparent priority-aware procedure aid help a Mars crew preserve critical mission/resource safety under time-critical anomalies when Earth guidance cannot arrive before the required decision deadline.

## 2. Hypothesis

Under a 5-minute one-way / 10-minute round-trip Earth-Mars communication delay, time-critical anomalies will produce fewer critical mission/resource constraint violations when the crew uses structured onboard procedures, and may produce still fewer prioritization/omission errors when a deterministic priority-aware procedure aid is available, compared with an Earth-dependent operating mode.

## 3. Operating modes

### Mode A — Earth-dependent operation
Crew follows the supplied Earth-dependent protocol and seeks Earth guidance for non-preauthorized decisions.

### Mode B — structured onboard procedures
Crew acts locally within supplied pre-authorized procedures and limits.

### Mode C — priority-aware procedure aid
Crew uses Mode B plus a deterministic advisory aid that ranks hazards by severity, time-to-threshold, resource impact and reversibility. It never commands hardware automatically.

## 4. Mars communication condition

- One-way delay: 5 minutes.
- Round trip: 10 minutes.
- Scenario design includes decisions that must be made safely before one complete round trip can finish.

The configured link delay is an operating constraint, not a measured finding.

## 5. Scenario families

### R — Resource / energy emergency
Energy reserve declines while a competing mission task consumes power. A safety/resource threshold will be crossed before an Earth answer can return unless the crew takes an allowed local action.

### C — Communications / relay degradation
Acknowledgement/relay degradation and competing messages create a prioritization problem. One message/action is safety-critical.

### S — Systems / mission conflict
A subsystem/resource anomaly occurs together with a distracting non-critical event. Crew must protect the critical resource while preserving as much mission value as possible.

Each family has matched variants so the crew does not repeat identical scripts.

## 6. Crew

Six crew members:

1. Mission Commander / Crew Lead
2. Communications Specialist
3. Operations / Flight-Control Engineer
4. Systems / Resource Engineer
5. Data / Verification Officer
6. Independent Observer / Evidence Recorder

## 7. Run structure

- 20 min briefing;
- 20 min unmeasured training episode;
- 9 measured episodes, approximately 20 min each;
- controlled 5 min reset between measured episodes;
- one 20 min short break;
- 30 min final evidence review/report.

Planned total: **5 h 15 min**.

Mode/scenario assignment is frozen before execution using a counterbalanced sequence; fixed A->B->C order on identical scenarios is not allowed.

## 8. Primary endpoint

**Critical mission/resource constraint violations**

Record count and, where meaningful, cumulative duration for each episode.

## 9. Secondary measures

- mandatory mission-objective completion;
- crew-internal deliberation time, excluding configured link delay;
- unsafe/incorrect actions;
- message-priority/acknowledgement errors;
- recovery time;
- procedure deviations;
- final mission/resource state.

## 10. Earth-message control and live-link architecture

Measured episodes use a frozen deterministic Earth-message script.

Preferred execution:

1. IST Pakistan Mission Control sends the protocol-defined Earth message over the normal Pakistan–Moscow Internet path.
2. The real network delivers that message as ordinary terrestrial traffic.
3. The Moscow experiment package places the message into the experiment queue and enforces the declared **5-minute one-way Mars delay**.
4. The crew sees the message only when the simulated Mars delay expires.
5. Crew acknowledgements/responses are handled through the same controlled experiment timing model.

The real Internet path is therefore **transport**, not the source of the Mars delay.

### Local scientific fallback

If the Pakistan–Moscow link is unavailable, the local Moscow package generates the **same frozen Earth message, at the same protocol time, with the same 5-minute delay**.

Therefore:

- live IST participation is desirable but not required for scientific completion;
- link failure does not change the measured condition;
- the experiment remains fully executable offline.

### Real-time monitoring path

A separate real-time path may mirror telemetry, run status and evidence to IST and approved observers/nodes. This path may support monitoring, analysis, video/media and an unmeasured showcase episode, but it must not introduce uncontrolled advice into measured crew decisions.

## 11. Turnkey concept

Crew receives:

- offline/local experiment package;
- role-specific instructions;
- one training scenario;
- preloaded matched scenarios;
- automated run logging;
- crew report form;
- evidence export;
- printed fallback instructions;
- local Earth-message fallback capable of reproducing the frozen IST script without Internet connectivity.

## 12. Safety/data boundary

Software-only crew experiment. No hazardous equipment or invasive procedure.

Crew results are reported at crew/episode level for evaluation of the procedure/system. Individual competence is not presented as an experiment outcome.

## 13. Non-claims

The proposal does not claim:

- autonomous Mars-habitat control;
- validated Mars AI;
- flight-qualified software;
- physical/HIL evidence as part of the crew experiment.
