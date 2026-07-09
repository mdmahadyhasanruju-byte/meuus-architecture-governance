Document: 04_authority_flow_and_decision_rights.md
Title: meUus Authority Flow and Decision Rights
Status: Ready for Review
Authority: Architectural Authority
Version: 0.1
Depends on:
- Book Zero
- 00_READ_FIRST.md
- README.md
- 01_master_architecture.md
- 02_ecosystem_topology.md
- 03_domain_responsibility_map.md
Supersedes: None
Purpose: Define how authority flows and how decision rights are assigned, constrained, escalated, and reviewed across the meUus ecosystem.
Last Updated: 2026-07-09
Reviewed by:
- Founder: N
- Architecture: N

---

## Purpose

This document defines the conceptual flow of authority and the boundaries of decision rights across the meUus ecosystem.

It explains how higher authority constrains lower authority, how evidence and proposals may move upward for review, which decisions may be made within inherited boundaries, which decisions require review or escalation, and which decisions are forbidden.

This document is Ready for Review. Its sections are declared complete and now await formal Founder Review and Architecture Review. It is not Frozen, is not canonical, and must not be treated as authority for implementation.

---

## Scope

This document defines:

- The inherited authority hierarchy.
- The distinction between constitutional authority and bounded domain decision rights.
- Decision-right categories and states.
- Direct, proposal, review, approval, and escalation boundaries.
- Freeze Rule triggers.
- Bounded implementation decisions.
- Public expression, canonical knowledge, runtime evidence, and status decision boundaries.
- Decisions that must never be made silently.

It does not redefine the authority hierarchy, domain topology, or responsibility ownership established by Frozen Documents 01-03.

### Authority Flow Overview

Authority flows downward:

```text
Book Zero
Foundational Authority
        |
        v
00_READ_FIRST.md
Governance Authority
        |
        v
Frozen architecture documents
Architectural Authority
        |
        v
Implementation specifications and implementation
Implementation Authority
```

Evidence and proposals may move upward or across domains for review. They do not move as authority:

```text
Evidence or proposal
        |
        v
Relevant review gate
        |
        v
Approved decision, rejection, or explicit deferral
```

No repository, website, application, runtime, content surface, popularity measure, analytics result, market signal, or implementation behavior acquires higher authority merely by existing or producing evidence.

### Constitutional Authority Layers

#### Foundational Authority

Foundational Authority belongs to Book Zero only.

This document does not assign a right to redefine foundational assumptions. Any apparent conflict with Book Zero must be documented and escalated to Founder Review under the inherited governance rules.

No lower authority may:

- Contradict Book Zero.
- Treat implementation evidence as a foundational assumption.
- Acquire Foundational Authority through publication, use, popularity, or institutional role.

#### Governance Authority

Governance Authority belongs to `00_READ_FIRST.md`.

It defines:

- The authority hierarchy.
- Document lifecycle.
- Review process.
- Freeze Rule.
- Dependency requirements.
- Uncertainty documentation.

Changes to Frozen governance follow the Freeze Rule. This document cannot create a parallel governance process.

#### Architectural Authority

Architectural Authority belongs to Frozen architecture documents.

Frozen Documents 01-03 are current Architectural Authority. Document 04 is Ready for Review and remains non-canonical until it completes the governance lifecycle.

Draft, Working, and Ready for Review documents may be developed or reviewed according to their status, but they do not become canonical merely because they exist.

#### Implementation Authority

Implementation Authority belongs to bounded implementation work within approved architecture.

Implementation may decide how to execute approved architecture where:

- The decision remains inside the responsible implementation domain.
- No higher-authority rule or Frozen boundary changes.
- No responsibility transfers between domains.
- No public, canonical, or operational claim becomes broader than its evidence.
- No unresolved privacy, consent, safety, or authority question is silently answered.

