# Evidence Classes

**Status:** ACTIVE  
**Last updated:** 2026-07-21  
**Used by:** [EVIDENCE_INDEX.md](EVIDENCE_INDEX.md), [STATUS.md](../STATUS.md), history notes, [testing-dashboard/](../testing-dashboard/)

## Classes

### `PUBLIC-ARTIFACT`

The claim is checkable from materials an external reader can open without company access: files in this repository, git tags/releases, or other public URLs explicitly cited.

**Examples:** thesis PDF text; that a history note exists; release tag `v1.0`; tables whose values are fully contained in public files.

### `ATTESTED-INTERNAL`

Dog House Ventures attests that the claim is true based on named **internal** authoritative records. Those records are cited by **title only** (no personal machine paths, no package dump). Outsiders can evaluate consistency, discipline, and non-claims; they cannot re-run proprietary verification unless additional public artifacts are later published.

**Examples:** automated test counts from internal completion reports; gold-standard cycle aggregates; product readiness grades from internal audits.

### `INDEPENDENTLY-ATTESTED`

A named external party, independent audit, public recompute path, or peer venue supports the claim. Absence of this class is not a defect when no independent attestation exists; inventing the class is forbidden.

**Examples (when they exist):** third-party audit report; customer-visible certification; independently re-run public harness with published inputs.

## Rules

1. Every factual engineering, product, validation, or governance claim published in this repository carries exactly one primary class (a claim may note secondary support).  
2. Perfect or strong metrics without published method remain `ATTESTED-INTERNAL` and must not be framed as independently re-runnable science.  
3. Superseded claims keep their original class, stay visible, and link to the correction ([CORRECTIONS.md](CORRECTIONS.md); Constitution publication standard).  
4. When a claim is upgraded (e.g. from attested to public artifact), keep the prior row and mark it superseded.  
5. “Verify yourselves” in public messaging applies fully only to `PUBLIC-ARTIFACT` (and `INDEPENDENTLY-ATTESTED`) claims. Attested claims ask for evaluation of **attestation quality**, not re-execution of private suites.

## Skeptical-reader guidance

| If you need… | Look at… |
|---|---|
| The argument | Thesis article / PDF |
| What can be checked offline | Rows classed `PUBLIC-ARTIFACT` |
| Company-reported engineering results | Rows classed `ATTESTED-INTERNAL` + history notes |
| Third-party proof | Rows classed `INDEPENDENTLY-ATTESTED` (may be empty) |
| What we refuse to claim | Non-claims sections on STATUS and each history note |
