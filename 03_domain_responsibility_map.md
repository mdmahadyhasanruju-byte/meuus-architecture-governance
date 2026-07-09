Document: 03_domain_responsibility_map.md
Title: meUus Domain Responsibility Map
Status: Ready for Review
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
- Founder: Y
- Architecture: N

---

## Purpose

This document defines the conceptual responsibility map for the four principal meUus ecosystem domains.

It refines the Frozen Master Architecture and Frozen Ecosystem Topology by distinguishing what each domain owns, does not own, may express, may reference, may receive, may propose, may approve, must never silently absorb, and must escalate for review.

This document is Ready for Review. Its sections are declared complete and now await formal Founder Review and Architecture Review. It is not Frozen, is not canonical, and must not be treated as authority for implementation.

---

## Scope

This document maps responsibility for:

- `meuus-architecture-governance`
- `meuus.org`
- `meuussoul.com`
- `meuus.app`

It defines conceptual accountability and exclusion boundaries. It does not establish present operational capability, implementation ownership, staffing, workflow mechanics, or technical access.

### Responsibility Map Overview

The four domains hold different primary responsibilities:

| Domain | Primary responsibility | Primary exclusion |
| --- | --- | --- |
| `meuus-architecture-governance` | Preserve governed architecture records and the architecture process under inherited authority | Does not own Foundational Authority or implementation behavior |
| `meuus.org` | Express approved institutional truth publicly | Does not own canonical knowledge depth or private runtime reflection |
| `meuussoul.com` | Preserve canonical knowledge, learning, and provenance | Does not own governance decisions or private runtime reflection |
| `meuus.app` | Hold reflection, Journey, and action runtime context within approved boundaries | Does not own canonical truth, institutional authority, or governance decisions |

These are architectural roles. A role does not prove that its full implementation exists, is Verified, or is live.

### Responsibility Categories

This document uses the following categories:

| Category | Meaning |
| --- | --- |
| Owns | Holds primary conceptual accountability for the responsibility within inherited authority |
| Does not own | Has no primary accountability or authority for the responsibility |
| May express | May present approved material appropriate to the domain without creating new authority |
| May reference | May point to another authority or domain while preserving source, status, and ownership |
| May receive | May accept a permitted representation, proposal, or evidence item without absorbing its source responsibility |
| May propose | May submit a candidate claim, correction, evidence item, or change for review |
| May approve | May approve only where an explicit higher-authority process grants approval authority |
| Must never silently absorb | Must not acquire the responsibility through storage, publication, use, repetition, or implementation |
| Must escalate for review | Must stop and seek the appropriate authority when a boundary, conflict, or unsupported claim appears |

Ownership is not unrestricted control. It remains subordinate to higher authority, evidence, and governance.

### Responsibility States

Responsibilities and responsibility movements may have these states:

| State | Meaning |
| --- | --- |
| Owned | Primary accountability is explicitly assigned to the domain |
| Referenced | The domain points to a source responsibility without acquiring it |
| Received | A permitted item enters the domain without transferring source ownership |
| Proposed | A candidate change or evidence item awaits review |
| Review-gated | Movement or use requires explicit approval before it can take effect |
| Forbidden | The responsibility or movement is prohibited |
| Future | The responsibility belongs to a possible later approved state and is not operationally asserted |
| Unresolved | The responsible authority or boundary has not yet been approved |

No state may be strengthened without evidence and the appropriate review.

### General Responsibility Rules

1. Book Zero remains Foundational Authority.
2. `00_READ_FIRST.md` remains Governance Authority.
3. Frozen Documents 01 and 02 establish the master roles and topology inherited here.
4. A domain may own a responsibility only within its inherited authority.
5. Expression, reference, receipt, or use does not transfer ownership.
6. A proposal is not an approval.
7. Evidence is not authority.
8. Publication does not create institutional, canonical, or architectural truth.
9. Repetition does not strengthen a claim.
10. A repository records governed decisions; it does not become the Founder or reviewing authority.
11. Private reflection remains within its approved boundary unless a later explicit privacy, consent, provenance, and review basis permits otherwise.
12. Planned, Future, Not live, or unverified responsibilities must not be represented as operational.

### Governance Repository Responsibilities

The responsibilities below apply to `meuus-architecture-governance`.