Implementation Authority cannot redefine foundational assumptions, governance, architecture, canonical knowledge, approved public truth, or another domain's responsibility.

### Bounded Domain Decision Contexts

The following are bounded decision contexts, not new constitutional authority levels:

#### Public Expression

`meuus.org` may express approved public institutional truth within inherited governance, architecture, evidence, and status boundaries.

Public expression cannot create Foundational, Governance, or Architectural Authority. Publication cannot approve the truth it expresses.

#### Canonical Knowledge

`meuussoul.com` holds the Planned architectural role for preserving canonical knowledge, learning, and provenance.

Canonical knowledge does not create governance or architecture authority. The process that grants canonical status remains unresolved and must not be self-assigned by the domain.

#### Runtime Evidence

`meuus.app` may produce or hold runtime evidence only within approved boundaries.

Runtime evidence remains evidence, not authority. Frequency, personalization, user demand, popularity, or observed outcomes cannot silently promote it into canonical knowledge, public truth, governance, or architecture.

### Decision-Right Categories

| Category | Meaning |
| --- | --- |
| May decide directly | May choose within an already approved and bounded authority without changing a higher boundary |
| May express | May communicate an approved decision or truth without creating new authority |
| May propose | May submit a candidate change, evidence item, or decision for review |
| May review | May evaluate a proposal only within an explicitly assigned review role |
| Must escalate | Must stop direct action and send the matter to the appropriate authority |
| Must not decide | Has no decision right over the subject |
| Requires Founder Review | Requires review for constitutional integrity or institutional readiness |
| Requires Architecture Review | Requires review for structural integrity, truthfulness, or maintainability |
| Requires Freeze Rule | Would modify a Frozen document or canonical architectural boundary |
| Requires later document | The decision process or authority remains unresolved and must not be invented here |
| Forbidden | No lower authority may make or imply the decision |

A right to express, propose, review, or record does not imply a right to approve.

### Decision States

| State | Meaning |
| --- | --- |
| Decidable | May be decided directly within an approved boundary |
| Expressible | May be communicated after approval without creating authority |
| Proposable | May be submitted for review but has no effect yet |
| Review-gated | Requires an identified review before taking effect |
| Escalated | Direct action is paused pending the appropriate review |
| Frozen-change | Requires the Freeze Rule |
| Forbidden | Must not be decided by the lower authority |
| Future | Belongs to a possible later approved state |
| Unresolved | No approved decision right or process yet exists |

### Decision Rights Matrix

| Decision subject | Direct decision right | Required review or gate | Must not decide |
| --- | --- | --- | --- |
| Foundational assumptions | Not assigned by this document | Apparent conflicts require Founder Review | Governance, architecture, implementation, public, knowledge, and runtime surfaces |
| Governance lifecycle | Governed only by the Charter | Frozen change requires Freeze Rule | Architecture and implementation surfaces |
| Architecture document content before Freeze | Authors may draft within dependencies | Founder Review and Architecture Review before Freeze | Implementation surfaces cannot approve |
| Frozen architecture change | None directly | Freeze Rule, including required reviews and decision record | Silent edits by any contributor or implementation |
| Public institutional claim | `meuus.org` may express already approved truth | New or broadened claims require the appropriate unresolved institutional review | Knowledge or runtime surfaces cannot independently create the claim |
| Canonical knowledge status | No direct right currently established | Requires later document and explicit review authority | Public or runtime surfaces cannot grant canonical status |
| Runtime reflection behavior | Bounded implementation choices may execute approved architecture | Escalate when safety, privacy, claims, or domain boundaries change | Runtime cannot redefine higher authority |
| Runtime evidence promotion | Runtime may propose evidence | Review-gated; approval authority and threshold require later document | Runtime cannot promote its own evidence |
| Privacy and consent | No broad decision right established here | Requires later document and Founder Review before boundary expansion | Implementation cannot infer permission |
| Cross-domain responsibility transfer | None directly | Requires Founder Review, Architecture Review, and Freeze Rule where Frozen boundaries change | Any domain acting alone |
| Status classification | A domain may report bounded evidence within its scope | Broader or changed status requires evidence and appropriate review | Popularity, analytics, or marketing cannot decide |
| Implementation details | Implementation may decide within approved architecture | Escalate when a higher boundary or unresolved matter is affected | Governance and architecture cannot be silently redefined |
| Professional, legal, religious, or crisis authority claim | None | No lower review can manufacture such authority | App, website, knowledge, or governance repository |
| DLAS definition or runtime authority | None while unresolved | Requires later Founder-approved architecture | Runtime or implementation surfaces |

