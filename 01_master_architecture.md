Document: 01_master_architecture.md
Title: meUus Ecosystem Master Architecture
Status: Working
Authority: Architectural Authority
Version: 0.1
Depends on:
- Book Zero
- 00_READ_FIRST.md
- README.md
Supersedes: None
Purpose: Define the conceptual master architecture map for the meUus ecosystem.
Last Updated: 2026-07-09
Reviewed by:
- Founder: N
- Architecture: N

---

## Purpose

This document defines the conceptual master architecture map for the meUus ecosystem.

It establishes the roles, boundaries, relationships, and authority flow among:

- `meuus-architecture-governance`
- `meuus.org`
- `meuussoul.com`
- `meuus.app`

It gives future contributors a shared map for understanding where governance, institutional expression, canonical knowledge, and runtime action belong. It also provides the architectural dependency point from which later architecture documents may inherit after this document completes the governance lifecycle.

This is a Working document. Its content is substantially complete but remains subject to Founder Review and Architecture Review. It is not Frozen and must not be cited as canonical Architectural Authority.

---

## Scope

This document covers:

- The conceptual topology of the principal meUus domains and repositories.
- The responsibility and exclusion boundaries of each domain.
- The flow of authority from governance into public, knowledge, and runtime systems.
- The movement of approved truth among institutional, knowledge, and runtime contexts.
- The distinction between existing, verified, planned, future, and not-live systems.
- The conditions under which runtime evidence may inform later knowledge or governance review.
- The inheritance relationship between this document and later architecture documents.
- Risks and unresolved questions that could affect the ecosystem-wide architecture.

This document defines ownership and relationships at the ecosystem level. It does not specify how any system is implemented.

### Master Topology

The ecosystem is organized into four distinct architectural domains:

| Domain | Primary role | Authority or responsibility | Explicit boundary |
| --- | --- | --- | --- |
| `meuus-architecture-governance` | Constitutional and architecture authority | Preserves institutional judgment and governs architecture documents | Contains no application code, UI, runtime behavior, APIs, databases, deployment configuration, or product features |
| `meuus.org` | Public institutional foundation | Expresses approved public truth, status boundaries, Amanah, orientation, public trust, book preview links, and institutional explanation | Does not own runtime reflections, canonical knowledge depth, or private user journeys |
| `meuussoul.com` | Canonical knowledge and learning platform | Preserves books, learning materials, source-of-truth knowledge, provenance, and structured learning | Does not make institutional governance decisions or own private runtime reflection data |
| `meuus.app` | Reflection, Journey, and action runtime | Supports reflection and responsible action within approved boundaries | Does not assert canonical truth or replace professional, religious, therapeutic, diagnostic, legal, or crisis authority |

These domains are separate so that no implementation surface silently acquires governance, institutional, or canonical knowledge authority merely by publishing content or operating software.

### Ecosystem Roles

#### `meuus-architecture-governance`

`meuus-architecture-governance` is the constitutional and architecture authority repository for the ecosystem.

It preserves the approved reasoning, dependencies, boundaries, and unresolved questions that future contributors need in order to act consistently. It governs architecture; it does not implement the systems it governs.

It does not contain:

- Application or website code.
- User interfaces.
- Runtime behavior.
- APIs or database structures.
- Deployment or infrastructure configuration.
- Product features.

#### `meuus.org`

`meuus.org` is the public institutional foundation of the meUus ecosystem.

Its role is to express approved public truth and explain the institution faithfully. Its responsibilities include public status boundaries, Amanah, orientation, public trust, institutional explanation, and appropriate links or previews for books and learning resources.

It does not own:

- Private reflection or journey data.
- Runtime user actions.
- The full canonical depth of books or structured knowledge.
- Governance decisions merely because they are publicly expressed there.

Its public statements must remain traceable to approved authority and evidence. Publication does not create constitutional or architectural authority.

#### `meuussoul.com`

`meuussoul.com` is the canonical knowledge and learning platform.

Its role is to preserve and present books, learning materials, source-of-truth knowledge, provenance, and structured learning. It provides knowledge depth that a public institutional surface or runtime application should not duplicate or silently redefine.

It does not:

- Make constitutional, governance, or architecture decisions.
- Own private runtime reflection data.
- Convert runtime observations into canonical knowledge without explicit review.
- Acquire institutional authority merely by preserving canonical content.

#### `meuus.app`

`meuus.app` is the Reflection, Journey, and action runtime.

