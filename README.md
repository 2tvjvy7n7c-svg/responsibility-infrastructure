# Responsibility Infrastructure

![The Responsibility Layer](assets/responsibility-layer-cover.png)

## AI Does Not Have an Intelligence Problem. It Has a Responsibility Problem.

*Notes from an ongoing experiment in governing AI-assisted work*

**By Douglas P. Galullo**  
Founder, Dog House Ventures LLC

---

## What this repository is

This repository is Dog House Ventures LLC’s **public claim ledger**: the permanent public home for (1) published research, (2) high-level engineering, product, validation, and governance milestones that materially support public claims, (3) program status with explicit non-claims, and (4) a claim→evidence map with explicit **evidence classes**.

**Philosophy:** Don’t ask people to trust us. Give them enough structure and evidence that they can evaluate our claims — including where verification stops at company attestation and where artifacts are public.

See the [Public Claim Ledger Charter](docs/PUBLIC_CLAIM_LEDGER_CHARTER.md).

### What this repository is not

- Product source code or private development monorepos  
- The internal constitution stack or business-record filesystem  
- A marketing site  
- A promise that proprietary tests are independently re-runnable unless a claim is classed `PUBLIC-ARTIFACT` or `INDEPENDENTLY-ATTESTED`

### Start here by role

| If you are… | Start with… |
|---|---|
| Reading the argument | [Full article](articles/ai-responsibility-problem.md) · [PDF](pdf/galullo-ai-responsibility-problem.pdf) |
| Evaluating engineering / product claims | [STATUS.md](STATUS.md) · [history notes](docs/history/README.md) · [Evidence Index](docs/EVIDENCE_INDEX.md) |
| Checking how evidence is classed | [Evidence classes](docs/EVIDENCE_CLASSES.md) · [Corrections](docs/CORRECTIONS.md) |
| Understanding programs / products | [Programs](docs/PROGRAMS.md) |
| Citing the thesis | [CITATION.cff](CITATION.cff) · [PUBLICATION.md](PUBLICATION.md) |

Maintainer preflight files (`AI_START_HERE.md`, `AGENTS.md`, `CLAUDE.md`) are for authorized maintainers; they are not part of the public argument.

---

## Abstract

This article argues that artificial intelligence's central challenge is not capability, but responsibility. The argument emerged from an ongoing applied study of AI-assisted work in which multiple systems were used for real operational tasks and the surrounding process was repeatedly observed, tested, and refined.

Recurring failures - lost context, evidence detached from conclusions, ambiguous approvals, and authority without clear limits - revealed a common gap. Conventional activity logs can show that something happened, but not that it was properly authorized, supported, reviewed, or accepted.

The resulting hypothesis is that consequential AI-assisted work requires **responsibility infrastructure**: bounded authority, preserved evidence, meaningful review, adaptive procedures, institutional memory, and identifiable human accountability.

> Authority enters through a mandate. Evidence and decisions persist through a governed record. Responsibility exits through explicit acceptance.

The work remains an ongoing experiment, but the hypothesis has held through each iteration so far: AI will not become governable simply by becoming more intelligent. Responsibility must be built into the process itself.

## Read the work

- [Full article](articles/ai-responsibility-problem.md)
- [Abstract](ABSTRACT.md)
- [Publication PDF](pdf/galullo-ai-responsibility-problem.pdf)
- [Publication record](PUBLICATION.md)
- [Author background](AUTHOR.md)
- [Citation metadata](CITATION.cff)
- [Version history](CHANGELOG.md)
- [Thesis publication milestone](docs/history/2026-07-18-thesis-v1-0-publication.md)

## Central thesis

As artificial intelligence becomes more deeply involved in consequential work, increased capability alone is insufficient.

The surrounding process must be able to establish:

- who authorized the work,
- what authority an AI system received,
- what evidence supported its output,
- which limitations were known,
- where the work was reviewed or challenged,
- how procedures changed,
- who approved the resulting decision,
- and who accepted responsibility for the consequence.

The distinction at the center of this work is the difference between an **activity record** and a **responsibility record**.

An activity record may show that something happened.

A responsibility record must also show that the work was authorized, evidenced, reviewed, decided, and accepted.

## Research status

This repository contains an original working thesis developed through an ongoing applied process study.

It does not claim:

- a completed scientific experiment,
- universal validation across industries,
- a final model of AI governance,
- or a substitute for law, regulation, professional standards, or institutional judgment.

The work is published so the argument, its development, and its revisions can be examined over time.

## Public engineering and program status

For multi-program status — Mission Control, external validation, Investment Vault, Proof Ready, Doghouse, and governance — see **[STATUS.md](STATUS.md)**.

Highlights (all non-public-artifact metrics are **company-attested** unless noted):

| Program | Public posture |
|---|---|
| **Research** | Thesis v1.0 published 2026-07-18 |
| **Mission Control** | **M1** closed 2026-07-20 (**112/112** at close); **M1-A+** trust maturity closed 2026-07-21 (**201/201** + **13/13** adversarial); not a production control plane |
| **External validation** | Gold-standard multi-cycle campaign: **49% → 65% → 94% → 100%** on 500-case cycles; final **Strong**, not Elite (`ATTESTED-INTERNAL`) |
| **Investment Vault** | In development; MVP audit remediation 2026-07-15; 2026-07-20 **separate** evaluations (App Store **C** / tests later **94/94** / product RC **A** / MVP readiness **B** — not one grade) |
| **Proof Ready** | In development; **HOLD FOR MARKET VALIDATION** — production build not authorized |
| **Governance** | Constitution activation 2026-07-20 (summary); Publication Safety Gate enrolled |