### Direct Decision Rights

A direct decision is permitted only when all of the following are true:

1. The deciding domain already owns the relevant responsibility.
2. The decision remains within Frozen architecture.
3. The decision does not change a status or public claim beyond evidence.
4. The decision does not transfer responsibility or authority.
5. The decision does not modify a Frozen document.
6. The decision does not resolve a documented uncertainty outside the domain's authority.
7. The decision does not broaden private-data use, professional authority, or future-system claims.

If any condition fails or is unclear, the matter must be escalated.

### Proposal Rights

Any domain may propose a change within the proposal boundaries established by Frozen Document 03.

A proposal must identify:

- The decision subject.
- The current authority and owner.
- The requested change.
- The evidence and its limitations.
- The affected Frozen or non-Frozen boundaries.
- The required reviewing authority, if known.
- Any unresolved authority or risk.

A proposal remains non-operative until approved. The ability to propose does not create a right to review, approve, implement, publish, or treat the proposal as true.

### Review and Approval Rights

Founder Review evaluates constitutional integrity and institutional readiness.

Architecture Review evaluates structural integrity, truthfulness, and maintainability.

Both reviews are required before an architecture document becomes Frozen. Changes to an already Frozen document additionally require the Freeze Rule process defined by `00_READ_FIRST.md`.

The repository records review outcomes; it does not itself become the approving actor.

Public expression, canonical knowledge, and implementation may have bounded review processes only when those processes are explicitly established. Where no approved process exists, the decision right remains Unresolved.

### Escalation Rules

A matter must be escalated when:

1. It conflicts or appears to conflict with higher authority.
2. It would modify a Frozen document or boundary.
3. The decision owner or approving authority is unclear.
4. Evidence is insufficient for the proposed claim.
5. A responsibility would move between domains.
6. Runtime evidence is proposed for canonical, public, governance, or architecture use.
7. Private reflection is proposed for a new purpose or audience.
8. A public statement would broaden approved truth or status.
9. A canonical claim lacks an approved status process or provenance.
10. An implementation choice would answer an architectural uncertainty.
11. A system would claim therapeutic, diagnostic, legal, professional, religious, emergency, or crisis authority.
12. A Future or Not live capability would be represented as Existing, Verified, or operational.

Escalation pauses the proposed decision. Silence, delay, popularity, urgency, or implementation convenience does not count as approval.

### Freeze Rule Triggers

The Freeze Rule is triggered when a proposed decision would:

- Change text, status, version, meaning, dependency, or authority in a Frozen document.
- Contradict or replace a Frozen architectural boundary.
- Transfer a responsibility fixed by Frozen architecture.
- Broaden a canonical architecture claim beyond its Frozen scope.
- Retire or supersede a Frozen architecture document.

The Freeze Rule requires the process defined in `00_READ_FIRST.md`, including a decision record, justification, Founder approval, Architecture Review confirmation, version increment, and change-log treatment.

This Ready for Review document does not create a Decision Register entry or modify a Frozen document.

### What Implementation May Decide

Implementation may decide bounded execution details when the decision:

