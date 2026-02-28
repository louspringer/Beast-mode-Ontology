# Issue #5: A2A edge transport + AgentCard

## Intent

Add an interoperability transport (A2A channel) alongside existing messaging, and introduce an AgentCard-style projection for semantic discovery/matching, with SHACL validation of A2A readiness.

## Context

As Beast Mode expands into multi-agent interoperability, agents need a standard way to advertise endpoints/identity and validate “ready-to-talk” constraints. This work adds an A2A transport abstraction and a discovery projection model aligned with that goal.

## What Changed (Implementation Summary)

Implemented in commit:

`fb7717d7ac3da3c035623f7f133e2ac8b2d680d6`

This commit introduces:

- A2A transport channel modeling (`beast:A2AChannel`)
- AgentCard projection and A2A skill constructs for discovery/matching
- SHACL shapes validating A2A readiness (e.g., endpoint URL, agent card URL, identity fields)
- Example agent exposed via A2A

## Primary Review Cues (Fast Skim)

Please review commit:

`fb7717d7ac3da3c035623f7f133e2ac8b2d680d6`

Focus areas:

- Ontology additions for A2A transport + AgentCard projection
- SHACL validation shapes for required fields
- Example TTL demonstrating the A2A surface

## Implementation Anchor

Primary commit implementing this work:

- fb7717d7ac3da3c035623f7f133e2ac8b2d680d6  
  "Title: Add A2A edge transport channel + AgentCard projection + SHACL"

## Traceability Map

| Concept                          | Commit                                       |
|----------------------------------|----------------------------------------------|
| A2A transport channel model      | fb7717d7ac3da3c035623f7f133e2ac8b2d680d6     |
| AgentCard projection + A2A skill | fb7717d7ac3da3c035623f7f133e2ac8b2d680d6     |
| SHACL A2A readiness validation   | fb7717d7ac3da3c035623f7f133e2ac8b2d680d6     |
| Example A2A agent                | fb7717d7ac3da3c035623f7f133e2ac8b2d680d6     |

This document links the conceptual Issue directly to its immutable implementation commit.