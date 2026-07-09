Document: 05_evidence_status_and_truth_taxonomy.md
Title: meUus Evidence, Status, and Truth Taxonomy
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
- 04_authority_flow_and_decision_rights.md
Supersedes: None
Purpose: Define how evidence, status labels, and truth claims are classified, constrained, reviewed, and communicated across the meUus ecosystem.
Last Updated: 2026-07-09
Reviewed by:
- Founder: N
- Architecture: N

---

## Purpose

This document defines the conceptual taxonomy for evidence, status labels, verification, uncertainty, and truth claims across the meUus ecosystem.

Its core doctrine is:

```text
Claim <= Evidence
```

A claim must never be broader, stronger, newer, or more certain than the evidence that supports it.

This is a Ready for Review document. Its sections are complete enough for Founder Review and Architecture Review. It is not Frozen, is not canonical, and must not be treated as authority for implementation or public claims.

---

## Scope

This document defines:

- The distinction among truth, claim, evidence, status, verification, uncertainty, and aspiration.
- Evidence categories and evidence-boundary requirements.
- Status labels and verification levels.
- Claim-strength rules for public, architectural, canonical, and runtime contexts.
- Rules for operational status.
- Treatment of missing, outdated, conflicting, and unverifiable evidence.
- Prohibited claim categories.
- Escalation requirements before expression or authority change.

It does not determine whether any particular implementation capability is presently operational. It does not strengthen the current classifications inherited from Frozen Documents 01-04.

### Taxonomy Overview

The conceptual relationship is:

```text
Truth
  is not created by a claim

Evidence
  supports or limits a claim

Claim
  describes only what evidence can support

Status
  communicates a bounded state of a document, artifact,
  system, capability, or claim

Review
  evaluates evidence and the proposed use of a claim

Approval
  authorizes a bounded use; it does not create truth
```

Publication, repetition, runtime frequency, popularity, analytics, market pressure, user demand, or institutional preference cannot create truth or authority.

### Truth, Claims, Evidence, and Status

| Term | Meaning |
| --- | --- |
| Truth | What is real or correct independently of preference; this architecture does not create or fully adjudicate foundational truth |
| Claim | A statement presented for internal, architectural, canonical, runtime, or public use |
| Evidence | Discoverable support or contradiction relevant to a specific claim |
| Status | A bounded label describing document maturity, artifact state, system state, capability state, or review state |
| Verification | A scoped act of checking a specific claim against identified evidence |
| Uncertainty | An explicit limit in knowledge, evidence, interpretation, freshness, or authority |
| Aspiration | A desired direction that is not evidence of commitment, existence, or operation |
| Proposal | A candidate claim or change awaiting review |
| Approval | A bounded authorization granted by the appropriate authority |

Truth is not reduced to available evidence. Evidence limits what meUus may responsibly claim.

### Core Taxonomy Rules

1. Claim must not exceed evidence.
2. Evidence is not truth, authority, approval, or certainty by itself.
3. A status label must name what it describes.
4. Verification must name the claim, evidence, scope, time, and limitations.
5. Public visibility does not prove operation.
6. Repository presence does not prove runtime capability.
7. Review does not broaden evidence.
8. Frozen or canonical status does not prove empirical or operational truth.
9. Missing evidence remains missing evidence.
10. Conflicting evidence lowers confidence and triggers review.
11. Outdated evidence cannot support a current claim without rechecking.
12. Private user reflection is not public, canonical, institutional, or governance truth.
13. Runtime evidence remains evidence, not authority.
14. Repetition across domains does not strengthen a claim.
15. Unknown must not be rewritten as false, true, live, or not live without evidence.

### Evidence Categories

Evidence categories describe source context. They do not create constitutional authority.

