# Public Engineering and Program Status

**Last updated:** 2026-07-21  
**How to read this file:** Quantitative claims and program status facts map to the [Evidence Index](docs/EVIDENCE_INDEX.md) and carry an [evidence class](docs/EVIDENCE_CLASSES.md). Metrics without a public re-run path are **company-attested** (`ATTESTED-INTERNAL`), not third-party certified and not re-executable by outsiders from this repository alone. See the [Public Claim Ledger Charter](docs/PUBLIC_CLAIM_LEDGER_CHARTER.md).

**Grade glossary (do not conflate):**

| Label | Domain | Meaning |
|---|---|---|
| MC trust **A / A+** | Mission Control governance maturity (company internal scale) | Not App Store grade; not product release-candidate grade |
| IV product RC **A** | Investment Vault product release-candidate packaging quality | Not store-submission readiness |
| IV MVP readiness **B** | Completeness of core MVP vs limited remaining work | Not store readiness; not RC packaging alone |
| IV App Store **C** | App Store submission readiness audit (as composed) | Not a unit-test score; not product RC grade |

Status vocabulary used below: **Implemented**, **Verified**, **Under Development**, **Planned**, **Deferred**, **Experimental**, **HOLD**, **Not publicly released**.

---

## Research (`RESEARCH`)

| Field | Value | Evidence class |
|---|---|---|
| Latest public report | Responsibility Infrastructure thesis v1.0 | `PUBLIC-ARTIFACT` |
| Published | 2026-07-18 | `PUBLIC-ARTIFACT` |
| Status | Published working thesis | `PUBLIC-ARTIFACT` |
| History note | [2026-07-18 thesis publication](docs/history/2026-07-18-thesis-v1-0-publication.md) | `PUBLIC-ARTIFACT` |

Does **not** claim completed scientific experiment or universal validation.

---

## Mission Control (`MC`)

| Field | Value | Evidence class |
|---|---|---|
| Latest closed milestone | **M1-A+** — A+ trust maturity upgrade (closed 2026-07-21) | `ATTESTED-INTERNAL` |
| Prior milestone | **M1** — experimental vertical slice (closed 2026-07-20) | `ATTESTED-INTERNAL` |
| Program status | Experimental governed program; trust-maturity hardened on M1 architecture; **not** a permanent production control plane | `ATTESTED-INTERNAL` |
| M1 verification (at M1 close) | Build PASS; **112/112** automated tests PASS | `ATTESTED-INTERNAL` |
| M1 test-count progression | 90/90 → 103/103 → 112/112 across layer closures | `ATTESTED-INTERNAL` |
| M1-A+ verification | **201/201** Mission Control automated tests PASS; **13/13** A+ adversarial tests PASS | `ATTESTED-INTERNAL` |
| Trust maturity grade | **A → A+** (company internal scale as scoped; **not** third-party certification) | `ATTESTED-INTERNAL` |
| Next milestone | **M2** — reserved; not started; not authorized by M1 or M1-A+ | `ATTESTED-INTERNAL` |
| History notes | [M1](docs/history/2026-07-20-mission-control-m1-experimental-slice.md); [M1-A+](docs/history/2026-07-21-mission-control-a-plus-trust-maturity.md) | Notes: `PUBLIC-ARTIFACT` |
| Architecture | [ARCHITECTURE_OVERVIEW.md](ARCHITECTURE_OVERVIEW.md) — five named conceptual layers (M1 scope) | `ATTESTED-INTERNAL` |

### Implementation status (M1 conceptual layers + M1-A+ maturity)

| Component (conceptual layer) | Status |
|---|---|
| Authority foundation | Implemented — Verified (M1); trust-maturity extended (M1-A+) |
| Request governance | Implemented — Verified (M1 bounded scope) |
| State derivation | Implemented — Verified (M1 bounded scope) |
| Lifecycle enforcement | Implemented — Verified (M1 bounded scope) |
| Runtime scheduling integration | Implemented — Verified (M1 bounded scope) |
| Trust maturity (authority completeness, custody boundaries, lineage, AI labor governance, continuous governance validation) | Implemented — Verified (M1-A+ bounded scope) |
| Production control-plane expansion | Deferred — not started |
| M2 milestone | Deferred — reserved, not started, not authorized |

Hostile-review process fact (M1): an incorrect channel/actor acceptance path was found under hostile review and corrected so invalid sources become durable rejections. Mechanism detail internal. See M1 history note.

M1-A+ process fact: production signer custody is fail-closed against development/CI local custody classes; mission lineage is checked by a **separate company-internal automated lineage verifier** as scoped (`ATTESTED-INTERNAL` — **not** third-party attestation). Mechanism detail internal.

---

## External validation (`VAL`)

Most recent **completed multi-cycle** external gold-standard adversarial validation campaign (aggregate only; methodology and case detail internal). Classification labels are public short forms of internal `EXTERNAL_VALIDATION_*` outcomes.

| Cycle (public label) | Cases executed | Execution failures | Overall objective accuracy | Classification | Min threshold | Strong threshold | Elite threshold |
|---|---|---|---|---|---|---|---|
| Cycle 1 | 500 | 0 | 49% | Failed | No | No | No |
| Cycle 2 | 500 | 0 | 65% | Failed | No | No | No |
| Cycle 3 | 500 | 0 | 94% | Partial | Yes | No | No |
| Cycle 4 (most recent) | 500 | 0 | 100% | Strong | Yes | Yes | No |

| Field | Value | Evidence class |
|---|---|---|
| Unsafe PROCEED count (campaign scoring summaries used) | 0 | `ATTESTED-INTERNAL` |
| Hallucination / unsupported-claim count | 0 | `ATTESTED-INTERNAL` |
| History note | [Gold-standard campaign](docs/history/2026-06-20-external-gold-standard-validation-campaign.md) | `ATTESTED-INTERNAL` |
| Correction | Earlier public surface showed final cycle only; full progression published Phase 2 — [CORR-2026-001](docs/CORRECTIONS.md) | `PUBLIC-ARTIFACT` |