| Category | Responsibility boundary |
| --- | --- |
| Owns | The governed architecture record, architecture document lifecycle, declared dependencies, architecture decision traceability, and preservation of approved architectural judgment |
| Does not own | Book Zero, Foundational Authority, public institutional expression, canonical knowledge depth, private runtime reflection, application behavior, or implementation choices |
| May express | Accurate architecture status, approved architecture boundaries, review outcomes, dependencies, unresolved questions, and recorded decisions |
| May reference | Book Zero, constitutional sources, Frozen governance and architecture documents, Founder directives, review records, and discoverable evidence |
| May receive | Architecture proposals, bounded evidence summaries, conflict reports, review findings, and requests for governed change |
| May propose | Contributors may propose new architecture or amendments through the governance process; the repository preserves the proposal and its rationale |
| May approve | The repository itself does not approve. Founder Review and Architecture Review approve according to `00_READ_FIRST.md`; the repository may record their approved decision |
| Must never silently absorb | Foundational assumptions, implementation behavior, product ownership, canonical content ownership, public institutional authority, or private reflection data |
| Must escalate for review | Conflicts with higher authority, proposed Frozen changes, unsupported architectural claims, domain ownership transfers, and evidence that would alter canonical architecture |

The governance repository preserves architecture under inherited Foundational Authority. It does not possess or reinterpret Foundational Authority.

### `meuus.org` Responsibilities

The responsibilities below apply to the public institutional foundation.

| Category | Responsibility boundary |
| --- | --- |
| Owns | Public institutional expression, status-boundary presentation, Amanah, orientation, public trust, institutional explanation, and appropriate public links or previews |
| Does not own | Foundational or governance authority, canonical knowledge depth, private reflection or journey context, runtime behavior, or architecture approval |
| May express | Approved institutional statements, evidence-appropriate status, public orientation, Amanah, and bounded summaries or previews with provenance |
| May reference | Governance status, canonical knowledge, books, learning materials, approved runtime surfaces, and their verified boundaries |
| May receive | Approved institutional statements, provenance-preserving knowledge summaries, verified status evidence, and reviewed corrections appropriate for public expression |
| May propose | Public wording corrections, status corrections, institutional clarifications, and requests for review where public truth may have changed |
| May approve | No architectural, canonical, or runtime authority arises from this domain. Any editorial or institutional approval mechanism beyond already approved truth remains unresolved until explicitly governed |
| Must never silently absorb | Canonical knowledge ownership, private runtime data, user journeys, governance decisions, architecture authority, or unverified operational claims |
| Must escalate for review | Conflicts between public expression and governing sources, broader status claims, sensitive knowledge summaries, responsibility transfers, and any private information proposed for public use |

Public expression must remain no broader than approved truth and discoverable evidence.

### `meuussoul.com` Responsibilities

The responsibilities below apply to the canonical knowledge and learning domain.

| Category | Responsibility boundary |
| --- | --- |
| Owns | The architectural role for canonical knowledge, books, learning materials, provenance, source-of-truth knowledge, and structured learning |
| Does not own | Foundational or governance authority, institutional decisions, public status authority, private runtime reflection data, or runtime behavior |
| May express | Canonical knowledge, provenance, source status, learning structure, and explicit uncertainty once the relevant content is approved |
| May reference | Foundational and governance constraints, institutional context, source materials, evidence, and approved runtime boundaries |
| May receive | Source materials, provenance records, reviewed corrections, and candidate evidence that has passed the required boundary review |
| May propose | Candidate canonical knowledge, corrections, provenance changes, learning structures, and questions requiring review |
| May approve | No governance or architecture approval. The authority and process for granting canonical knowledge status remain unresolved and must not be self-assigned by the domain |
| Must never silently absorb | Governance decisions, institutional authority, private reflection, runtime-generated suggestions, popularity signals, or implementation behavior as canonical truth |
| Must escalate for review | Conflicting sources, insufficient provenance, proposed promotion of runtime evidence, institutional implications, responsibility transfers, and claims broader than evidence |

This responsibility is Planned as an architectural role. This document does not verify that the full knowledge platform or its capabilities are operational.

### `meuus.app` Responsibilities

The responsibilities below apply to the Reflection, Journey, and action runtime domain.

| Category | Responsibility boundary |
| --- | --- |
| Owns | The architectural responsibility for supporting runtime reflection, Journey, contextual action, and responsible next steps within approved boundaries |
| Does not own | Foundational Authority, governance decisions, institutional authority, canonical truth, therapy, diagnosis, legal advice, professional advice, religious authority, or crisis support |
| May express | User-authored reflection, contextual guidance, approved institutional boundaries, evidence-appropriate status, and clear distinctions between source knowledge and runtime suggestion |
| May reference | Approved institutional truth, canonical knowledge, provenance pointers, governance constraints, and applicable runtime boundaries |
| May receive | Approved contextual knowledge, institutional boundaries, status constraints, and user-provided context only within future approved privacy and consent boundaries |
| May propose | Runtime observations, user-reported concerns, candidate evidence, status corrections, and architecture questions for explicit review |
| May approve | No canonical, institutional, governance, or architectural claim. Runtime or user action does not constitute higher-authority approval |
| Must never silently absorb | Canonical knowledge ownership, institutional authority, governance power, professional or religious authority, private data beyond its approved purpose, or future capabilities as present reality |
| Must escalate for review | Safety-boundary concerns, conflicts with canonical or institutional truth, privacy or consent ambiguity, evidence proposed for external use, responsibility transfers, and claims broader than evidence |

