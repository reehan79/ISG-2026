# Thread / Agent Handoff Protocol

**Status:** CANONICAL  
**Updated:** 2026-09-23

This repository is designed so that future ChatGPT threads, coding agents, media work, letter-writing work and programme planning do not independently reinvent the programme.

## Mandatory reading before any derived work

Every new thread/agent should first read:

1. `README.md`
2. `docs/master/PROGRAM_ARCHITECTURE_FREEZE_V0_1.md`
3. `docs/master/AUTHORITY_AND_CLAIMS.md`
4. `docs/STATUS_AND_NEXT_STEPS.md`

Then read the domain-specific source:

- **development:** `docs/technology/IMPLEMENTATION_REPOSITORY_MAPPING.md` plus the relevant ISG experiment documents;
- **letters / partner outreach:** `docs/partnerships/PARTICIPATION_MODELS.md` and `docs/communications/MESSAGE_HOUSE.md`;
- **media / website / social:** `docs/communications/MESSAGE_HOUSE.md` and the claims rules;
- **MissionLab Challenge:** `docs/challenge/ISG_TO_CHALLENGE_CONTINUITY.md`;
- **node design:** `docs/nodes/MISSION_NODE_MODEL.md`;
- **scientific execution:** the three documents under `docs/isg/`.

## Working rule

Do not reconstruct architecture from an individual chat.

Use this repository as the programme source of truth, then verify implementation facts in the implementation repository that owns them.

## When a new decision is made

If a discussion changes one of the following, update this repository before downstream work is treated as authoritative:

- programme scope;
- scientific boundary;
- node class or permission;
- ISG / Challenge commercial relationship;
- public claim;
- implementation ownership;
- partner participation model;
- campaign continuity.

Add a dated decision-history entry explaining what changed and why.

## Conflict rule

A later explicit programme decision can supersede an earlier planning decision, but it must not silently rewrite a frozen scientific submission. If a new programme idea conflicts with the submitted experiment protocol, preserve the submitted protocol and place the new activity outside the measured scientific condition unless formally revised through the appropriate authority.
