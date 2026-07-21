# Testing and Validation Dashboard

`history.json` records **aggregate**, company-verified counts admitted to the public claim ledger.

## Field semantics (required reading)

| `metric_kind` | Meaning of count fields |
|---|---|
| `automated_tests` | Unit/regression suite: `tests_total` / `tests_passing` |
| `gold_standard_cases` | Validation cases: `cases_total` / `cases_objective_correct` (objective-correct), **not** unit tests |
| `qualitative_closeout` | No single numeric suite published for that entry |

Do **not** chart VAL rows as if they were unit-test pass rates without reading `metric_kind`.

## What is and is not included

**Included (when authorized for public disclosure):**

- Aggregate totals for automated tests or gold-standard cases  
- Public cycle labels for validation campaigns (not internal codenames)  
- Program tags (`MC`, `IV`, `VAL`, …)  
- Evidence class (`ATTESTED-INTERNAL` for essentially all numeric rows today)  
- Short public-safe labels  

**Not included:**

- Case-level results, domain breakdowns, calibration methodology  
- Run/RC internal identifiers  
- Coverage percentages not measured for the relevant test kind  
- Re-runnable harnesses or proprietary scoring code  

## How to read numbers

Most rows are **`ATTESTED-INTERNAL`**: Dog House Ventures attests they match internal completion or scoring reports. Outsiders cannot re-run the private suites from this repository alone. See [EVIDENCE_CLASSES.md](../docs/EVIDENCE_CLASSES.md) and the [Evidence Index](../docs/EVIDENCE_INDEX.md).

Gold-standard validation is a **multi-cycle progression** (including failed and partial cycles), not a single final score. See [EGS history note](../docs/history/2026-06-20-external-gold-standard-validation-campaign.md) and [CORR-2026-001](../docs/CORRECTIONS.md).

Entries are added only when a milestone or validation cycle formally closes and clears the Publication Safety Gate — this file is not updated speculatively.
