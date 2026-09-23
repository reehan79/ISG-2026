# Implementation Repository Mapping

**Status:** CANONICAL DEVELOPMENT BOUNDARY  
**Updated:** 2026-09-23

This document tells development threads where programme requirements belong. It does not claim that every item is already implemented.

## 1. Programme authority

Repository: `reehan79/ISG-2026`

Owns:
- programme architecture;
- scientific/procedural experiment definitions;
- node/partner model;
- ISG-to-Challenge continuity;
- public claims and message boundaries;
- development requirements;
- decision history.

Does **not** own runtime implementation code.

## 2. Digital Twin / MissionLab

Repository: `reehan79/digital-twin`

Owns the canonical MissionLab/Digital Twin implementation, including the accepted Core / ModelPack / experiment-orchestration / provider / evidence / Programme / Challenge directions already established there.

New ISG/MissionLab work should extend those authorities rather than create a second simulator or a separate ISG platform.

Key development principle:

```text
Experience / Programme / Challenge
        ->
Mission Experiment Runtime
        ->
Experiment / Scenario / FaultCampaign / ExecutionPlan
        ->
provider orchestration
        ->
Core/ModelPacks OR TwinLink
        ->
Evidence / Digital Thread
```

## 3. TwinLink

Repository: `reehan79/cubestem-twinlink`

Owns physical resource/session/command/telemetry transport and physical/hybrid integration.

TwinLink transport faults must not be misused as the MARS-LINK human/mission communications delay model.

## 4. Edge Node

Repository: `reehan79/cubestem-edge-node`

Owns site-edge presence and later physical resource attachment patterns.

A site being online must not by itself imply that a physical resource is available or validated.

## 5. Mission Experiment Runtime requirement

The platform needs a reusable protocol/runtime layer for scientific/mission execution semantics such as:

- crew roles;
- briefing/training/measured episodes;
- counterbalanced assignment;
- blinding/concealment;
- lock-before-reveal;
- observer/evidence record;
- controlled reset;
- protocol deviation;
- local persistence/resume;
- final report/export.

MARS-LINK and TWIN-RESILIENCE should be Experiment Packs on this runtime.

## 6. MARS-LINK implementation rule

MARS-LINK needs a mission communications semantic layer (message queue, one-way delay, release time, priority/deadline/acknowledgement/store-and-forward semantics).

Do not implement its 5-minute Mars delay by abusing TwinLink telemetry-egress delay.

## 7. TWIN-RESILIENCE implementation rule

Maintain separation between authoritative scenario truth, canonical evidence and what the crew is shown.

Do not corrupt canonical measured telemetry and then label it as measured truth.

Observation transforms may create degraded/stale/wrong views for the crew while preserving the underlying truth/evidence lineage.

## 8. Distributed Mission Node implementation rule

Mission Nodes are deployment/participation projections over the existing platform, not independent numerical authorities.

The federation should support durable event/submission exchange, reconnect and provenance while keeping the official Moscow scientific execution independent of WAN availability.

## 9. Challenge reuse rule

The later Challenge should compose accepted MissionLab experiment/scenario/evidence capabilities through Challenge/Programme configuration.

A new Challenge must not mean a new physics engine.

## 10. Implementation-status rule

Before stating that a feature is complete, verify the live implementation repository/branch. This programme repository records requirements and decisions, not current code completion.