| Category | Conceptual meaning | Primary limit |
| --- | --- | --- |
| Foundational-source evidence | Material cited by or relevant to Foundational Authority | Architecture cannot use it to redefine Book Zero |
| Governance evidence | Frozen governance text, approved governance decisions, and governed review records | Proves the recorded governance state, not implementation operation |
| Architectural evidence | Frozen architecture text, dependencies, decisions, and review records | Proves approved architecture, not that implementation exists |
| Repository evidence | Directly inspectable files, commits, tags, releases, or repository state | Proves only the inspected repository facts |
| Public-expression evidence | Directly inspectable public statements or surfaces | Proves visibility and wording, not truth or operational capability |
| Canonical-knowledge evidence | Sources, provenance, reviewed knowledge records, and explicit uncertainty | Canonical status process remains unresolved |
| Runtime evidence | Observations or artifacts produced within a runtime boundary | Cannot promote itself into authority or canonical truth |
| Operational evidence | Direct evidence that a specific capability operated under stated conditions | Applies only to the capability, conditions, and time checked |
| User-authored evidence | A person's own reflection, statement, or artifact | Remains contextual and private unless an approved boundary permits otherwise |
| External evidence | Evidence originating outside meUus | Source authority, independence, scope, and freshness require review |
| Historical evidence | Evidence of a past state or decision | Does not prove current state |
| Missing evidence | Required support that is absent or unavailable | Supports no stronger claim |
| Conflicting evidence | Evidence items that support incompatible conclusions | Requires review and explicit uncertainty |
| Outdated evidence | Evidence no longer sufficiently current for the proposed claim | Requires rechecking before current use |

No category is automatically stronger than another. Strength depends on relevance, scope, provenance, freshness, limitations, and the claim being evaluated.

### Evidence Boundary Requirements

Every evidence item used for a consequential claim should retain:

| Boundary field | Required meaning |
| --- | --- |
| Source | Where or from whom the evidence originated |
| Claim supported | The exact claim the evidence is being used to support or challenge |
| Scope | What system, document, capability, population, condition, or period the evidence covers |
| Observed date | When the evidence was observed, recorded, or reviewed |
| Freshness | Whether the evidence remains current enough for the proposed claim |
| Provenance | How the evidence relates to its source and whether transformations occurred |
| Limitations | What the evidence cannot establish |
| Authority relationship | Which authority or responsibility context governs its use; evidence itself owns no authority |
| Review state | Unreviewed, reviewed, disputed, approved for bounded use, or otherwise unresolved |
| Public suitability | Whether the evidence may support public expression and under what qualification |
| Privacy boundary | Whether the evidence contains private or user-authored material |

If a required boundary is unknown, that uncertainty must travel with the evidence.

### Status Label Taxonomy

Status labels fall into different families. A label from one family must not be treated as a label from another.

#### Governance Lifecycle Status

These statuses are governed by `00_READ_FIRST.md`:

| Status | Meaning |
| --- | --- |
| Draft | Exploratory and non-authoritative |
| Working | Substantially complete but subject to change |
| Ready for Review | Declared complete and awaiting formal review |
| Frozen | Approved and canonical within the document's authority and scope |
| Retired | Historical and no longer authoritative |

"In review" may describe current activity, but it is not a replacement for the formal lifecycle status.

#### System and Capability Status

| Status | Meaning |
| --- | --- |
| Existing | The named artifact, domain, system, or capability is known to exist; completeness and operation are not implied |
| Verified | The specific claim has been checked against identified evidence; verification scope must be stated |
| Planned | An explicit intended direction; existence and operation are not implied |
| Future | A possible later state; commitment, existence, and operation are not implied |
| Not live | Explicitly unavailable as an operational public service at the time of the claim |
| Unknown | Available evidence does not support a confident status assignment |
| Unverified | A claim exists but has not been checked against sufficient evidence |

#### Relationship and Historical Labels

| Label | Meaning |
| --- | --- |
| In review | A proposal or claim is currently being evaluated; no approval is implied |
| Deprecated | Use is discouraged or expected to end, but the label does not replace the Charter's Retired lifecycle status |
| Superseded | An explicitly identified successor governs the relevant scope; the relationship must be documented |

Deprecated and Superseded must not be used to bypass the Freeze Rule or retirement process for Frozen documents.

### Verification Level Taxonomy

Verification levels describe how a claim was checked. They are not interchangeable with authority or lifecycle status.