The Phase Zero role remains subject to separate verification of present operation. Future journeys, DLAS runtime, and other action systems remain Future until approved. DLAS remains conceptual, unresolved, and not live.

### Cross-Domain Responsibility Matrix

| Responsibility | Governance repository | `meuus.org` | `meuussoul.com` | `meuus.app` |
| --- | --- | --- | --- | --- |
| Foundational constraints | References and inherits constraints | References and inherits constraints | References and inherits constraints | References and inherits constraints |
| Governed architecture record | Owns | References | References | References |
| Public institutional expression | Governs applicable boundaries | Owns | May supply canonical source | May display approved boundaries |
| Canonical knowledge and provenance | Governs applicable boundaries | References or summarizes | Owns architectural role | Uses contextually |
| Private reflection and journey context | Does not own | Does not own | Does not own | Owns architectural role within approved boundaries |
| Architecture proposal | Receives and records | May propose | May propose | May propose |
| Runtime evidence proposal | Receives for governed review where relevant | May report public effects | May receive after review | May propose |
| Architecture approval | Records approved outcome | Cannot approve | Cannot approve | Cannot approve |
| Operational status expression | Defines taxonomy and constraints | Expresses approved public status | Reports evidence within scope | Reports evidence within scope |

Every matrix entry identifies conceptual responsibility. It does not assert present operational capability.

### Approval Boundaries

Approval must remain distinct from ownership, expression, and proposal.

- Book Zero is not approved or redefined by an architecture domain.
- Governance rules are controlled by the Freeze Rule and the authority declared in `00_READ_FIRST.md`.
- Architecture approval requires the governed Founder Review and Architecture Review process.
- Public expression may communicate only already approved institutional truth; publication does not approve the truth it expresses.
- Canonical knowledge approval authority is unresolved and must be established before candidate knowledge becomes canonical.
- Runtime behavior, user choice, generated output, frequency, or popularity cannot approve institutional, canonical, or architectural claims.
- A domain may record or display an approval only when the approving authority and scope are discoverable.

### Escalation Rules

A domain must escalate for explicit review when:

1. A claim appears to conflict with a higher-authority document.
2. Evidence would require a change to a Frozen document.
3. A responsibility appears to belong to more than one domain.
4. A domain is asked to absorb another domain's ownership.
5. A current-state claim lacks sufficient evidence.
6. Private reflection is proposed for public, canonical, aggregate, or governance use.
7. Runtime evidence is proposed as candidate canonical knowledge.
8. A public summary may alter the meaning or status of canonical knowledge.
9. A future responsibility is proposed as Existing, Verified, or live.
10. The responsible reviewing authority is itself unresolved.

Escalation pauses the proposed movement. It does not authorize the receiving domain to act while review is pending.

### Forbidden Absorption

The following responsibility absorption is forbidden:

- Any repository or implementation surface absorbing Foundational Authority.
- `meuus.org` absorbing canonical knowledge depth or private runtime responsibility.
- `meuussoul.com` absorbing governance, institutional, or private runtime authority.
- `meuus.app` absorbing canonical truth, institutional authority, governance decisions, or professional and religious authority.
- Governance absorbing implementation behavior, product operation, canonical content ownership, or private reflection data.
- Any domain absorbing responsibility merely because it stores, links to, summarizes, displays, personalizes, or receives material.
- Any domain treating repeated, popular, automated, or commercially useful output as approval.

### Evidence and Proposal Responsibilities

Evidence and proposals remain below approval:

1. A domain may identify evidence within its scope.
2. Evidence must retain source, status, date, scope, provenance, and limitations.
3. A proposal must name the responsibility or claim it seeks to change.
4. The proposal must identify the authority required for review.
5. The receiving domain may not act as though the proposal is approved.
6. Private evidence remains inside its approved boundary while privacy and consent authority are unresolved.
7. Approved outcomes must be recorded by the domain responsible for the relevant authoritative record.

### Public Expression Responsibilities

Public institutional expression belongs to `meuus.org`, within inherited governance and evidence boundaries.

