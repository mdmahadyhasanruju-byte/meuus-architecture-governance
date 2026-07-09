Document: 03_domain_responsibility_map.md
Title: meUus Domain Responsibility Map
Status: Draft
Authority: Architectural Authority
Version: 0.1
Depends on:
- Book Zero
- 00_READ_FIRST.md
- README.md
- 01_master_architecture.md
- 02_ecosystem_topology.md
Supersedes: None
Purpose: Define responsibility ownership and exclusion boundaries for each principal ecosystem domain.
Last Updated: 2026-07-09
Reviewed by:
- Founder: N
- Architecture: N

---

## Purpose

Develop a conceptual responsibility map for the four principal meUus ecosystem domains.

This Draft identifies the intended work without assigning the full responsibility map. It is exploratory, is not canonical, and must not be cited as authority.

---

## Scope

This document is intended to clarify what each principal domain:

- Owns.
- Does not own.
- May reference.
- May receive.
- May express.
- May propose as evidence.
- May approve within its authority.
- Must never silently absorb.

The principal domains are:

- `meuus-architecture-governance`
- `meuus.org`
- `meuussoul.com`
- `meuus.app`

Detailed responsibility assignments remain to be developed in a later Working draft.

---

## Authority

This document is subordinate to:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.

Book Zero remains Foundational Authority. No repository or implementation surface may be assigned Foundational Authority by this document.

As a Draft under Architectural Authority, this document is not canonical. It cannot modify, reinterpret, or supersede a Frozen dependency, authorize implementation, create a new ecosystem domain, or begin Document 04.

---

## Inputs

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- Documented Founder direction and discoverable evidence relevant to domain responsibility.

---

## Outputs

If developed, reviewed, and Frozen through the governance lifecycle, this document is intended to provide:

- A responsibility ownership map for each principal domain.
- Explicit exclusion boundaries.
- Rules for reference, receipt, expression, evidence proposal, and approval.
- Protection against silent responsibility or authority absorption.
- A bounded responsibility reference for later architecture documents.

This Draft does not yet provide those canonical outputs.

---

## Dependencies

This document depends on:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.

It must refine the Frozen domain roles and topology without duplicating, replacing, or contradicting them.

No document may treat this Draft as an authoritative responsibility map.

---

## Interfaces

Conceptual responsibility interfaces to be examined during Working development include:

- Governance and public institutional expression.
- Governance and canonical knowledge.
- Governance and runtime evidence.
- Public institution and canonical knowledge.
- Canonical knowledge and runtime context.
- Runtime evidence and explicit review.

This Draft does not define technical interfaces, protocols, schemas, data movement, or runtime mechanics.

---

## Questions Unresolved

- What is the minimum responsibility vocabulary needed for all four domains?
- Which responsibilities are exclusive to one domain?
- Which responsibilities may be referenced or expressed across domains without transferring ownership?
- What may each domain receive, and under what conceptual boundary?
- Which domains may propose evidence, and which authority may approve its use?
- What responsibility movements require explicit review?
- What must remain prohibited, future, or unresolved?
- Which responsibility details belong in later architecture documents rather than this document?

---

## Risks

- Duplicating or silently redefining Frozen Documents 01 or 02.
- Assigning Foundational Authority to a repository or implementation surface.
- Confusing reference or expression with ownership.
- Allowing responsibility to move silently between domains.
- Introducing implementation assumptions into the responsibility map.
- Making the document too broad to remain explainable.
- Presenting future responsibilities as operational.

---

## Non-goals

This document will not:

- Modify Book Zero, `00_READ_FIRST.md`, `README.md`, `01_master_architecture.md`, or `02_ecosystem_topology.md`.
- Create new domains or transfer Foundational Authority.
- Select technologies, frameworks, vendors, or hosting.
- Define databases, APIs, schemas, or technical protocols.
- Define UI, authentication, payments, analytics, or deployment.
- Define runtime implementation or product features.
- Define pricing or marketing claims.
- Authorize implementation work.
- Begin, create, or authorize Document 04.

---

## Review Criteria

Before this document may move from Draft to Working, reviewers should confirm:

- It remains subordinate to all declared dependencies.
- It refines rather than duplicates Frozen Documents 01 and 02.
- Its required sections are substantially developed.
- Responsibility ownership and exclusions remain conceptual and explainable.
- Reference, receipt, expression, evidence proposal, and approval remain distinguishable.
- Book Zero remains the sole Foundational Authority.
- Uncertainty and non-goals remain explicit.
- No implementation details or operational overclaims are introduced.