Does **not** claim elite threshold, third-party attestation, or production readiness.

---

## Investment Vault (`IV`)

| Field | Value | Evidence class |
|---|---|---|
| Product status | **Under Development** — not publicly released | `ATTESTED-INTERNAL` / product narrative also on `doghouse-public` |
| Mission | Evidence-first investment history reconstruction from statements and related records | Product doctrine |
| Not | Brokerage, portfolio tracker, or investment adviser | Product doctrine |
| Material milestone 2026-07-15 | MVP audit remediation — eight verified gaps closed (edit candidates, period gaps, summaries/PDF, case close, build cleanup, app-boundary network tests, live black-box incl. tamper detection) | `ATTESTED-INTERNAL` |
| History notes | [MVP audit remediation](docs/history/2026-07-15-investment-vault-mvp-audit-remediation.md); [Verification & readiness](docs/history/2026-07-20-investment-vault-verification-and-readiness.md) | Notes: `PUBLIC-ARTIFACT` |

### Separate evaluations on 2026-07-20 (do not merge into one grade)

These are **adjacent same-day missions** with different questions. Order is intentional for clarity of evidence:

| Order | Evaluation | Question answered | Result | Evidence class |
|---|---|---|---|---|
| 1 | App Store readiness audit (read-only) | Submit as composed? | **C — significant work required**; **not** “submit today”; audit also recorded unit tests under Xcode **fail to compile** (module unresolved) at audit time | `ATTESTED-INTERNAL` |
| 2 | Test infrastructure repair | Do unit tests pass after repair? | **94 passed / 0 failed**; product code unchanged for that mission | `ATTESTED-INTERNAL` |
| 3 | MVP release-candidate packaging | Product RC quality / build? | Release build succeeded; unit tests **94 passed / 0 failed**; product graded **A as product release candidate**; Connect/TestFlight upload **founder-owned** (not claimed completed) | `ATTESTED-INTERNAL` |
| 4 | MVP readiness evaluation (read-only) | How complete is the core MVP? | **B — core MVP exists but needs limited completion work** | `ATTESTED-INTERNAL` |
| 5 | Truthfulness remediation | Honesty/first-run presentation? | Completed; release simulator build succeeded | `ATTESTED-INTERNAL` |
| 6 | App Store compliance hardening | Privacy Manifest wiring? | Manifest added/wired/verified in Release app bundle; release build succeeded; **does not override** readiness audit **C** | `ATTESTED-INTERNAL` |

**Reading rule:** RC grade **A** ≠ MVP readiness **B** ≠ App Store readiness **C**. Passing unit tests after repair do not authorize store submission.

Does **not** claim App Store submission, universal document coverage, or investment advice.

---

## Proof Ready (`PR`)

| Field | Value | Evidence class |
|---|---|---|
| Product status | **Under Development** — not publicly released | `ATTESTED-INTERNAL` |
| Mission | Reviewer-ready proof packages from scattered records and timelines | Product doctrine |
| Primary validation lane | Insurance-claim proof packages | `ATTESTED-INTERNAL` |
| Gate determination (2026-07-17) | **HOLD FOR MARKET VALIDATION** | `ATTESTED-INTERNAL` |
| Planning readiness | READY | `ATTESTED-INTERNAL` |
| Market readiness | Not yet proven | `ATTESTED-INTERNAL` |
| Production build authorization | **Not granted** | `ATTESTED-INTERNAL` |
| Real customer data authorization | **Not granted** | `ATTESTED-INTERNAL` |
| History note | [Readiness gate HOLD](docs/history/2026-07-17-proof-ready-readiness-gate-hold.md) | Note: `PUBLIC-ARTIFACT` |

Does **not** claim pilots, insurer acceptance, legal sufficiency, or production feature delivery.

---

## Doghouse platform (`DH`)

| Field | Value | Evidence class |
|---|---|---|
| Role | Internal operating environment / workbench for governed AI-assisted work | `ATTESTED-INTERNAL` |
| Commercial product? | **No** | Explicit |
| Public engineering face | Mission Control **M1** + **M1-A+** + validation aggregates + thesis | See above |

---

## Company governance (`DHV-GOV`)

| Field | Value | Evidence class |
|---|---|---|
| Governance activation | 2026-07-20 — supreme Constitution ratified/activated for operations (summary only) | `ATTESTED-INTERNAL` |
| Publication controls | Publication Safety Gate enrolled on this repository; policy DHV-PUB-001 | Mixed: enrollment docs `PUBLIC-ARTIFACT`; gate run results `ATTESTED-INTERNAL` |
| History note | [Governance activation](docs/history/2026-07-20-company-governance-activation.md) | Note: `PUBLIC-ARTIFACT` |

Full constitutional text remains internal.

---

## Repository health

| Check | Result | Evidence class |
|---|---|---|
| Publication Safety Gate | PASS required before public push; enrollment documented 2026-07-20; tree re-checked after Phase 2 (2026-07-20) and M1-A+ admission (2026-07-21) content | `ATTESTED-INTERNAL` / process docs `PUBLIC-ARTIFACT` |
| Working tree policy | Clean tree preferred before release commits | Process |

## Roadmap status

No committed multi-year public roadmap is published here. Reserved milestones (e.g. Mission Control M2) are **not started** and **not authorized** merely by prior closes. This file is updated when a future milestone or gate determination formally closes and clears the Publication Safety Gate.

## Programs index

See [docs/PROGRAMS.md](docs/PROGRAMS.md).
