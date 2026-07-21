# Public Claim Ledger Charter

**Status:** ACTIVE — repository identity and admission standard  
**Applies to:** This repository (`responsibility-infrastructure`)  
**Last updated:** 2026-07-21  

## 1. What this repository is

This repository is Dog House Ventures LLC’s **public claim ledger**.

It is the permanent public home for:

1. **Published research** — theses, articles, abstracts, citation metadata, and versioned release records.  
2. **Public engineering and product milestones** — high-level history of material engineering, product-maturity, validation, and governance events that strengthen the public case for the company’s discipline.  
3. **Program status** — current public status of named programs and products, with explicit non-claims.  
4. **Evidence mapping** — every factual public claim linked to a source and an evidence class.  
5. **Corrections** — superseded or corrected claims kept visible and cross-linked.

It exists so an independent reader can understand **what Dog House Ventures claims**, **what evidence supports those claims**, **what remains internal**, and **where disclosure boundaries intentionally exist**.

## 2. What this repository is not

- Not product source code or private development monorepos.  
- Not the company’s internal constitution stack or business-record filesystem.  
- Not a marketing site (see sibling public surfaces for company front-door narrative).  
- Not a promise that proprietary tests can be re-run by outsiders unless a claim is classed `PUBLIC-ARTIFACT` or `INDEPENDENTLY-ATTESTED`.  
- Not authorization for production, App Store, investor-readiness, or scientific-finality claims unless a note explicitly states so (default: it does not).

## 3. Publication standard

**Disciplined publication** — not maximum disclosure, and not minimal disclosure by default.

For every candidate public addition, all of the following must be true:

1. **Credibility** — it materially strengthens the public case for engineering discipline, governance, products, or research.  
2. **Safety** — it can be summarized without proprietary implementation, security-sensitive material, competitive mechanism detail, or confidential company information.  
3. **Evidence** — authoritative evidence exists (public artifact and/or named internal title).  
4. **Meaning** — a skeptical technical reviewer would treat it as a meaningful addition, not noise.

If yes → admit a public summary.  
If no → defer or exclude.

**Four simultaneous goals:** truthfulness; credibility; evidence-based publication; long-term protection of Dog House Ventures intellectual property.

## 4. Evidence classes

See [EVIDENCE_CLASSES.md](EVIDENCE_CLASSES.md). Every factual claim in this repository must carry one of:

| Class | Code | Reader power |
|---|---|---|
| Public artifact | `PUBLIC-ARTIFACT` | Can check files, tags, or public URLs in this ledger (or cited public URL) |
| Internally attested | `ATTESTED-INTERNAL` | Company attests from named internal records (title only); cannot re-run proprietary verification |
| Independently attested | `INDEPENDENTLY-ATTESTED` | Named third party, external audit, or independent recompute path |

## 5. Programs and milestone IDs

Programs are registered in [PROGRAMS.md](PROGRAMS.md).

- **Do not invent empty product trees.** Structure follows admitted content.  
- Milestone IDs may be program-scoped (e.g. Mission Control **M1** / alias **MC-M1**).  
- Prior public labels are not renumbered.  
- Governance milestones are not forced into engineering M-numbering.

## 6. Required fields on public history notes

| Field | Required |
|---|---|
| Milestone / event ID | Yes |
| Program | Yes |
| Engineering or event completion date (when known) | Yes |
| Public documentation date | Yes |
| Why it mattered | Yes |
| What was demonstrated (capability/result level) | Yes |
| Explicit non-claims | Yes |
| Supporting evidence (public + internal titles) | Yes |
| Evidence classification | Yes |

If public documentation date is later than engineering completion, say so. Do not backdate git history to invent contemporaneous publication.

## 7. Hierarchy of contents

1. Research core (thesis and papers)  
2. Public engineering / product / governance record  
3. Evidence system (classes, index, corrections)  
4. Maintainer adapters (`AI_START_HERE`, `AGENTS`, `CLAUDE`) — for authorized maintainers, not the public argument  

## 8. Related public surfaces

| Surface | Role |
|---|---|
| **This repository** | Authoritative public claim ledger (research + engineering/product/governance record + evidence map) |
| `doghouse-public` | Company front door / product narrative at a high level |
| `doghouse-governed-ai-evaluations` | Evaluation protocols and results when evaluations publish; plan-only material is not completed evidence |

## 9. Authority

This charter governs framing for this repository. It does not outrank company publication policy (DHV-PUB-001), the Publication Safety Gate, founder instruction, or the Doghouse Constitution. External publication remains fail-closed under the Safety Gate.
