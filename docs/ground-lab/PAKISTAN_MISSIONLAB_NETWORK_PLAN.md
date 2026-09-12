# Pakistan MissionLab Network / National Ground Laboratory Plan

**Status:** programme architecture baseline  
**Purpose:** organize Pakistan's ISG Ground-Lab participation without diluting IST authority or contaminating measured experiments.

---

## 1. Topology

```text
International Space Games / Host MCC
                |
                |
       Pakistan National Hub
        IST / SSTRL / NCGSA
      Pakistan Mission Control
                |
      CubeSTEM MissionLab layer
                |
   +------------+-------------+
   |            |             |
University A University B  National Technical Node
                              (e.g. SUPARCO)
   |
Associate / Observer Institutions

SQU / international collaborators remain outside the
Pakistan national laboratory unless organizer-approved.
```

---

## 2. Tier 1 — IST national hub

IST remains:

- sole organizer interface;
- sole authoritative Pakistan MCC voice;
- experiment-control authority for Pakistan Ground-Lab participation;
- national evidence archive;
- node accreditation/coordination point;
- media/operations hub;
- failover owner for power/connectivity.

External nodes strengthen IST only if this hierarchy remains explicit.

---

## 3. Tier 2 — operational university nodes

October target: **two serious external operational nodes**, selected by capability and reliability rather than number of logos.

A node should have:

- named faculty owner;
- named backup;
- committed student/technical team;
- written one-page role;
- tested connectivity;
- attendance at a full rehearsal;
- no critical single-point dependency.

Candidate capability assignments:

- communications / SDR / link analysis;
- control systems / ROS / automation;
- independent telemetry analysis;
- experiment evidence verification;
- specialist media/science communication.

---

## 4. SUPARCO / national technical node

SUPARCO can conceptually participate because the Ground-Lab rules allow work at “other organizations” within the participating country.

Preferred bounded roles:

- independent link/telemetry analysis;
- technical observer;
- independent evidence-package validation;
- specialist ground-segment advice outside measured episodes.

Rules:

- no public/organizer-facing “SUPARCO node” claim before written acceptance;
- no sole possession of a required capability;
- no uncontrolled intervention during measured episodes;
- data-sharing boundaries agreed explicitly.

RESOLVE and other organizations may be treated similarly if there is a concrete technical role.

---

## 5. Associate / observer institutions

Additional universities may participate without becoming operational dependencies.

Possible functions:

- receive released telemetry;
- run independent post-episode analysis;
- attend technical briefings;
- support outreach;
- enter the December MissionLab Challenge pipeline.

This enables national scale without live-operational fragility.

---

## 6. SQU / international collaboration

SQU should not be described as part of Pakistan's national Ground Laboratory unless explicitly approved by ISG, because the national-lab requirement is territorial.

Possible October position:

- international academic observer/collaborator;
- zero critical experiment function.

Possible December/future position:

- invited international Challenge node;
- first Gulf MissionLab collaboration/reference path.

---

## 7. Measured-episode firewall

External nodes must not contaminate the experiment.

For measured episodes:

- standardized Earth-message content/timing is frozen;
- IST executes the script;
- nodes may analyse in parallel;
- node advice cannot change crew decisions;
- all messages are logged.

For unmeasured showcase episodes:

- live distributed analysis may be enabled;
- outputs may route through IST;
- media/public dashboard may show safe mission state.

---

## 8. Ground-Lab capability checklist

Provision/verify:

- primary Internet plus independent backup;
- UPS / generator failover;
- computers and required operator workstations;
- ≥50 Mb/s capability as stated by ISG document;
- 3D/circuit tools where needed;
- ROS-capable control environment;
- GNURadio/SDR# communications tooling;
- photo/video capture, processing and publishing;
- access to SSTRL fabrication/bench resources where useful;
- secure evidence/log storage.

Capabilities may be distributed across IST and nodes but the critical operation must degrade safely if a node disappears.

---

## 9. December continuity

October nodes become the seed for December:

- operational nodes -> founding Challenge nodes / qualification sites;
- associates -> participating universities;
- SUPARCO/technical organizations -> jury/advisory/validation roles if agreed;
- experiment-pack infrastructure -> Challenge mission substrate.

The network is therefore not dismantled after ISG.