Its Phase Zero role is a browser-local reflection prototype. This statement defines the approved role boundary; any claim about the prototype's present operational state still requires verification.

Its future role may include user journeys, reflection artifacts, responsible next steps, DLAS runtime, and other action systems only after governance approval. Future roles are not live capabilities and must not be represented as operational before verification.

`meuus.app` does not:

- Assert or redefine canonical truth.
- Make governance decisions.
- Replace therapy, diagnosis, legal advice, professional advice, religious authority, or crisis support.
- Promote private runtime evidence into institutional or canonical knowledge without explicit review.

### Truth and Status Taxonomy

Every architecture or public claim about a system, capability, artifact, or relationship must use language appropriate to its evidence and status.

| Term | Meaning |
| --- | --- |
| Existing | The named artifact or system is presently known to exist. Existence alone does not prove that it is complete, public, operational, or verified. |
| Draft | The document or proposal is exploratory and is not authoritative. |
| Working | The content is substantially complete but remains subject to change and formal review. |
| Verified | The specific claim has been checked against current, discoverable evidence. Verification applies only to the claim and evidence examined. |
| Planned | The work is an explicit intention or approved direction but is not represented as operational. |
| Future | The capability or system belongs to a possible later state and carries no claim of present availability. |
| Not live | The capability or system is explicitly unavailable as an operational public service at the time of the claim. |

These terms must not be treated as interchangeable. In particular:

- Existing does not automatically mean Verified or live.
- Planned and Future do not mean Existing.
- Draft and Working describe maturity without granting Frozen authority.
- A system described as Not live must not be presented elsewhere as operational.

When current evidence is insufficient, the architecture must use the less expansive claim. Claim must never exceed evidence.

---

## Authority

This document is subordinate to:

1. Book Zero as Foundational Authority.
2. `00_READ_FIRST.md` as Governance Authority.
3. `README.md` as Frozen Governance Orientation.

This document is classified under Architectural Authority. While its status is Working, it can be referenced as a developing architecture document but is not canonical and remains subject to change.

This document cannot:

- Modify Foundational Authority or Governance Authority.
- Grant itself Frozen status.
- Authorize implementation merely by describing a future relationship.
- Give an implementation repository the power to redefine architecture.
- Resolve constitutional questions that belong to Book Zero.

### Governing Principles

The master architecture applies the following inherited and Founder-directed principles:

- **Claim <= Evidence.** No claim may exceed its discoverable support.
- **Governance before implementation.** Authority and boundaries must be established before implementation acts on them.
- **Architecture before runtime.** Runtime behavior must inherit approved architectural intent.
- **Knowledge before action.** Responsible action should be grounded in appropriate, reviewed knowledge.
- **Amanah before marketing.** Entrusted truth and responsibility take priority over promotional advantage.
- **No silent contradiction.** Apparent conflicts with higher authority must be documented and resolved.
- **Preserve existing truth.** Existing truthful work should be improved before replacement.
- **Preserve judgment.** Architecture exists to preserve judgment, not merely structure.

These principles establish decision boundaries; they do not prescribe implementation choices.

### Authority Flow

Authority flows downward:

1. Book Zero establishes foundational assumptions.
2. `00_READ_FIRST.md` establishes governance rules.
3. Frozen architecture documents establish approved conceptual boundaries.
4. Implementation specifications interpret those boundaries within their proper repositories.
5. Code, content presentation, configuration, and runtime behavior execute approved specifications.

Lower-authority systems may provide evidence upward, but they do not acquire higher authority by doing so. Evidence can inform review; it cannot silently amend governance, architecture, or canonical knowledge.

---

## Inputs

The discoverable inputs to this Working document are:

- Book Zero as Foundational Authority.
- `00_READ_FIRST.md` as Governance Authority.
- `README.md` as Governance Orientation.
- Documented Founder directives and approved review decisions.
- Verified repository state where a present-state claim is required.
- Explicitly identified evidence relevant to ecosystem roles and boundaries.

Later review must distinguish inherited authority from contextual evidence. A current implementation may demonstrate what exists, but it does not determine what the architecture ought to authorize.

---

## Outputs

When reviewed and Frozen, this document is intended to provide:

- The master conceptual map of the meUus ecosystem.
- Stable responsibility and exclusion boundaries for each principal domain.
- A shared truth and status taxonomy for architectural claims.
- The authority flow from governance to architecture and implementation.
- The conceptual movement of approved truth into public, knowledge, and runtime contexts.
- The governed feedback path by which runtime evidence may be reviewed.
- A dependency anchor for later architecture documents.
- Explicit non-goals, risks, and unresolved questions that constrain later work.

