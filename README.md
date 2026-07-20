# Responsibility Infrastructure

![The Responsibility Layer](assets/responsibility-layer-cover.png)

## AI Does Not Have an Intelligence Problem. It Has a Responsibility Problem.

*Notes from an ongoing experiment in governing AI-assisted work*

**By Douglas P. Galullo**  
Founder, Dog House Ventures LLC

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

## Repository contents

- `articles/` - canonical Markdown article
- `pdf/` - publication PDF
- `assets/` - cover artwork
- `research/` - sourcing agenda and future-paper scope
- `releases/` - fixed release notes
- `docs/history/` - public project-history notes (not thesis revisions)
- `CITATION.cff` - citation metadata
- `PUBLICATION.md` - authorship and publication record
- `CHANGELOG.md` - version history

## Related project history (not the thesis text)

Dog House Ventures occasionally records **high-level** applied-engineering milestones that are relevant to the responsibility thesis but are **not** amendments to the paper.

- [2026-07-20 — Mission-Control M1 experimental vertical slice](docs/history/2026-07-20-mission-control-m1-experimental-slice.md)

That note summarizes that a **bounded experimental** supervised request-to-durable-evidence path completed verification under explicit non-goals (not production control plane; further phases deferred). Implementation detail remains internal.

## Dog House Ventures map

| Artifact | Location |
|---|---|
| This public thesis | This repository |
| Internal constitutions & business records | `DOG HOUSE VENTURES LLC/` business filesystem (not this repo) |
| Engineering OS & labs | `DOG_HOUSE_SYSTEM/` |

## Relationship to Dog House Ventures governance

This repository is the **public research publication** of the responsibility thesis. It is not the company’s internal constitution stack, product source, or business-record filesystem.

Internal Dog House Ventures governance (Constitution, AI Control Constitution, File Structure Constitution, operational standards) lives in the company business filesystem under Dog House Ventures LLC operations policies — separate from this public research tree. As of 2026-07-20 that internal stack is treated as activated and stable for operations; this public thesis remains the published argument, not the operating control system.

The session handoff for company architecture (business filesystem) states the same operating principle published here: authority enters through a mandate/governance, evidence persists with decisions, and responsibility exits through explicit acceptance. Products (Doghouse as command-and-control, Investment Vault, Proof Ready, and others) inherit internal governance rather than replacing it.

This publication discloses thesis, process, and results. It does not disclose proprietary implementation (architecture, source code, prompts, schemas, or security design).

## Version

- Version: 1.0
- Initial public record: July 18, 2026
- Status: Published working thesis
- Author: Douglas P. Galullo
- Affiliation: Founder, Dog House Ventures LLC

## Suggested citation

> Galullo, Douglas P. "AI Does Not Have an Intelligence Problem. It Has a Responsibility Problem." Version 1.0, July 18, 2026.

## Feedback

Substantive criticism, corrections, counterarguments, and relevant sources are welcome through GitHub Issues or Discussions.

Feedback should address the argument rather than speculate about proprietary Doghouse implementation details.

## Rights

Copyright © 2026 Douglas P. Galullo. All rights reserved.

No open-source or Creative Commons license is granted for the article, abstract, cover image, or associated publication materials. See [LICENSE.md](LICENSE.md) and [NOTICE.md](NOTICE.md).