Public expression must:

- Distinguish approved truth from proposal, plan, aspiration, and uncertainty.
- Preserve status and evidence limits.
- Preserve provenance when summarizing canonical knowledge.
- Avoid implying that a linked knowledge or runtime system is operational without verification.
- Avoid turning orientation, visibility, or marketing advantage into authority.

Other domains may display necessary institutional boundaries, but doing so does not transfer ownership of public institutional expression.

### Canonical Knowledge Responsibilities

The canonical knowledge role belongs to `meuussoul.com`.

Canonical responsibility includes:

- Preserving source meaning and provenance.
- Distinguishing source knowledge from summary, interpretation, contextual guidance, and runtime suggestion.
- Recording uncertainty where evidence is incomplete.
- Preventing public or runtime adaptations from silently replacing the source.
- Requiring an approved path before candidate evidence becomes canonical.

The exact canonical approval process remains unresolved. The domain role alone does not grant self-approval authority.

### Runtime Reflection Responsibilities

The runtime responsibility belongs to `meuus.app` within approved boundaries.

Runtime responsibility includes:

- Preserving the distinction between user-authored reflection and system-generated guidance.
- Keeping contextual use separate from canonical ownership.
- Preserving institutional and status boundaries.
- Keeping private reflection within its approved purpose.
- Treating runtime observations as candidate evidence rather than truth or authority.
- Escalating safety, privacy, consent, provenance, and authority conflicts.

This document defines no runtime mechanics and makes no claim that future runtime capabilities are operational.

### Matters Reserved for Later Documents

This document does not decide:

- The canonical knowledge approval process.
- Detailed institutional editorial approval.
- Privacy, consent, retention, aggregation, or disclosure rules.
- Evidence thresholds for promotion into canonical knowledge.
- Operational staffing or human role assignments.
- Technical permissions or access control.
- Status verification procedures and cadence.
- Detailed content provenance mechanisms.
- The definition or internal architecture of DLAS.
- Responsibilities for any future domain not approved by the Founder.

---

## Authority

This document is subordinate to:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.

Book Zero remains Foundational Authority. `00_READ_FIRST.md` remains Governance Authority. Frozen Documents 01 and 02 remain controlling Architectural Authority for master roles and topology.

While its status is Ready for Review, it awaits formal review, is not canonical, and remains subject to change through the review process.

This document cannot:

- Modify or reinterpret a Frozen dependency.
- Claim Foundational or Governance Authority.
- Create or transfer responsibility outside inherited boundaries.
- Authorize implementation work.
- Begin or authorize Document 04.

---

## Inputs

The inputs to this Ready for Review document are:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- Documented Founder directives relevant to responsibility.
- Discoverable evidence where a current-state responsibility claim is required.

Implementation state may provide evidence about what exists. It does not assign architectural responsibility or authority.

---

## Outputs

If reviewed and Frozen through the governance lifecycle, this document is intended to provide:

- A canonical conceptual responsibility map for the four principal domains.
- Explicit ownership and exclusion boundaries.
- Rules for expression, reference, receipt, proposal, approval, and escalation.
- Protection against silent responsibility absorption.
- A responsibility reference for later architecture documents.

At Ready for Review status, these outputs are declared complete but remain non-canonical pending formal review.

---

## Dependencies

This document depends on:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.

It inherits the authority hierarchy, domain roles, topology, movement rules, truth taxonomy, and evidence discipline established by those documents.

If this document conflicts with a Frozen dependency, the Frozen dependency governs and the conflict must be documented for review. No later document acquires authority merely by depending on this Ready for Review document.

---

## Interfaces

The interfaces below are conceptual responsibility relationships, not technical interfaces.

### Governance and Public Expression

Governance constrains public institutional claims. `meuus.org` owns public expression but cannot alter the authority it expresses.

### Governance and Canonical Knowledge

Governance constrains the authority and use of canonical knowledge. `meuussoul.com` owns the canonical knowledge role but cannot make governance decisions.

### Governance and Runtime Evidence

Runtime evidence may be proposed for governed review. It remains evidence and does not acquire architectural authority.

### Public Expression and Canonical Knowledge

`meuus.org` may reference or summarize canonical knowledge with provenance. `meuussoul.com` retains the canonical knowledge role.

### Canonical Knowledge and Runtime Context

`meuus.app` may use approved knowledge contextually. Contextual use does not transfer canonical ownership.

### Runtime Evidence and Review

`meuus.app` may propose bounded evidence. The appropriate authority must review it before it can affect public, canonical, or architectural responsibility.

---

## Questions Unresolved