Mission Control conceptual layers (named only): [ARCHITECTURE_OVERVIEW.md](ARCHITECTURE_OVERVIEW.md).

Quantitative claims and program status facts in [STATUS.md](STATUS.md) and the engineering/product highlights below resolve to the [Evidence Index](docs/EVIDENCE_INDEX.md). Thesis narrative is evidenced by the article/PDF themselves.

### Public history (not thesis revisions)

Ordered by **engineering / event date** (public documentation date may be later; see each note).

| Event date | Note |
|---|---|
| 2026-06-20 | [External gold-standard validation campaign](docs/history/2026-06-20-external-gold-standard-validation-campaign.md) (public doc 2026-07-20) |
| 2026-07-15 | [Investment Vault MVP audit remediation](docs/history/2026-07-15-investment-vault-mvp-audit-remediation.md) |
| 2026-07-17 | [Proof Ready readiness gate HOLD](docs/history/2026-07-17-proof-ready-readiness-gate-hold.md) |
| 2026-07-18 | [Thesis v1.0 publication](docs/history/2026-07-18-thesis-v1-0-publication.md) |
| 2026-07-20 | [Mission Control M1](docs/history/2026-07-20-mission-control-m1-experimental-slice.md) |
| 2026-07-20 | [Company governance activation](docs/history/2026-07-20-company-governance-activation.md) |
| 2026-07-20 | [Investment Vault verification & readiness](docs/history/2026-07-20-investment-vault-verification-and-readiness.md) (separate evaluations; not one merged grade) |
| 2026-07-21 | [Mission Control M1-A+ trust maturity](docs/history/2026-07-21-mission-control-a-plus-trust-maturity.md) |

Full index: [docs/history/README.md](docs/history/README.md).

## Repository contents

- `articles/` — canonical Markdown article  
- `pdf/` — publication PDF  
- `assets/` — cover artwork  
- `research/` — sourcing agenda and future-paper scope  
- `releases/` — fixed release notes  
- `docs/PUBLIC_CLAIM_LEDGER_CHARTER.md` — repository identity and admission standard  
- `docs/EVIDENCE_CLASSES.md` — public / attested / independent evidence classes  
- `docs/EVIDENCE_INDEX.md` — claim-to-source mapping  
- `docs/PROGRAMS.md` — program register  
- `docs/CORRECTIONS.md` — corrections and supersessions  
- `docs/history/` — public milestone notes  
- `docs/PUBLICATION_SAFETY.md` — Publication Safety Gate enrollment  
- `testing-dashboard/` — aggregate test and validation counts (see field semantics in its README)  
- `STATUS.md` — multi-program public status  
- `ARCHITECTURE_OVERVIEW.md` — Mission Control conceptual layers only  
- `SECURITY.md` — security contact and repository scope  
- `CITATION.cff` — citation metadata  
- `PUBLICATION.md` — authorship and publication record  
- `CHANGELOG.md` — version / ledger history  

## Public surface map

| Surface | Role |
|---|---|
| **This repository** | Authoritative **public claim ledger** (research + engineering/product/governance record + evidence map) |
| [`doghouse-public`](https://github.com/2tvjvy7n7c-svg/doghouse-public) | Company front door / high-level product narrative |
| [`doghouse-governed-ai-evaluations`](https://github.com/2tvjvy7n7c-svg/doghouse-governed-ai-evaluations) | Evaluation protocols/results when published; plan-only material is not completed evidence |
| Internal business filesystem | Constitutions, operational standards, legal/financial records (not this repo) |
| Internal engineering OS | Implementation, audits, completion packages (not this repo) |

## Relationship to Dog House Ventures governance

Internal Dog House Ventures governance (Constitution, AI Control Constitution, File Structure Constitution, operational standards) lives in the company business filesystem — separate from this public tree. As of 2026-07-20 that internal stack is treated as activated for operations; this repository remains the **public claim ledger**, not the operating control system. See [governance activation note](docs/history/2026-07-20-company-governance-activation.md).

Products (Doghouse as internal platform, Investment Vault, Proof Ready, and others) inherit internal governance rather than replacing it.

This publication discloses thesis, process, results, and high-level milestones. It does not disclose proprietary implementation (source code, prompts, schemas, lock models, or security design).

## Version

- Thesis version: 1.0  
- Initial public research record: July 18, 2026  
- Public claim ledger framing (Phase 2): July 20, 2026  
- Mission Control M1-A+ public admission: July 21, 2026  
- Author: Douglas P. Galullo  
- Affiliation: Founder, Dog House Ventures LLC  

## Suggested citation

> Galullo, Douglas P. "AI Does Not Have an Intelligence Problem. It Has a Responsibility Problem." Version 1.0, July 18, 2026.

## Feedback

Substantive criticism, corrections, counterarguments, and relevant sources are welcome through GitHub Issues or Discussions.

Feedback should address the argument and public claims rather than speculate about proprietary implementation details.

## Rights

Copyright © 2026 Douglas P. Galullo. All rights reserved.

No open-source or Creative Commons license is granted for the article, abstract, cover image, or associated publication materials. See [LICENSE.md](LICENSE.md) and [NOTICE.md](NOTICE.md).