- Faithfully implements approved architecture.
- Remains within the implementation repository's responsibility.
- Does not change authority, responsibility, or cross-domain boundaries.
- Does not create or broaden public, canonical, status, safety, or professional claims.
- Does not silently resolve an unresolved architecture question.
- Does not require a Frozen document change.

This document does not select or prescribe any implementation option.

### What Implementation Must Never Decide

Implementation must never silently decide:

- Foundational assumptions.
- Governance lifecycle or review rules.
- Architectural authority or Frozen boundaries.
- Which domain owns a responsibility.
- What becomes approved public institutional truth.
- What becomes canonical knowledge.
- Whether runtime evidence becomes authority.
- Whether private reflection may be reused outside its approved boundary.
- Whether a system has professional, legal, religious, emergency, or crisis authority.
- Whether a Planned, Future, Not live, or unverified system is operational.
- Whether popularity, analytics, market pressure, user demand, or commercial value overrides higher authority.

### Public Expression Decision Rights

`meuus.org` may decide how to express already approved public institutional truth within its bounded responsibility, provided meaning, status, provenance, and evidence limits remain intact.

It may propose:

- Corrections to public wording.
- Status corrections.
- Institutional clarifications.
- New claims for explicit review.

It must escalate when expression would change approved meaning, broaden a claim, weaken provenance, imply unverified operation, or absorb canonical or governance authority.

The exact editorial approval process beyond already approved truth remains Unresolved.

### Canonical Knowledge Decision Rights

`meuussoul.com` may preserve, organize, reference, and propose canonical knowledge within its Planned architectural role.

It may not self-grant canonical status, governance authority, or architecture authority. Candidate knowledge remains Proposed until an approved canonical review process exists and grants status.

The canonical approval process, evidence threshold, and reviewing authority require a later document.

### Runtime Evidence Decision Rights

`meuus.app` may identify and propose runtime evidence within approved runtime, privacy, consent, and provenance boundaries.

It may not:

- Approve its own evidence as canonical knowledge.
- Convert frequency or user demand into authority.
- Publish private reflection as institutional truth.
- Use runtime outcomes to amend governance or architecture automatically.

Any promotion of runtime evidence is Review-gated. Exact thresholds and approval authority require a later document.

### Status Classification Decision Rights

Status claims must remain no broader than evidence.

A domain may report evidence about its own state, but:

- Existing does not mean Verified or live.
- Verified applies only to the claim and evidence reviewed.
- Planned and Future do not mean Existing.
- Not live must not be represented as operational.
- Repetition across domains does not strengthen status.
- A broader classification requires new evidence and appropriate review.

The exact status verification process and cadence remain Unresolved.

### Emergency, Professional, and Religious Authority Boundaries

No repository, public website, knowledge platform, application, runtime, content, or architecture document acquires therapy, diagnostic, legal, professional, religious, emergency, or crisis authority through implementation or declaration.

No lower authority may decide to represent meUus as replacing those authorities. Safety-related implementation must remain within separately approved boundaries and cannot create authority by urgency alone.

### DLAS Decision Boundary

DLAS remains a conceptual Future runtime family and architecture subject.

Its definition, scope, authority, decision rights, and runtime behavior remain Unresolved. It is not live, and no implementation surface may define or operationalize it as approved architecture without later Founder-approved architectural work.

### Matters Reserved for Later Documents

This document does not decide:

- Canonical knowledge approval process.
- Institutional editorial approval process.
- Privacy, consent, retention, aggregation, or disclosure authority.
- Runtime evidence promotion thresholds.
- Status verification process and cadence.
- Emergency or crisis implementation behavior.
- Human staffing or organizational delegation.
- Technical permissions, access control, or workflow.
- DLAS definition or internal architecture.
- Decision rights for any future domain not approved by the Founder.

---

## Authority

This document is subordinate to:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- `03_domain_responsibility_map.md`.

Book Zero remains Foundational Authority. `00_READ_FIRST.md` remains Governance Authority. Frozen Documents 01-03 remain controlling Architectural Authority for master roles, topology, and responsibility.

