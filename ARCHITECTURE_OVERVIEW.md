# Mission Control — Conceptual Architecture Overview

**Status:** Describes the bounded experimental scope closed at milestone **M1** (2026-07-20). Does not describe a production control plane. Implementation detail — source layout, lock mechanisms, schemas, security design — is intentionally not disclosed here. See [PUBLICATION.md](PUBLICATION.md) and [docs/PUBLICATION_SAFETY.md](docs/PUBLICATION_SAFETY.md).

## What this page is

Mission Control is Dog House Ventures' internal applied-engineering program on governed AI-assisted request handling — authority, durable evidence, and reviewable rejection under real process constraints. This page names the conceptual layers verified as part of milestone **M1**, at a level that lets a reader evaluate the architecture's shape without exposing how it is built.

## Conceptual layers (M1 scope)

1. **Authority foundation** — establishes bounded authority for a request before any downstream action is possible.
2. **Request governance** — governs how an incoming request is admitted, rejected, or escalated.
3. **State derivation** — derives current system state from a durable, evidence-based record rather than mutable in-memory state alone.
4. **Lifecycle enforcement** — enforces which state transitions are valid for a given request or mission.
5. **Runtime scheduling integration** — coordinates multiple in-flight missions under a supervising schedule.

These layers were closed, verified, and audited as bounded experimental work under milestone M1. An orchestration layer above these remains the decision engine and is outside M1's closed scope.

## What this is not

- Not a description of source layout, module boundaries, or file structure.
- Not a description of lock mechanisms, schemas, or security design.
- Not a claim of a permanent, production-grade control plane. Expansion beyond M1 (a reserved future milestone) has not started and is not authorized by M1's closure.

## Source

Layer names and scope are drawn from the internal Doghouse Engineering Milestone Index entry for M1. Full technical detail remains internal. See the [Evidence Index](docs/EVIDENCE_INDEX.md) and the [M1 milestone note](docs/history/2026-07-20-mission-control-m1-experimental-slice.md).