This document does not itself create, launch, verify, or authorize any implementation capability.

---

## Dependencies

This document depends on:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.

The dependency order is constitutional, not merely editorial. If this document appears to conflict with a higher-authority dependency, the higher authority governs and the conflict must be documented for review.

### Inheritance by Later Documents

Later architecture documents should:

- Declare this document as a dependency where their scope derives from the master topology.
- Preserve the ecosystem roles and exclusion boundaries defined here once this document is Frozen.
- Refine one bounded architectural concern without silently redefining another domain.
- Carry forward the truth and status taxonomy.
- Keep unresolved matters open unless resolved through discoverable evidence and the governance process.
- Record any proposed conflict rather than silently overriding this document.

No later document derives canonical authority from this Working draft. Formal inheritance begins only after the relevant documents pass their required governance lifecycle.

---

## Interfaces

The interfaces in this section are conceptual relationships. They are not technical APIs, protocols, payloads, schemas, or deployment instructions.

### Governance to Ecosystem

Governance defines approved authority, architectural boundaries, review status, and constraints. Each ecosystem domain must be able to trace consequential claims and responsibilities to the authority appropriate for them.

Governance is not a content delivery service or runtime dependency. Its role is to preserve the judgment that those systems must inherit.

### Governance to Public Institution

Approved institutional truth may be expressed publicly through `meuus.org`.

`meuus.org` may explain governance status and institutional commitments, but its publication layer does not alter the governing source. If the public expression and governing source diverge, the discrepancy must be documented and corrected through the appropriate authority.

### Governance and Knowledge

Governance establishes the boundaries within which canonical knowledge is preserved and used. `meuussoul.com` preserves knowledge and provenance but does not create governance authority.

Knowledge may inform architectural review when its source, status, and relevance are discoverable. It does not silently amend Frozen documents.

### Knowledge to Public Institution

`meuus.org` may orient the public toward approved books, learning resources, or previews. Canonical depth and provenance remain with `meuussoul.com`.

Public summaries must not overstate, distort, or replace the canonical source. Where the two differ in depth, the canonical source governs the knowledge claim while governance governs whether and how the institution may represent it.

### Knowledge to Runtime

Approved knowledge may inform reflection, journeys, responsible next steps, and future action systems in `meuus.app`.

The runtime must preserve the distinction between:

- Canonical knowledge.
- Contextual guidance.
- User-authored reflection.
- Runtime-generated suggestions.

Runtime presentation or personalization does not create canonical truth.

### Public Institution to Runtime

`meuus.org` may orient people toward an approved runtime experience and explain its verified status and boundaries.

It must not represent a planned, future, or not-live runtime as operational. `meuus.app` must not use its runtime role to make institutional claims outside approved public truth.

### Runtime Evidence to Knowledge and Governance

Runtime activity may produce observations, feedback, or other evidence that could later inform knowledge or governance.

That movement is review-gated:

1. Runtime evidence remains evidence, not authority.
2. Private reflection data remains within its approved privacy and ownership boundary.
3. Any candidate insight must be separated from personal or unsupported inference.
4. The relevant knowledge or governance authority must review provenance, evidence, limitations, and proposed use.
5. Only explicit approval may change canonical knowledge or architectural authority.

No automated, popular, frequent, or commercially useful runtime outcome may silently become canonical knowledge or governance policy.

### Conceptual Truth Flow

The intended flow is:

1. Governance preserves approved judgment and boundaries.
2. The public institution expresses approved institutional truth.
3. The knowledge platform preserves canonical depth, learning structure, and provenance.
4. The runtime supports reflection and responsible action within those boundaries.
5. Runtime evidence may return for explicit knowledge or governance review without acquiring authority on its own.

This is a flow of responsibility and review, not a prescribed technical data flow.

---

## Questions Unresolved

The following questions remain open and must not be resolved through implementation assumptions:

- What Founder-approved evidence is required to classify the Phase Zero browser-local reflection prototype as Existing, Verified, or Not live?
- Which specific institutional statements belong only on `meuus.org`, and which may be reproduced with provenance on other surfaces?
- What review authority and evidence threshold should govern promotion of runtime observations into candidate knowledge?
- What privacy and consent principles must be established before any private runtime reflection may contribute to aggregated evidence?
- What is the approved conceptual definition and scope of DLAS before any later architecture document treats it as a runtime family?
- Which later architecture documents should inherit directly from this master document, and in what approved order?
- Which terms require inclusion in the future glossary to prevent differing interpretations across repositories?
- What mechanism should identify and reconcile status differences when a claim is verified at one time but later becomes outdated?
- What minimum provenance must accompany canonical knowledge when it is summarized by `meuus.org` or used contextually by `meuus.app`?