| Level | Meaning | What it does not prove |
| --- | --- | --- |
| Unverified | No sufficient check has been completed | Truth, existence, or operation |
| Self-reported | The responsible or interested source reports the claim | Independent confirmation |
| Repository-confirmed | Direct repository evidence confirms the scoped repository claim | Public availability or runtime operation |
| Publicly visible | A public surface was directly observed | Accuracy, completeness, endorsement, or operational depth |
| Reviewed | Identified reviewers evaluated the claim and evidence within a stated scope | Universal truth or current operation outside scope |
| Operationally verified | A specific capability was directly observed operating under stated conditions | Continuous availability, safety, impact, or broader capability |
| Time-limited verified | Verification is valid only for an identified period or freshness window | Present truth after that window |
| Frozen or Canonical | The claim or document is approved as authority within its scope | Empirical verification or operational reality |

Frozen or Canonical is an approval marker, not a superior form of empirical evidence.

### Claim Strength Rules

Claim language must match the strongest conclusion the evidence can responsibly support.

| Evidence condition | Maximum responsible claim pattern |
| --- | --- |
| Missing | "Evidence is not available" or "Unknown" |
| Self-reported only | "Reported by [source]" |
| Repository-confirmed | "The inspected repository contains..." |
| Publicly visible | "The inspected public surface displays..." |
| Reviewed | "Reviewed for [scope] using [evidence]" |
| Operationally verified | "Observed operating for [capability, condition, and time]" |
| Historical | "At [time], evidence showed..." |
| Conflicting | "Evidence conflicts; conclusion remains unresolved" |
| Outdated | "Previously evidenced; current status requires rechecking" |
| Frozen architecture | "Architecturally approved as [role or boundary]" |

Words such as live, validated, safe, effective, available, endorsed, canonical, approved, complete, and operational require evidence and authority appropriate to the precise claim.

### Public Expression Rules

Public expression must:

- Use evidence appropriate to the claim.
- Preserve source, scope, freshness, limitations, and status.
- Distinguish current fact from plan, aspiration, proposal, and Future possibility.
- State uncertainty when verification is incomplete.
- Avoid implying operation from repository presence or public visibility.
- Preserve provenance when summarizing canonical knowledge.
- Avoid presenting private reflection as public truth.
- Avoid marketing language that strengthens a claim beyond evidence.

When evidence is insufficient, the public claim must be narrowed, qualified, deferred, or withheld.

### Internal Architecture Rules

Internal architecture may discuss uncertainty and Future possibilities more broadly than public expression, but it must:

- Label Draft, Working, proposal, Planned, Future, Unknown, and Unverified states explicitly.
- Keep evidence boundaries discoverable.
- Avoid treating architectural approval as operational verification.
- Record conflicts with Frozen documents rather than silently resolving them.
- Keep unresolved matters in Questions Unresolved.

Internal language is not exempt from `Claim <= Evidence`.

### Canonical Knowledge Evidence Rules

Canonical knowledge requires:

- Discoverable source and provenance.
- A bounded knowledge claim.
- Explicit uncertainty and limitations.
- Review appropriate to the claim.
- Separation from public summary and runtime adaptation.

Public summaries cannot replace canonical sources. Runtime adaptation cannot modify canonical truth. Runtime evidence may be proposed as candidate evidence but cannot grant itself canonical status.

The canonical approval process and evidence threshold remain unresolved and require later architecture.

### Runtime Evidence Rules

Runtime evidence:

- Remains contextual to the runtime, user, event, conditions, and time in which it arose.
- Must preserve privacy, consent, provenance, and limitation boundaries.
- Must distinguish user-authored reflection from system-generated interpretation.
- Cannot become public institutional truth automatically.
- Cannot become canonical knowledge automatically.
- Cannot amend governance or architecture automatically.
- Cannot become stronger through frequency, popularity, personalization, or user demand.

User-authored reflection is evidence of what the person expressed in that context. It is not evidence that every interpretation, inference, diagnosis, or generalized claim is true.

### Operational Status Rules

Operational claims must identify:

- The capability observed.
- The environment or conditions relevant to the observation.
- The observation time.
- The evidence source.
- The limitations of the observation.
- Whether availability was momentary, repeated, or time-limited.

The following distinctions are mandatory:

- Existing does not mean live.
- Planned does not mean Existing.
- Future does not mean committed.
- Publicly visible does not mean fully operational.
- Repository-confirmed does not mean deployed or available.
- Not live must not be represented as operational.
- Verified must state what was verified.
- One verified capability does not verify the entire system.

### Outdated, Missing, and Conflicting Evidence

#### Outdated Evidence

Evidence becomes outdated when it is no longer current enough for the claim being made. No universal expiration period is defined here.

Outdated evidence:

- May support a historical claim.
- Must not support a stronger current claim without rechecking.
- Must retain its original observation date.

#### Missing Evidence

Missing evidence must remain Missing.

It must not be replaced by confidence, assumption, repetition, urgency, aspiration, or institutional preference.

#### Conflicting Evidence

Conflicting evidence requires:

- Preservation of each source and scope.
- Explicit documentation of the conflict.
- Narrowing or suspending the claim.
- Escalation to the authority appropriate to the affected claim.

Evidence conflicting with a Frozen document does not silently modify that document. It may trigger review and, if a change is proposed, the Freeze Rule.

#### Unverifiable Claims

An unverifiable claim must be labeled Unknown, Unverified, aspirational, or otherwise explicitly limited. It must not be presented as Verified.

### Prohibited Claims

The following claim categories must not be made without evidence and review appropriate to their scope:

| Claim category | Minimum architectural boundary |
| --- | --- |
| Live platform or capability | Direct, current operational evidence for the named capability |
| Validated assessment | Discoverable validation evidence, defined scope, limitations, and appropriate review |
| AI advisor or equivalent authority | Verified capability, explicit boundaries, and no implication of professional or canonical authority |
| Therapy, diagnosis, legal, professional, religious, or crisis authority | Must not be self-created by meUus; requires applicable external authority and governance before any bounded claim |
| Operational emergency support | Current operational evidence, approved safety boundaries, and applicable external authority |
| Account, payment, backend, or runtime capability | Direct operational evidence for the specific capability |
| Partnership or institutional endorsement | Discoverable evidence from the relevant external party and approved public expression |
| Performance, safety, reliability, or impact | Scoped evidence, limitations, freshness, and appropriate review |

No wording may imply these claims merely because a design, repository, prototype, plan, demonstration, or aspiration exists.

### Escalation Rules

| Evidence or status problem | Required escalation |
| --- | --- |
| Apparent conflict with Book Zero | Founder Review |
| Governance or Frozen architecture would change | Freeze Rule with required reviews |
| Structural taxonomy conflict or cross-domain inconsistency | Architecture Review |
| Public institutional claim exceeds approved truth | Founder Review or the later approved institutional process |
| Canonical status or evidence threshold is unclear | Requires later document |
| Private runtime evidence is proposed for another use | Founder Review and later privacy/consent architecture |
| Operational claim lacks current evidence | Withhold or narrow claim; requires evidence before resolution |
| Evidence is conflicting | Architecture Review where architecture or taxonomy is affected; otherwise the appropriate later review |
| Professional, emergency, religious, legal, diagnostic, or crisis claim appears | Founder Review and applicable external authority |
| DLAS or another Future system is presented as live | Founder Review and Architecture Review |

Escalation does not approve the claim. It pauses stronger expression until the appropriate authority resolves or defers it.

### Current Classification Preservation

This Ready for Review document does not strengthen the classifications in Frozen Documents 01-04.

In particular:

- `meuus-architecture-governance` is Existing and Verified only within the inspected repository scope established by Frozen architecture.
- `meuus.org` is an Existing ecosystem domain; current public capabilities and live status are not Verified here.
- `meuussoul.com` remains Planned as the canonical knowledge and learning domain; full operation is not Verified here.
- `meuus.app` is an Existing ecosystem domain; Phase Zero operation is not Verified here, and later runtime roles remain Future.
- DLAS remains conceptual, Future, Unresolved, and not live.

---

## Authority

