Document: 02_ecosystem_topology.md
Title: meUus Ecosystem Topology
Status: Working
Authority: Architectural Authority
Version: 0.1
Depends on:
- Book Zero
- 00_READ_FIRST.md
- README.md
- 01_master_architecture.md
Supersedes: None
Purpose: Define the ecosystem topology derived from the Frozen Master Architecture.
Last Updated: 2026-07-09
Reviewed by:
- Founder: N
- Architecture: N

---

## Purpose

This document refines the Frozen Master Architecture into a detailed conceptual topology for the meUus ecosystem.

It explains how the four principal domains are positioned in relation to one another, what each domain owns, what may move between domains, what must not move, and what requires explicit review. It provides more structural detail than `01_master_architecture.md` without restating or replacing the master architecture.

This is a Working document. Its sections are substantially developed but remain subject to Founder Review and Architecture Review. It is not Frozen, is not canonical, and must not be treated as authority for implementation.

---

## Scope

This document defines:

- The topology of the four principal ecosystem domains.
- The conceptual relationships among governance, public institution, knowledge, and runtime.
- Responsibility and exclusion boundaries for each domain.
- Allowed, forbidden, and review-gated cross-domain movement.
- The conceptual movement of authority, public expression, knowledge, status, and evidence.
- Separation rules that prevent authority drift and domain collapse.
- The topology concerns that must remain for later architecture documents.

This document does not redefine the roles established by `01_master_architecture.md`. It describes their structural relationship in greater detail.

### Topology Overview

The ecosystem consists of four distinct domains:

1. **Governance and architecture:** `meuus-architecture-governance`
2. **Public institution:** `meuus.org`
3. **Canonical knowledge and learning:** `meuussoul.com`
4. **Reflection, Journey, and action runtime:** `meuus.app`

The conceptual topology is:

```text
Book Zero
    |
    v
00_READ_FIRST.md
    |
    v
Frozen architecture in meuus-architecture-governance
    |
    +--------------------+--------------------+
    |                    |                    |
    v                    v                    v
meuus.org          meuussoul.com          meuus.app
Public             Canonical              Reflection,
institution        knowledge              Journey, and
                   and learning           action runtime
    |                    |                    |
    +------ public ------+------ contextual --+
           orientation          knowledge

Runtime evidence may return toward knowledge or governance
only through explicit review. It does not return as authority.
```

This is a conceptual authority and responsibility map. It is not a network, deployment, data, or runtime diagram.

### Principal Domains

#### `meuus-architecture-governance`

Topology role:

- Sits above implementation domains in the authority hierarchy.
- Preserves the governed architecture record and architectural judgment under inherited Foundational Authority.
- Defines approved architecture boundaries through governed documents.
- Receives proposed evidence or change requests only through explicit review.

It does not:

- Operate application or website behavior.
- Own UI, runtime state, APIs, databases, deployment, or product features.
- Acquire new constitutional authority through implementation evidence.

#### `meuus.org`

Topology role:

- Serves as the public institutional foundation.
- Expresses approved public truth, status boundaries, Amanah, orientation, public trust, book preview links, and institutional explanation.
- Directs people toward approved knowledge or runtime surfaces using evidence-appropriate status language.

It does not:

- Own private reflection or journey data.
- Replace canonical knowledge depth with public summaries.
- Convert publication into governance or architecture authority.
- Represent planned, future, or unverified capabilities as operational.

#### `meuussoul.com`

Topology role:

- Serves as the canonical knowledge and learning domain.
- Preserves books, learning materials, source-of-truth knowledge, provenance, and structured learning.
- Provides reviewed knowledge that may be summarized publicly or used contextually by runtime systems.

It does not:

- Make constitutional, governance, or architecture decisions.
- Own private runtime reflection data.
- Convert runtime observations into canonical knowledge without explicit review.
- Acquire institutional authority merely by preserving knowledge.

Its architectural role is Planned. Its operational status is not Verified by the evidence available to this document.

#### `meuus.app`

Topology role:

- Serves as the Reflection, Journey, and action runtime domain.
- Holds the architectural role of the Phase Zero browser-local reflection prototype, subject to separate verification of present operation.
- May support future journeys, reflection artifacts, responsible next steps, DLAS runtime, and other action systems only after governance approval.

It does not:

- Assert or redefine canonical truth.
- Make institutional or governance decisions.
- Promote private reflection into public or canonical contexts without explicit review.
- Replace therapy, diagnosis, legal advice, professional advice, religious authority, or crisis support.

DLAS remains a conceptual future runtime family and architecture subject. Its definition, scope, and authority remain unresolved; it is not treated as live or specified by this document.

### Domain Responsibility Matrix

| Responsibility | Governance repository | `meuus.org` | `meuussoul.com` | `meuus.app` |
| --- | --- | --- | --- | --- |
| Preserve governed architecture record and architectural judgment | Owns architecture record within inherited authority | Does not own | Does not own | Does not own |
| Express approved institutional truth publicly | Governs applicable boundaries | Owns public expression | May supply canonical source material | May display approved contextual boundaries |
| Preserve canonical knowledge and provenance | Governs applicable boundaries | May summarize with provenance | Owns canonical knowledge role | May use approved knowledge contextually |
| Hold private reflection and journey context | Does not own | Does not own | Does not own private runtime data | Owns runtime role within future approved boundaries |
| Produce runtime observations or evidence | Does not produce runtime evidence | Does not own production | May receive reviewed candidate evidence | May produce candidate evidence |
| Approve architectural change | Owns governed architecture process | Cannot approve | Cannot approve | Cannot approve |
| Establish operational status claims | Defines taxonomy and governance constraints | Expresses only approved claims | Reports evidence within its scope | Reports evidence within its scope |

"Owns" identifies conceptual responsibility, not present operational capability. Every current-state claim remains subject to evidence and the status taxonomy.

### Domain Boundary Rules

1. A domain may not acquire another domain's authority merely because it stores, displays, links to, summarizes, or uses that domain's material.
2. Public expression does not create institutional, canonical, or architectural truth.
3. Canonical knowledge does not create governance authority.
4. Runtime behavior, frequency, popularity, or personalization does not create canonical knowledge.
5. Implementation evidence may inform review but cannot silently amend a Frozen document.
6. Private reflection remains within its approved runtime boundary unless an explicit, consent-respecting review path is later established.
7. A status claim must travel with its evidence boundary; it may not become stronger when repeated by another domain.
8. Cross-domain movement transfers a permitted representation or evidence item, not ownership of the originating responsibility.

### Allowed Movement

The following conceptual movement is allowed when the source and status remain clear:

- Frozen governance and architecture constraints may be inherited by public, knowledge, and runtime domains.
- Approved institutional truth may be expressed by `meuus.org`.
- Public orientation may point toward canonical knowledge or an approved runtime surface.
- Canonical knowledge may be summarized by `meuus.org` with preserved meaning and provenance.
- Approved canonical knowledge may inform contextual runtime guidance.
- Runtime systems may present approved institutional boundaries and status notices.
- A domain may report evidence about its own current state for later verification.

Allowed movement does not itself verify the receiving system, authorize implementation, or transfer authority.

### Forbidden Movement

The following conceptual movement is forbidden:

- Private reflection or journey data moving directly into public institutional content.
- Private reflection becoming canonical knowledge without an approved review, provenance, privacy, and consent basis.
- Runtime output becoming governance policy or architecture automatically.
- Runtime-generated suggestions being represented as canonical truth.
- Public summaries replacing or silently altering canonical knowledge.
- Canonical knowledge being used to claim governance authority.
- Implementation choices being promoted into architecture without the governance process.
- Planned, Future, Not live, or unverified capabilities being relabeled as Verified or operational without evidence.
- One domain silently taking ownership of another domain's responsibility.

### Review-Gated Movement

The following movement requires explicit review by the authority appropriate to the proposed change:

- Runtime observations proposed as candidate knowledge.
- Candidate knowledge proposed for canonical status.
- Canonical knowledge proposed for institutional public expression where meaning, risk, or status could change.
- Runtime evidence proposed as a reason for architectural or governance change.
- A change to a public operational-status claim.
- Reuse of private or aggregated reflection evidence outside its original approved boundary.
- A new cross-domain responsibility or a transfer of ownership between domains.
- Any claim that would broaden an Existing, Verified, Planned, Future, or Not live classification.

Review-gated movement remains a proposal until approved. Movement through review does not bypass higher authority or the Freeze Rule.

### Status and Evidence Movement

Status and evidence move differently from authority:

- **Authority** is inherited downward from higher-authority documents.
- **Status** is a bounded claim about a document, system, capability, or relationship.
- **Evidence** may be submitted upward or across domains for review.
- **Approval** determines whether reviewed evidence may change an authoritative or canonical claim.

The following rules apply:

1. Evidence must retain its source, scope, date, and limitations when it moves.
2. A receiving domain may not broaden a claim beyond the evidence supplied.
3. Repetition across domains does not increase confidence or authority.
4. Existing does not mean Verified or live.
5. Planned and Future do not mean Existing.
6. Not live must not be represented as operational.
7. Unverified status remains unverified until reviewed against discoverable evidence.
8. Evidence that conflicts with a Frozen document must trigger review; it does not directly rewrite the document.

### Topology States

The topology inherits the truth taxonomy established in `01_master_architecture.md`.

| State | Topology meaning |
| --- | --- |
| Existing | The domain, artifact, or relationship is known to exist; completeness and operation are not implied. |
| Verified | The specific topology claim has been checked against discoverable evidence. |
| Planned | The topology role or relationship is an explicit intention but is not represented as operational. |
| Future | The role, relationship, or capability belongs to a possible later topology. |
| Not live | The system or relationship is explicitly unavailable as an operational public service at the time of the claim. |

Current classifications inherited from Frozen Document 01:

| Domain | Inherited classification | Evidence limit |
| --- | --- | --- |
| `meuus-architecture-governance` | Existing; Verified within its repository | Verification does not extend to implementation domains. |
| `meuus.org` | Existing as an established domain | Present public capabilities and live status are not Verified here. |
| `meuussoul.com` | Planned canonical knowledge and learning domain | Full platform existence and operation are not Verified here. |
| `meuus.app` | Existing as an established domain; later runtime roles are Future | Phase Zero operation and live status are not Verified here. |

This Working document does not strengthen those classifications.

### Public-to-Knowledge Relationship

`meuus.org` may orient the public toward books, learning materials, previews, and canonical knowledge maintained by `meuussoul.com`.

The relationship is constrained as follows:

- Public summaries must preserve the meaning and status of the canonical source.
- A summary must not replace canonical depth or provenance.
- Public accessibility does not grant the institutional surface ownership of canonical knowledge.
- If the public expression and canonical source diverge, the discrepancy requires review and correction.
- The existence of a public link or preview does not prove that the full knowledge platform is operational.

### Knowledge-to-Runtime Relationship

Approved canonical knowledge may inform reflection, journeys, responsible next steps, and future action systems.

The relationship must preserve distinctions among:

- Canonical knowledge.
- Contextual guidance.
- User-authored reflection.
- Runtime-generated suggestions.

Runtime adaptation does not alter the canonical source. A runtime must not present personalization, inference, or generated guidance as canonical truth.

### Runtime-to-Governance Evidence Path

Runtime evidence may inform knowledge or governance only through an explicit path:

1. The runtime produces an observation or candidate evidence item within its approved boundary.
2. The item remains evidence, not authority.
3. Its source, scope, limitations, privacy boundary, and provenance must be identified.
4. The relevant knowledge or governance authority reviews the proposed use.
5. If a Frozen architectural change is proposed, the Freeze Rule applies.
6. Only an approved decision may change canonical knowledge, public institutional truth, or architecture.

This path is conceptual. It does not define collection, storage, transmission, aggregation, or processing mechanics.

### Separation Rules

The following separations must remain visible:

- Foundational assumptions remain above architecture.
- Governance remains separate from implementation.
- Public institutional expression remains separate from canonical knowledge ownership.
- Canonical knowledge remains separate from runtime personalization.
- Runtime reflection remains separate from public institutional content.
- Private user context remains separate from public and canonical contexts.
- Evidence remains separate from approval.
- Status remains separate from aspiration.
- A cross-domain relationship remains separate from a transfer of responsibility.

### Matters Reserved for Later Documents

This document does not determine:

- Detailed domain-specific responsibility inventories.
- Content representation and provenance requirements.
- Status verification procedures or review cadence.
- Privacy, consent, retention, or aggregation rules.
- Technical system, network, data, or deployment topology.
- Identity, authentication, authorization, or payment architecture.
- Runtime mechanics or product behavior.
- The definition or internal architecture of DLAS.
- The existence or design of shared implementation capabilities.

Reserving these matters prevents this topology document from absorbing later architecture or implementation work.

---

## Authority

This document is subordinate to:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.

While its status is Working, it may be referenced as a developing architecture document but is not canonical and remains subject to change.

This document cannot:

- Modify or reinterpret a Frozen dependency.
- Grant itself Frozen status.
- Transfer authority among domains.
- Authorize implementation work.
- Begin or authorize Document 03.

---

## Inputs

The inputs to this Working document are:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- Documented Founder directives relevant to ecosystem topology.
- Discoverable evidence where a present-state topology claim is required.

Implementation state may provide evidence about what exists. It does not determine architectural authority or silently redefine topology.

---

## Outputs

If reviewed and Frozen through the governance lifecycle, this document is intended to provide:

- A canonical conceptual topology for the four principal domains.
- A domain responsibility matrix.
- Allowed, forbidden, and review-gated movement rules.
- Status and evidence movement constraints.
- Separation rules for later architecture documents.
- An explicit boundary between ecosystem topology and later architectural concerns.

At Working status, these outputs are substantially developed but remain non-canonical.

---

## Dependencies

This document depends on:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.

It inherits the authority hierarchy, domain roles, truth taxonomy, evidence discipline, and unresolved boundaries established by those documents.

If this document appears to conflict with a Frozen dependency, the Frozen dependency governs and the conflict must be documented for review. No later document acquires authority merely by depending on this Working document.

---

## Interfaces

The interfaces below are conceptual topology relationships, not technical interfaces.

### Governance and Public Institution

Governance constrains what `meuus.org` may claim institutionally. Public expression may communicate approved governance status but cannot change it.

### Governance and Knowledge

Governance constrains the use and authority of canonical knowledge. `meuussoul.com` may preserve knowledge and provenance but cannot create governance decisions.

### Governance and Runtime

Governance constrains runtime purpose, claims, and boundaries. Runtime evidence may inform review but cannot amend governance automatically.

### Public Institution and Knowledge

`meuus.org` may orient people toward canonical knowledge and summarize it within approved provenance and truth boundaries. `meuussoul.com` retains the canonical knowledge role.

### Knowledge and Runtime

Approved knowledge may inform runtime context. Runtime adaptation, personalization, and user reflection remain distinct from canonical content.

### Public Institution and Runtime

`meuus.org` may orient people toward an approved runtime and communicate its verified status. The runtime may display approved institutional boundaries but cannot make institutional claims independently.

### Runtime Evidence and Review

Runtime evidence may be proposed to knowledge or governance through explicit review. The relationship does not permit direct promotion into canonical or architectural authority.

---

## Questions Unresolved

- What is the minimum set of topology views needed to make this document explainable without adding implementation detail?
  - **Disposition:** Deferred to Architecture Review.
- What artifact categories require explicit provenance when moving between public, knowledge, and runtime domains?
  - **Disposition:** Deferred to later architecture document.
- What evidence threshold should govern promotion of runtime observations into candidate knowledge?
  - **Disposition:** Deferred to later architecture document.
- What privacy and consent authority is required before private or aggregated reflection evidence may leave its original runtime boundary?
  - **Disposition:** Deferred to Founder Review.
- How should a topology status be re-verified when its evidence becomes outdated?
  - **Disposition:** Deferred to later architecture document.