- What explicit process grants canonical knowledge status?
  - **Disposition:** Deferred to later architecture document.
- What approval boundary governs institutional editorial changes that do not alter approved truth?
  - **Disposition:** Deferred to Founder Review.
- What privacy and consent authority governs receipt or external use of private reflection?
  - **Disposition:** Deferred to Founder Review.
- What evidence threshold permits runtime observations to become candidate canonical knowledge?
  - **Disposition:** Deferred to later architecture document.
- How should conflicts between two apparent responsibility owners be resolved before either acts?
  - **Disposition:** Deferred to Architecture Review.
- What status verification process confirms that an architectural responsibility is operational?
  - **Disposition:** Requires evidence before resolution.
- What responsibilities, if any, may be shared without creating shared authority?
  - **Disposition:** Deferred to later architecture document.
- How should external institutions or future domains participate without absorbing existing responsibility?
  - **Disposition:** Requires evidence before resolution.
- Which terms require glossary treatment before this map can be interpreted consistently?
  - **Disposition:** Deferred to later architecture document.

These questions remain explicit and bounded. Their dispositions identify where resolution belongs without authorizing another document or resolving uncertainty by assumption.

---

## Risks

### Foundational Authority Drift

Risk: a repository or implementation surface could be treated as the source of foundational assumptions.

Response: preserve Book Zero as Foundational Authority and limit governance responsibility to the governed architecture record and process.

### Responsibility Absorption

Risk: a domain could acquire another domain's responsibility through publication, storage, linking, receipt, or use.

Response: distinguish ownership from expression, reference, receipt, and proposal.

### Approval Inflation

Risk: ownership, publication, operation, or popularity could be mistaken for approval authority.

Response: require explicit, discoverable approval authority and keep proposals below approvals.

### Operational Overclaiming

Risk: architectural responsibility could be presented as proof of operational capability.

Response: separate role from implementation state and preserve inherited evidence classifications.

### Private Boundary Failure

Risk: private reflection could move into public, canonical, or governance contexts without an approved basis.

Response: prohibit silent movement and require future privacy, consent, provenance, and review authority.

### Canonical Knowledge Dilution

Risk: public summaries or runtime adaptations could silently replace canonical knowledge.

Response: preserve canonical ownership, provenance, and distinctions among source, summary, context, and suggestion.

### Governance Overreach

Risk: governance could absorb implementation, content, or operational responsibility.

Response: limit governance to architecture records and process under inherited authority.

### Implementation Leakage

Risk: responsibility mapping could become technical permissions, workflow, or product specification.

Response: keep the map conceptual and reserve implementation mechanisms for their proper authority.

### Excessive Centralization

Risk: this document could absorb detailed decisions that belong to later architecture.

Response: reserve approval processes, privacy, provenance, status procedures, and technical roles for later documents.

---

## Non-goals

This document does not:

- Modify Book Zero, `00_READ_FIRST.md`, `README.md`, `01_master_architecture.md`, or `02_ecosystem_topology.md`.
- Create new domains or transfer Foundational Authority.
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
- Begin, create, or authorize Document 04.

---

## Review Criteria

During formal Founder Review and Architecture Review, reviewers should confirm:

### Constitutional and Governance Integrity

- Book Zero remains Foundational Authority.
- The document remains subordinate to every declared dependency.
- It does not modify, reinterpret, or contradict a Frozen document.
- It does not grant a repository or domain authority beyond inherited boundaries.

### Structural Integrity

- Each domain has all nine responsibility categories addressed.
- Ownership, expression, reference, receipt, proposal, approval, and escalation remain distinguishable.
- The cross-domain matrix is consistent with the domain-specific maps.
- Forbidden absorption is explicit.
- Matters reserved for later documents remain outside this scope.

### Truthfulness

- No responsibility claim exceeds its evidence.
- Architectural role is not represented as operational capability.
- Planned, Future, Not live, and unverified responsibilities remain clearly bounded.
- DLAS remains conceptual, unresolved, and not live.

### Institutional Readiness

- Public expression, canonical knowledge, runtime reflection, and governance remain separate.
- Private reflection cannot move silently.
- Approval authority is explicit where known and unresolved where not known.
- Escalation rules protect against silent responsibility drift.

### Implementation Independence

- No technology, framework, vendor, database, API, schema, UI, deployment, or runtime mechanism is embedded.
- Conceptual responsibility cannot be mistaken for technical access or operational control.

### Lifecycle Readiness

- All required sections are substantially complete.
- Dependencies and non-goals remain explicit.
- Unresolved questions are resolved or explicitly accepted for formal review.
- Founder Review and Architecture Review have not been presumed.