This document is subordinate to:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- `03_domain_responsibility_map.md`.
- `04_authority_flow_and_decision_rights.md`.

Book Zero remains Foundational Authority. `00_READ_FIRST.md` remains Governance Authority. Frozen Documents 01-04 remain controlling Architectural Authority.

While its status is Working, this document may be referenced as developing architecture but is not canonical and remains subject to change.

This document cannot:

- Modify or reinterpret a Frozen dependency.
- Turn evidence into authority or approval.
- Authorize a public or canonical claim.
- Define evidence-processing implementation.
- Authorize implementation work.
- Begin or authorize Document 06.

---

## Inputs

The inputs to this Ready for Review document are:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- `03_domain_responsibility_map.md`.
- `04_authority_flow_and_decision_rights.md`.
- Documented Founder directives relevant to evidence, status, and truth claims.
- Discoverable evidence where a current-state claim is required.

The existence of evidence does not determine its authority, interpretation, or approved use.

---

## Outputs

If reviewed and Frozen through the governance lifecycle, this document is intended to provide:

- A canonical conceptual evidence taxonomy.
- Status and verification taxonomies.
- Evidence-boundary requirements.
- Claim-strength and communication rules.
- Operational-status constraints.
- Rules for missing, outdated, conflicting, and unverifiable evidence.
- Prohibited-claim and escalation boundaries.

At Ready for Review status, these outputs are complete enough for formal review but remain non-canonical.

---

## Dependencies

This document depends on:

- Book Zero.
- `00_READ_FIRST.md`.
- `README.md`.
- `01_master_architecture.md`.
- `02_ecosystem_topology.md`.
- `03_domain_responsibility_map.md`.
- `04_authority_flow_and_decision_rights.md`.

It inherits the authority hierarchy, lifecycle, topology, responsibility, decision rights, status language, and evidence discipline established by those documents.

If this document conflicts with a Frozen dependency, the Frozen dependency governs and the conflict must be documented for review. No later document acquires authority merely by depending on this Ready for Review document.

---

## Interfaces

The interfaces below are conceptual taxonomy relationships, not technical interfaces.

### Claim and Evidence

Evidence supports or limits a specific claim. It does not create truth.

### Evidence and Verification

Verification checks a claim against identified evidence within a declared scope and time.

### Verification and Status

Verification may support a status label only within the verified scope.

### Status and Public Expression

Public expression must preserve status meaning, evidence limits, and uncertainty.

### Canonical Knowledge and Evidence

Canonical knowledge requires provenance and review but does not create governance authority.

### Runtime Evidence and Review

Runtime evidence may be proposed for review but cannot approve itself.

### Conflicting Evidence and Frozen Architecture

Conflicting evidence may trigger review. It cannot silently amend Frozen authority.

---

## Questions Unresolved

- What exact process grants canonical knowledge status?
  - **Disposition:** Deferred to later architecture document.
- What review process governs institutional public claims beyond already approved truth?
  - **Disposition:** Deferred to Founder Review.
- What freshness criteria apply to different operational claims?
  - **Disposition:** Requires evidence before resolution.
- What evidence threshold supports a validated-assessment claim?
  - **Disposition:** Deferred to later architecture document.
- What privacy and consent authority governs reuse of user-authored evidence?
  - **Disposition:** Deferred to Founder Review.
- What external evidence standards apply to partnership, endorsement, safety, or professional claims?
  - **Disposition:** Requires evidence before resolution.
- How should verification be revoked or narrowed when later evidence conflicts?
  - **Disposition:** Deferred to Architecture Review.
- Which status labels may be used publicly before an institutional review process exists?
  - **Disposition:** Deferred to Founder Review.
- What process governs Deprecated and Superseded labels outside the architecture lifecycle?
  - **Disposition:** Deferred to later architecture document.
- Which taxonomy terms require inclusion in the future glossary?
  - **Disposition:** Deferred to later architecture document.
- What evidence, if any, may later support a DLAS status claim?
  - **Disposition:** Requires evidence before resolution.

These questions remain explicit and bounded. Their dispositions identify where resolution belongs without authorizing another document or resolving uncertainty by assumption.

