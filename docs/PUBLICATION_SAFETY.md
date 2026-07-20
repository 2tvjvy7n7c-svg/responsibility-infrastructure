# Publication Safety Gate

This repository is enrolled in the Doghouse **Publication Safety Gate**
(control **DHV-PUB-GATE-001**).

## Policy

Canonical company policy (internal business filesystem; titles only in public trees):

- `DOGHOUSE_PUBLICATION_POLICY.md` (DHV-PUB-001)
- `DOGHOUSE_PUBLICATION_SAFETY_GATE_SPECIFICATION.md` (DHV-PUB-GATE-001)
- `DOGHOUSE_PUBLICATION_DETECTION_RULE_CATALOG.md` (DHV-PUB-RULES-001)

Location (conceptual company path, not a personal machine path):

`DOG HOUSE VENTURES LLC/09_OPERATIONS/Policies and Procedures/STANDARDS/`

## Executable package

Engineering package (conceptual OS path):

`DOG_HOUSE_SYSTEM/Development/DOGHOUSE_PUBLICATION_SAFETY_GATE/`

Git hooks installed in this repository invoke that package. Hooks themselves
are local (`.git/hooks`) and are not published content.

## Enforcement

- `pre-commit` — scans staged files (fail closed)
- `pre-push` — scans commits being pushed (fail closed)

## Manual run

From a machine that has the Doghouse engineering tree:

```bash
export PYTHONPATH="$DOG_HOUSE_SYSTEM/Development/DOGHOUSE_PUBLICATION_SAFETY_GATE/src"
# where DOG_HOUSE_SYSTEM is your local path to the Doghouse OS root
python3 -m doghouse_publication_safety_gate staged --repo .
python3 -m doghouse_publication_safety_gate tree --repo .
```

## On FAIL

Fix every finding in the violation report. Re-run until PASS.

Do **not** use `--no-verify` for public publication. Safety Gate PASS is
necessary but not sufficient: governance approval and evidence requirements
still apply (policy §7).