- How should external institutions or future ecosystem domains be represented without weakening the four-domain topology?
  - **Disposition:** Requires evidence before resolution.
- Should any capability be classified as shared across domains, and how would shared use avoid creating shared authority?
  - **Disposition:** Deferred to later architecture document.
- What additional topology claim, if any, is required before this document can move to Ready for Review?
  - **Disposition:** Deferred to Architecture Review.

These questions remain explicit and bounded. Their dispositions identify where resolution belongs without authorizing another document or resolving uncertainty by assumption.

---

## Risks

### Duplication of the Master Architecture

Risk: this document could restate Document 01 instead of refining topology.

Response: retain Document 01 as the authority for ecosystem roles and use this document only for placement, movement, and separation.

### Authority Drift

Risk: cross-domain movement could be mistaken for transfer of responsibility or authority.

Response: distinguish movement of representations and evidence from ownership and approval.

### Operational Overclaiming

Risk: Planned, Future, Not live, or unverified topology could be described as operational.

Response: inherit Document 01 classifications and prevent stronger claims without evidence.

### Implementation Leakage

Risk: conceptual topology could become a technical architecture or data-flow specification.

Response: exclude technologies, protocols, schemas, storage, transmission, processing, and deployment mechanics.

### Privacy Boundary Failure

Risk: private runtime reflection could move into public, canonical, or governance contexts without an approved basis.

Response: forbid direct movement and require future privacy, consent, provenance, and review authority.

### Knowledge Dilution

Risk: public summaries or runtime adaptations could replace or distort canonical knowledge.

Response: preserve provenance, canonical ownership, and the distinction between source, summary, and contextual use.

### Excessive Centralization

Risk: this document could absorb domain responsibilities or later architectural decisions.

Response: reserve detailed responsibility, provenance, privacy, status, and runtime matters for later documents.

### Ambiguous Review Gates

Risk: contributors may treat the phrase "explicit review" as sufficient without identifying the proper authority.

Response: keep review authority unresolved where it has not been approved and require later documents to make it discoverable.

---

## Non-goals

This document does not:

- Modify Book Zero, `00_READ_FIRST.md`, `README.md`, or `01_master_architecture.md`.
- Create new foundational, governance, or architectural principles.
- Select technologies, frameworks, vendors, or hosting.
- Define databases, APIs, schemas, protocols, or technical data flows.
- Define UI, authentication, payments, analytics, or deployment.
- Define runtime implementation, product features, or application state.
- Define privacy, consent, retention, or legal mechanisms.
- Define pricing or marketing claims.
- Fully define DLAS or represent it as operational.
- Establish shared services or shared implementation ownership.
- Authorize implementation work.
- Begin, create, or authorize Document 03.

---

## Review Criteria

Before this document may move from Working to Ready for Review, reviewers should confirm:

### Constitutional and Governance Integrity

- It remains subordinate to all declared dependencies.
- It does not modify, reinterpret, or contradict a Frozen document.
- Every unresolved architectural question remains visible.

### Structural Integrity

- The four principal domains remain distinct and non-overlapping.
- The responsibility matrix reflects Document 01 without replacing it.
- Allowed, forbidden, and review-gated movement are clear.
- Authority, status, evidence, and approval remain distinguishable.
- Matters reserved for later documents remain outside this scope.

### Truthfulness

- No claim exceeds its evidence.
- Existing, Verified, Planned, Future, and Not live are used conservatively.
- No future or unverified system is represented as operational.
- Cross-domain repetition does not strengthen a claim.

### Implementation Independence

- No technology, framework, vendor, database, API, schema, UI, deployment, or runtime mechanism is embedded.
- Conceptual paths cannot be mistaken for technical data flows.

### Maintainability

- A future contributor can understand the topology without prior Founder conversation.
- The document remains explainable and no more complex than necessary.
- Later architecture can refine bounded concerns without silently changing this topology.

### Lifecycle Readiness

- All required sections are substantially complete.
- Dependencies and non-goals remain explicit.
- Unresolved questions are resolved or explicitly accepted for formal review.
- Founder Review and Architecture Review have not been presumed.
