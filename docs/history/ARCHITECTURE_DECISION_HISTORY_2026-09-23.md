# Architecture Decision History — 22–23 September 2026

**Purpose:** preserve the reasoning that moved the programme from a two-experiment source-of-truth repository to a unified ISG / MissionLab / distributed-node programme source of truth.

This is a structured decision history, not a verbatim chat transcript.

## 1. Starting point

The repository had been intentionally narrowed on 12 September to two scientific Model Experiments: MARS-LINK and TWIN-RESILIENCE.

That was appropriate for submission discipline, but it no longer represented the wider programme that emerged around:

- IST Ground Support;
- distributed university/school nodes;
- the later MissionLab Challenge;
- CubeSTEM MissionLab / Digital Twin / TwinLink continuity;
- potential international collaborator nodes;
- partner, sponsor and media communication.

## 2. Technical architecture review

The Digital Twin, MissionLab and TwinLink architecture was reviewed before broadening the programme.

The central conclusion was that ISG should not create a second simulator or a one-off product.

The accepted direction is to reuse the existing MissionLab engineering authorities and add only the missing reusable programme/runtime concepts, especially:

- scientific/mission Experiment Runtime;
- MARS mission-message semantics;
- TWIN observation/truth separation;
- Mission Node federation;
- offline field hardening;
- Challenge/Programme projection.

MARS-LINK and TWIN-RESILIENCE become reusable Experiment Packs rather than hard-coded applications.

## 3. Distributed-node decision

The node model was expanded from a small Ground-Lab support concept into a persistent institutional Mission Node.

A node should survive across:

- ISG 2026;
- MissionLab Challenge;
- remote KidSat missions;
- future institutional MissionLab use.

This enables the international event to become a genuine first deployment of the later platform rather than a disconnected showcase.

## 4. Scientific protection decision

The official ISG experiments remain independent of the distributed network.

Nodes may observe approved projections, perform parallel analysis and join unmeasured/showcase activities, but cannot contaminate measured scientific episodes or become necessary for completion.

## 5. Commercial decision

No fee will be charged for ISG participation.

The later MissionLab Challenge is a separate fee-bearing programme.

The important commercial refinement is that Challenge registration may open before ISG. Registered teams can receive MissionLab access, Mission Node activation, training missions and selected ISG-linked distributed mission exposure before progressing into the Challenge.

Thus the international event becomes an acquisition/activation milestone without selling ISG status.

## 6. Participation-class decision

A single "node" category was considered too weak for organizations with different relationships.

The programme therefore distinguishes:

- Mission Hub;
- Operational Mission Node;
- Participant Mission Node;
- National Technical / Strategic Node;
- International Collaborator Node.

A sponsor is a separate relationship.

## 7. National-organization decision

National organizations such as SUPARCO should not be asked for a registration fee.

They should be invited into a bounded National Technical / Strategic Node role. Financial support, if appropriate, is a separate conversation from node status.

## 8. International-collaborator decision

Institutions such as KFUPM or SQU may be invited as International Collaborator Nodes.

They should not be described as part of the Pakistan national Ground Laboratory unless the organizer explicitly authorizes that status.

The long-term value is that an institution can first experience MissionLab through a distributed international activity and later progress into a permanent institutional deployment.

## 9. Challenge / KidSat continuity decision

ISG software, Challenge software and KidSat software should not be developed as three separate products.

The same institution/node/team/campaign/mission/evidence architecture should continue across them.

Physical KidSat/TwinLink becomes a later provider/resource binding, not a replacement product.

## 10. Repository-scope decision

The earlier decision that ISG-2026 should contain only the two experiment submissions is now intentionally superseded.

The repository remains **source of truth only**, but its source-of-truth scope is broader:

- scientific experiments;
- Ground Support/node programme;
- Challenge continuity;
- participation models;
- communication claims;
- implementation requirements;
- decision history.

Implementation code remains in the technical repositories.

## 11. Rejected or explicitly avoided approaches

The programme should not:

- charge an ISG participation/registration fee;
- hard-code a MARS-LINK-only web page as the architecture;
- use TwinLink telemetry delay as the Mars communications model;
- create a separate Digital Twin authority at every university;
- mutate canonical measured evidence to simulate an incorrect twin;
- rebuild the product for the December Challenge;
- represent foreign collaborator nodes as Pakistan Ground-Lab nodes without organizer approval;
- make distributed connectivity necessary for the Moscow scientific result.

## 12. Result

The frozen programme architecture is now:

**MissionLab Network 2026 — ISG 2026 International Mission Campaign -> MissionLab Challenge -> Remote KidSat Missions**

This repository is the common context that future development, media, website, letter-writing, sponsor and outreach threads must follow.