---

## Risks

### Claim Inflation

Risk: language could become stronger than the evidence.

Response: enforce `Claim <= Evidence` and require explicit boundaries.

### Evidence Inflation

Risk: evidence could be mistaken for truth, authority, approval, safety, or impact.

Response: separate evidence category, verification, status, authority, and approved use.

### Status Collapse

Risk: Existing, Verified, live, Planned, Future, and Not live could be treated as interchangeable.

Response: preserve distinct definitions and require the subject and scope of every status.

### Canonical and Operational Confusion

Risk: Frozen or Canonical approval could be mistaken for empirical or operational verification.

Response: classify canonical approval separately from verification levels.

### Runtime Generalization

Risk: user reflection or runtime patterns could become generalized truth.

Response: preserve context, privacy, provenance, limitations, and review gates.

### Outdated Evidence

Risk: historical evidence could continue supporting current claims.

Response: require observation date, freshness, and rechecking.

### Public Overclaiming

Risk: visibility, marketing pressure, or institutional preference could strengthen public claims.

Response: narrow, qualify, defer, or withhold claims when evidence is insufficient.

### Freeze Bypass

Risk: conflicting evidence could be used to alter Frozen architecture silently.

Response: require explicit review and the Freeze Rule for proposed changes.

### Implementation Leakage

Risk: taxonomy could become an evidence-processing, storage, or analytics specification.

Response: keep mechanisms outside architectural taxonomy.

### Excessive Complexity

Risk: too many labels could make consistent use impossible.

Response: separate label families and require the minimum label needed for the claim.

---

## Non-goals

This document does not:

- Modify Book Zero, `00_READ_FIRST.md`, `README.md`, or Frozen Documents 01-04.
- Create new constitutional authority categories.
- Define implementation policy or public marketing copy.
- Assert that a future or unverified system is live.
- Select technologies, frameworks, vendors, or hosting.
- Define databases, APIs, schemas, protocols, or technical data flows.
- Define evidence collection, storage, transformation, processing, or analytics mechanisms.
- Define UI, authentication, payments, or deployment.
- Define runtime implementation, product features, or application state.
- Define privacy, consent, retention, or legal mechanisms.
- Define pricing or marketing claims.
- Authorize implementation work or public publication.
- Begin, create, or authorize Document 06.

---

## Review Criteria

Before this document may move from Ready for Review to Frozen, reviewers should confirm:

### Constitutional and Governance Integrity

- Book Zero remains Foundational Authority.
- `00_READ_FIRST.md` remains Governance Authority.
- Frozen Documents 01-04 remain controlling Architectural Authority.
- Evidence, verification, status, and publication do not create higher authority.
- No Frozen dependency is modified, reinterpreted, or contradicted.

### Structural Integrity

- Truth, claim, evidence, status, verification, review, approval, and authority remain distinguishable.
- Evidence categories and boundary requirements are clear.
- Status families do not collapse into one another.
- Verification levels are scoped and do not imply authority.
- Matters reserved for later documents remain outside scope.

### Truthfulness

- Claim does not exceed evidence.
- Missing evidence remains missing.
- Outdated and conflicting evidence are handled explicitly.
- No future or unverified system is represented as operational.
- Frozen or Canonical does not imply operational verification.
- DLAS remains conceptual, Future, Unresolved, and not live.

### Institutional Readiness

- Public expression rules prevent overclaiming.
- Canonical knowledge requires provenance and review.
- Runtime evidence remains contextual and non-authoritative.
- Prohibited claims cannot be inferred from plans, prototypes, repositories, or visibility.
- Escalation rules protect truth and Frozen authority.

### Implementation Independence

- No technology, framework, vendor, database, API, schema, UI, deployment, or runtime mechanism is embedded.
- Conceptual evidence boundaries cannot be mistaken for data-processing requirements.

### Lifecycle Readiness

- All required sections are substantially complete.
- Dependencies and non-goals remain explicit.
- Unresolved questions are resolved or explicitly accepted for formal review.
- Founder Review and Architecture Review have not been presumed.