While its status is Ready for Review, it awaits formal review, is not canonical, and remains subject to change through the review process.

This document cannot:

- Modify or reinterpret a Frozen dependency.
- Create a new constitutional authority category.
- Claim or transfer Foundational or Governance Authority.
- Authorize implementation work.
- Begin or authorize Document 05.

---

## Inputs

The inputs to this Ready for Review document are:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- `03_domain_responsibility_map.md`.
- Documented Founder directives relevant to authority and decision rights.
- Discoverable evidence where a current-state decision claim is required.

Implementation state may provide evidence. It does not assign or expand authority.

---

## Outputs

If reviewed and Frozen through the governance lifecycle, this document is intended to provide:

- A canonical conceptual authority-flow map.
- A decision-right matrix.
- Direct, proposal, review, approval, escalation, and Freeze Rule boundaries.
- Explicit implementation decision limits.
- Decision boundaries for public expression, canonical knowledge, runtime evidence, status, and future systems.

At Ready for Review status, these outputs are declared complete but remain non-canonical pending formal review.

---

## Dependencies

This document depends on:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- `03_domain_responsibility_map.md`.

It inherits the authority hierarchy, lifecycle, topology, responsibility map, truth taxonomy, and evidence discipline established by those documents.

If this document conflicts with a Frozen dependency, the Frozen dependency governs and the conflict must be documented for review. No later document acquires authority merely by depending on this Ready for Review document.

---

## Interfaces

The interfaces below are conceptual authority relationships, not technical interfaces.

### Foundational and Governance Authority

Governance inherits foundational constraints but cannot redefine Book Zero.

### Governance and Architectural Authority

Governance defines how architecture is created, reviewed, Frozen, amended, and inherited. Architecture cannot create a parallel governance process.

### Architecture and Implementation Authority

Architecture defines approved boundaries. Implementation chooses bounded execution without redefining architecture.

### Evidence and Review

Evidence may trigger review but cannot change authority automatically.

### Proposal and Approval

A proposal requests a decision. Approval exists only when the proper reviewing authority grants it.

### Frozen Authority and Change

A proposed change to Frozen authority invokes the Freeze Rule rather than direct modification.

---

## Questions Unresolved

- What process grants canonical knowledge status?
  - **Disposition:** Deferred to later architecture document.
- What approval process governs institutional editorial decisions beyond already approved truth?
  - **Disposition:** Deferred to Founder Review.
- What privacy and consent authority governs new uses of private reflection?
  - **Disposition:** Deferred to Founder Review.
- What evidence threshold permits runtime evidence to become candidate canonical knowledge?
  - **Disposition:** Deferred to later architecture document.
- What status verification process and cadence govern operational claims?
  - **Disposition:** Requires evidence before resolution.
- What decision rights, if any, may be delegated to human roles without transferring domain authority?
  - **Disposition:** Deferred to later architecture document.
- How should emergency implementation decisions be bounded when delay may create harm?
  - **Disposition:** Deferred to Founder Review.
- Which conflicts require both Founder Review and Architecture Review when no Frozen text changes?
  - **Disposition:** Deferred to Architecture Review.
- What authority, if any, may define DLAS in later architecture?
  - **Disposition:** Deferred to Founder Review.
- Which decision-right terms require glossary treatment?
  - **Disposition:** Deferred to later architecture document.

These questions remain explicit and bounded. Their dispositions identify where resolution belongs without authorizing another document or resolving uncertainty by assumption.

---

## Risks

### Authority Inflation

Risk: a bounded responsibility or successful implementation could be mistaken for higher authority.

Response: preserve the four constitutional authority layers and distinguish domain decision contexts from authority levels.

### Evidence Inflation

Risk: runtime frequency, popularity, analytics, or market demand could be treated as approval.

Response: keep evidence below review and approval.

