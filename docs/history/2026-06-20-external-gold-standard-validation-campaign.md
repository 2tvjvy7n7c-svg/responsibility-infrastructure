# Milestone note: External gold-standard adversarial validation campaign (aggregate)

**Milestone ID:** VAL-EGS-2026-06  
**Program:** External validation (`VAL`)  
**Engineering / event completion date:** 2026-06-20 (multi-cycle campaign day; aggregate scoring records)  
**Public documentation date:** 2026-07-20 (Phase 1 disclosed final-cycle aggregates only; **Phase 2 publishes full multi-cycle progression**)  
**Status:** Historical validation campaign summary  
**Evidence classification:** `ATTESTED-INTERNAL` (aggregates from internal scoring reports; methodology and case packs remain internal)

---

## Why this milestone is recorded

Dog House Ventures ran a multi-cycle **adversarial external gold-standard validation** campaign against a fixed-size case pack. The campaign is meaningful public evidence because it shows **measurement, failure, improvement, and threshold classification** — not a single marketed score.

A skeptical reader should treat these figures as **company-attested aggregates**, not as independently re-runnable science, until methodology and artifacts are deliberately published (they are not published here).

---

## What is disclosed (aggregate only)

Four ordered cycles, each with **500 cases executed** and **0 execution failures**:

| Cycle (public label) | Overall objective accuracy | Classification (public short label for internal `EXTERNAL_VALIDATION_*`) | Minimum-acceptable threshold | Strong-result threshold | Elite-result threshold |
|---|---|---|---|---|---|
| Cycle 1 | 49% (245/500 objective-correct) | Failed | Not met | Not met | Not met |
| Cycle 2 | 65% (325/500 objective-correct) | Failed | Not met | Not met | Not met |
| Cycle 3 | 94% (470/500 objective-correct) | Partial | Met | Not met | Not met |
| Cycle 4 (most recent completed) | 100% (500/500 objective-correct) | Strong | Met | Met | Not met |

Additional aggregate facts reported for the completed cycles:

- **Unsafe PROCEED count:** 0 (across the completed campaign scoring summaries used for these aggregates).  
- **Hallucination / unsupported-claim count:** 0 (same basis).  
- **Elite-result threshold:** not met even on Cycle 4.

Public labels use **Cycle 1–4** only. Internal release-candidate codenames, case IDs, domain-by-domain score tables, trap catalogs, and methodology remain internal by design.

---

## Correction relative to earlier public presentation

An earlier public STATUS / testing-dashboard presentation emphasized the **most recent** cycle (500/500, 100%, strong threshold) without the prior failed and partial cycles. That presentation was incomplete relative to the full campaign record. See [CORRECTIONS.md](../CORRECTIONS.md) entry **CORR-2026-001**.

---

## Non-claims

This note does **not**:

- publish case packs, scoring code, prompts, or methodology,  
- claim independent third-party attestation,  
- claim elite-threshold performance,  
- claim universal domain competence outside the internal objective criteria,  
- or claim that 100% accuracy is a scientific proof of product production readiness.

---

## Supporting evidence

| Kind | Source |
|---|---|
| Public | This note; [STATUS.md](../../STATUS.md); [testing-dashboard/history.json](../../testing-dashboard/history.json); [Evidence Index](../EVIDENCE_INDEX.md) |
| Internal (title only) | External gold-standard validation scoring reports for the four completed cycles; related validation/break reports (not published) |

---

## Document control

| Field | Value |
|---|---|
| Disclosure level | Aggregate campaign summary only |
| Authorizes production claims | No |