These questions do not prevent Working status because they are explicit and bounded. They must be resolved or formally deferred before this document is considered Ready for Review.

---

## Risks

### Authority Drift

An implementation or publishing surface could begin making governance, institutional, or canonical claims outside its role.

Architectural response: preserve explicit ownership boundaries and require review for upward changes in authority.

### Operational Overclaiming

Planned or future capabilities could be described as existing or live.

Architectural response: apply the truth and status taxonomy and require evidence appropriate to each claim.

### Knowledge Dilution

Summaries or runtime adaptations could become detached from canonical knowledge and provenance.

Architectural response: preserve traceability to `meuussoul.com` and keep adaptation distinct from canonical source material.

### Runtime Authority Inflation

Personalization, user activity, or repeated runtime outcomes could be mistaken for canonical truth or institutional judgment.

Architectural response: treat runtime outputs as contextual artifacts or evidence subject to explicit review.

### Privacy Boundary Failure

Private reflection data could move into public, knowledge, or governance contexts without an approved basis.

Architectural response: preserve private runtime ownership and leave evidence use unresolved until privacy, consent, and provenance authority are explicitly established.

### Implementation Leakage

Current technologies or product mechanics could become embedded in long-lived architecture.

Architectural response: define conceptual responsibilities and interfaces only; place implementation choices in their proper repositories and specifications.

### Premature Dependency

Later documents could treat this Working draft as Frozen authority.

Architectural response: require explicit status awareness and prohibit canonical inheritance until governance approval is complete.

### Excessive Centralization

The master architecture could expand until it absorbs decisions that belong to bounded later documents.

Architectural response: retain only ecosystem-level roles, boundaries, flows, and dependencies here.

---

## Non-goals

This document does not:

- Define or select a technology stack, framework, language, vendor, or hosting platform.
- Define backend architecture, databases, schemas, APIs, endpoints, analytics, or infrastructure.
- Define authentication, payment, or deployment mechanisms.
- Define UI components, screen behavior, or implementation instructions.
- Define pricing, commercial strategy, or marketing claims.
- Establish therapy, diagnostic, legal, professional, religious, or crisis authority.
- Specify the content of books, learning materials, or personal reflections.
- Decide privacy or consent mechanisms before the appropriate authority and evidence exist.
- Assert that planned or future systems are live.
- Modify Book Zero, `00_READ_FIRST.md`, or `README.md`.
- Replace the governance lifecycle or Decision Register process.
- Authorize implementation work.
- Begin, create, or authorize Document 02.

---

## Review Criteria

Before this document may move to Ready for Review, reviewers should confirm:

### Constitutional Integrity

- The document remains consistent with Book Zero.
- It inherits the governance rules in `00_READ_FIRST.md`.
- It does not reinterpret or amend any Frozen document.
- Every architectural decision has a discoverable reason or is identified as unresolved.

### Structural Integrity

- Each principal domain has one clear primary role and explicit exclusions.
- Governance, institution, knowledge, and runtime remain conceptually distinct.
- Authority flows downward while evidence returns upward only through explicit review.
- Later document inheritance is clear without pre-authorizing later documents.

### Truthfulness

- Existing, Draft, Working, Verified, Planned, Future, and Not live are clearly distinguished.
- No future system or capability is implied to be operational.
- Claims remain no broader than their evidence.
- Unresolved questions remain visible.

### Maintainability

- The architecture is independent of current technology choices.
- A future contributor can understand the topology without prior Founder conversation.
- The document remains explainable and no more complex than necessary.
- Existing truthful work is preserved before replacement.

### Institutional Readiness

- `meuus.org` faithfully owns public institutional expression without absorbing canonical knowledge or runtime responsibilities.
- `meuussoul.com` faithfully owns canonical knowledge and learning without acquiring governance or private runtime authority.
- `meuus.app` faithfully owns reflection, Journey, and action runtime without asserting canonical or professional authority.
- Amanah and evidence govern public representation before marketing advantage.

### Lifecycle Readiness

- All required sections are substantially complete.
- Dependencies and status are accurate.
- Remaining questions are resolved or explicitly accepted for formal review.
- Founder Review and Architecture Review have not been presumed.
- The document is not marked Frozen before approval.
