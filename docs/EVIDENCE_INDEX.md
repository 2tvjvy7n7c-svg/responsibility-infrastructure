# Evidence Index

Every factual claim published in this repository resolves to a source on this page. If a claim exists elsewhere in this repository without an entry here, that is a governance defect — open an issue.

Internal sources are cited by title only (per [PUBLICATION.md](../PUBLICATION.md) and [docs/PUBLICATION_SAFETY.md](PUBLICATION_SAFETY.md)); this repository does not publish personal machine paths, in accordance with `DOGHOUSE_PUBLICATION_POLICY.md` (DHV-PUB-001) §6.1.

| Claim | Where published | Evidence source |
|---|---|---|
| Responsibility infrastructure thesis, v1.0, published 2026-07-18 | [README.md](../README.md), [PUBLICATION.md](../PUBLICATION.md) | [articles/ai-responsibility-problem.md](../articles/ai-responsibility-problem.md), [CITATION.cff](../CITATION.cff) |
| M1 is Mission Control's first formal engineering milestone, closed 2026-07-20 | [docs/history/2026-07-20-mission-control-m1-experimental-slice.md](history/2026-07-20-mission-control-m1-experimental-slice.md), [STATUS.md](../STATUS.md) | Internal Doghouse Engineering Milestone Index (title only) |
| M1 verification: build PASS; 112/112 automated tests PASS | [STATUS.md](../STATUS.md), [testing-dashboard/history.json](../testing-dashboard/history.json) | Internal M1 final completion report (title only) |
| M1 conceptual architecture: five named layers (authority foundation, request governance, state derivation, lifecycle enforcement, runtime scheduling integration) | [ARCHITECTURE_OVERVIEW.md](../ARCHITECTURE_OVERVIEW.md) | Internal Doghouse Engineering Milestone Index, M1 entry (title only) |
| M1 test-count progression: 90/90 → 103/103 → 112/112 across layer closures | [testing-dashboard/history.json](../testing-dashboard/history.json) | Internal M1 final completion report and phase series (title only) |
| M2 is reserved, not started, and not authorized by M1's closure | [STATUS.md](../STATUS.md), [ARCHITECTURE_OVERVIEW.md](../ARCHITECTURE_OVERVIEW.md) | Internal Doghouse Engineering Milestone Index §6 "Reserved: M2" (title only) |
| Phase 6 / production control-plane expansion has not started and is explicitly deferred | [STATUS.md](../STATUS.md) | Internal Doghouse Engineering Milestone Index, M1 non-claims table (title only) |
| Most recent external gold-standard adversarial validation cycle: 500 cases executed, 0 execution failures, 100.0% overall objective accuracy | [STATUS.md](../STATUS.md), [testing-dashboard/history.json](../testing-dashboard/history.json) | Internal external gold-standard validation program (title only; case-level detail and methodology remain internal) |
| Publication Safety Gate PASS on current repository content | [STATUS.md](../STATUS.md) | Gate run, 2026-07-20, 23 files scanned, 0 findings — see [docs/PUBLICATION_SAFETY.md](PUBLICATION_SAFETY.md) |

## Maintenance rule

When a new claim is added anywhere in this repository, add a row here in the same change. When a claim is superseded, keep the old row, mark it superseded, and link the correction — do not delete it (Constitution §11: a superseded public claim stays visible, dated, and cross-linked).