### Approval Ambiguity

Risk: a domain could act when no approved reviewer or process exists.

Response: mark the decision Unresolved and require escalation.

### Governance Overreach

Risk: governance could absorb bounded implementation or content decisions.

Response: preserve direct implementation rights inside approved architecture while escalating only boundary-changing decisions.

### Implementation Overreach

Risk: implementation could silently resolve architecture, privacy, status, or authority questions.

Response: define direct-decision conditions and explicit prohibitions.

### Freeze Bypass

Risk: a Frozen boundary could change through code, content, convention, or undocumented practice.

Response: treat semantic and responsibility changes as Freeze Rule triggers.

### Public or Canonical Authority Confusion

Risk: public expression or canonical knowledge could be treated as constitutional authority.

Response: classify them as bounded decision contexts within the inherited hierarchy.

### Runtime Authority Inflation

Risk: runtime evidence or user demand could become canonical or institutional authority.

Response: preserve runtime evidence as evidence and require explicit review.

### Professional Authority Overclaim

Risk: a runtime or public surface could imply therapy, diagnosis, legal, professional, religious, emergency, or crisis authority.

Response: forbid such authority claims and reserve safety behavior for later approved boundaries.

### Excessive Complexity

Risk: decision governance could become too complex to follow.

Response: use a small decision vocabulary and require escalation only when direct-decision conditions fail.

---

## Non-goals

This document does not:

- Modify Book Zero, `00_READ_FIRST.md`, `README.md`, or Frozen Documents 01-03.
- Create a new constitutional authority category.
- Transfer Foundational, Governance, or Architectural Authority.
- Assign human staffing, organizational positions, or operational teams.
- Select technologies, frameworks, vendors, or hosting.
- Define databases, APIs, schemas, protocols, or technical data flows.
- Define UI, authentication, payments, analytics, or deployment.
- Define technical permissions, access control, or workflow implementation.
- Define runtime implementation, product features, or application state.
- Define privacy, consent, retention, or legal mechanisms.
- Define pricing or marketing claims.
- Fully define DLAS or represent it as operational.
- Authorize implementation work.
- Begin, create, or authorize Document 05.

---

## Review Criteria

During formal Founder Review and Architecture Review, reviewers should confirm:

### Constitutional and Governance Integrity

- Book Zero remains Foundational Authority.
- `00_READ_FIRST.md` remains Governance Authority.
- Frozen Documents 01-03 remain controlling Architectural Authority.
- No bounded domain decision context is presented as a new constitutional authority level.
- No Frozen dependency is modified, reinterpreted, or contradicted.

### Structural Integrity

- Authority, responsibility, evidence, proposal, review, decision, approval, and escalation remain distinguishable.
- Decision categories and states are consistently applied.
- Direct decision and escalation boundaries are clear.
- Freeze Rule triggers match the Charter.
- Matters reserved for later documents remain outside scope.

### Truthfulness

- Claim does not exceed evidence.
- Runtime evidence remains evidence, not authority.
- Public expression does not create authority.
- Popularity, analytics, market pressure, frequency, or user demand cannot silently create authority.
- Future and Not live systems are not represented as operational.
- DLAS remains conceptual, Future, Unresolved, and not live.

### Institutional Readiness

- Founder Review and Architecture Review roles remain distinct.
- Public, canonical, runtime, governance, architecture, and implementation decisions remain bounded.
- Professional and religious authority are not claimed.
- Unknown decision rights remain Unresolved rather than invented.

### Implementation Independence

- No technology, framework, vendor, database, API, schema, UI, deployment, or runtime mechanism is embedded.
- Conceptual decision rights cannot be mistaken for technical permissions.

### Lifecycle Readiness

- All required sections are substantially complete.
- Dependencies and non-goals remain explicit.
- Unresolved questions are resolved or explicitly accepted for formal review.
- Founder Review and Architecture Review have not been presumed.
