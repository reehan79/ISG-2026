# MissionLab Network 2026 — Programme Architecture Freeze v0.1

**Status:** FROZEN PROGRAMME ARCHITECTURE  
**Date:** 2026-09-23  
**Change rule:** branding, pricing and participant counts may evolve; the architectural boundaries below require an explicit decision update in this repository.

## 1. Umbrella

The programme is framed as:

**MissionLab Network 2026**  
*ISG 2026 International Mission Campaign -> MissionLab Challenge -> Remote KidSat Missions*

IST/SSTRL is the mission/programme hub for the Pakistan activity. CubeSTEM MissionLab is the enabling Digital Twin / TwinLink technology platform.

MARS-LINK and TWIN-RESILIENCE remain scientifically distinct experiments inside the ISG campaign. They are not the umbrella programme.

## 2. Three connected campaigns, one platform

The programme is a continuous journey rather than three disconnected products:

```text
MissionLab Network 2026
        |
        +-- ISG 2026 International Mission Campaign
        |      +-- MARS-LINK
        |      +-- TWIN-RESILIENCE
        |      +-- IST Ground Support / distributed node activity
        |
        +-- MissionLab Challenge
        |      +-- Digital Twin missions
        |      +-- team evidence / evaluation / competition
        |
        +-- Remote Mission Programme
               +-- TwinLink
               +-- KidSat / HIL where approved and available
               +-- future institutional MissionLab use
```

The same institutional identity, node concept, mission/evidence model and platform should survive across campaigns.

## 3. Node is not Team and Team is not Registration

A **Mission Node** represents an institution/site participation identity.

A **Team** represents a group of participants operating under a node for a campaign.

A **Registration** is a commercial/administrative enrollment into a specific programme such as the MissionLab Challenge.

Therefore one institution may retain one Mission Node across multiple campaigns while hosting several teams over time.

## 4. Persistent Mission Node identity

A node established for the ISG-linked activity should not be discarded after October/November.

Example:

```text
University Mission Node
      |
      +-- ISG 2026 campaign
      +-- MissionLab Challenge 2026
      +-- Remote KidSat campaign
      +-- future MissionLab programmes
```

This persistence is central to the long-term Digital Twin / MissionLab value proposition.

## 5. ISG scientific core remains protected

The official MARS-LINK and TWIN-RESILIENCE scientific execution remains:

- independently executable in Moscow;
- offline/local capable;
- independent of Pakistan-Moscow Internet for scientific completion;
- insulated from uncontrolled node advice;
- auditable through frozen experiment conditions and evidence.

Distributed nodes are **additive**. They must not become a scientific single point of failure.

## 6. Two distributed participation layers during ISG

### Core Operational Nodes

A small number of strongly owned technical nodes may have bounded operational roles such as communications analysis, telemetry analysis, evidence validation or mission planning.

### Participant Mission Nodes

A larger set of universities/schools may participate through approved projections of mission state, telemetry, messages, parallel analysis, released evidence and unmeasured activities.

Participant nodes must not receive hidden scientific truth or an ability to contaminate measured episodes.

## 7. Participation classes

The programme uses the following institutional classes:

- **Mission Hub** — IST/SSTRL; central coordination, Pakistan Ground Support and programme integration.
- **Operational Mission Node** — selected Pakistani universities with defined technical responsibility.
- **Participant Mission Node** — schools/universities participating in the broader MissionLab journey.
- **National Technical / Strategic Node** — national technical organizations such as SUPARCO when formally involved.
- **International Collaborator Node** — foreign institutions such as KFUPM or SQU when formally involved.

International Collaborator Nodes are not described as part of the Pakistan national Ground Laboratory unless the ISG organizer explicitly approves such a status.

A sponsor is not automatically a Mission Node; sponsorship and technical participation are separate concepts.

## 8. Commercial boundary

There is **no programme fee for ISG participation**.

The MissionLab Challenge is a separate fee-bearing programme. Challenge registration may open before ISG and may include:

- early MissionLab platform access;
- institutional Mission Node activation;
- participant/team account activation;
- orientation and training missions;
- selected ISG-linked distributed mission exposure;
- subsequent Challenge missions, evidence and evaluation;
- later remote KidSat access where the final programme includes it.

This must never be described as selling official ISG participation or official ISG registration.

Exact registration fee, team size, institutional quotas and commercial terms remain TBD until separately approved.

## 9. Product / technology continuity

The implementation should preserve the same high-level entities:

```text
Institution
  -> Mission Node
     -> Team / Participant
        -> Campaign Enrollment
           -> Mission / Experiment
              -> Execution
                 -> Evidence / Report
```

The execution provider may evolve:

```text
simulation -> replay -> hybrid -> remote hardware / HIL
```

The platform should not be rebuilt for each stage.

## 10. MARS-LINK and TWIN-RESILIENCE as reusable experiment packs

MARS-LINK and TWIN-RESILIENCE should be implemented as reusable Experiment Packs on the common MissionLab experiment runtime, not as one-off pages or separate engines.

MARS-LINK contributes reusable delayed/disrupted mission-communications semantics.

TWIN-RESILIENCE contributes reusable telemetry/reference disagreement, evidence-quality and calibrated-trust semantics.

## 11. Future KidSat relationship

KidSat/TwinLink is not required for the official ISG scientific result.

Later MissionLab Challenge or institutional missions may bind an accepted experiment to a physical TwinLink resource. The scientific/educational identity should remain stable while the execution provider changes from simulation to physical/hybrid.

## 12. Strategic outcome

The intended long-term path is:

```text
ISG international credibility
        ->
distributed Mission Node experience
        ->
MissionLab Challenge
        ->
remote KidSat / HIL
        ->
permanent institutional MissionLab adoption
```

The programme therefore creates both a meaningful educational/engineering activity and a credible multi-institution reference deployment for CubeSTEM MissionLab / Digital Twin / TwinLink.
