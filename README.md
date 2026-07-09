# meUus Architecture Governance

Document: README.md  
Version: v1.0  
Status: Frozen  
Authority: Governance Orientation  
Depends on: Book Zero; 00_READ_FIRST.md (Frozen v1.0)  
Supersedes: None

## Purpose

This repository exists to preserve the constitutional and architectural governance of the meUus ecosystem.

It is not an implementation repository. It does not contain the public website, application code, Knowledge Hub code, runtime prototypes, or product-specific implementation plans.

Its purpose is to keep foundational judgment stable while the software evolves across separate projects:

- `meuus-architecture-governance` - constitutional and architecture documents only.
- `meuus.org` - public foundation website and institutional surface.
- `meuus.app` - reflection, journey, and runtime application.
- `meuussoul.com` - knowledge, learning, books, and canonical content platform.

All documents in this repository are subordinate to Book Zero and governed by `00_READ_FIRST.md`.

## Repository Scope

This repository governs architecture.

It does not contain:

- implementation code.
- deployment configuration.
- infrastructure configuration.
- product features.
- runtime behavior.
- UI specifications.
- API implementation.
- databases.
- application state.

Those belong to their respective implementation repositories.

## Repository Navigation

Start here:

1. `00_READ_FIRST.md` - governance charter (Frozen v1.0).
2. `README.md` - repository orientation, navigation, workflow, and contribution expectations.

No future document acquires authority merely by being created. Authority is granted only through the governance process established in `00_READ_FIRST.md`.

This README does not authorize continuation into future architecture documents by itself.

## Document Order

The document order is governed by `00_READ_FIRST.md`.

Readers should proceed from higher authority to lower authority:

1. Book Zero - Foundational Authority.
2. `00_READ_FIRST.md` - Governance Authority.
3. `README.md` - orientation for repository use.
4. Architecture documents - only when created, reviewed, and governed according to the Charter.
5. Implementation documents - only in the relevant implementation repositories.

No later document may silently contradict an earlier or higher-authority document.

## Authority Hierarchy

This repository follows the authority hierarchy established by the Charter:

1. Foundational Authority - Book Zero.
2. Governance Authority - `00_READ_FIRST.md` and formal governance decisions.
3. Architectural Authority - approved architecture documents.
4. Implementation Authority - code, configuration, product behavior, and operational choices in implementation repositories.

If a conflict appears, the lower authority yields to the higher authority. The conflict must be documented and resolved through the established review process.

## Review Workflow

Documents move through review before becoming authoritative.

Status labels:

- Draft - initial creation or exploratory content.
- Working - substantially complete but may still contain unresolved questions.
- Ready for Review - author declares the document complete enough for formal review.
- Frozen - approved by Founder Review and Architecture Review; canonical until amended.
- Retired - no longer authoritative, retained for historical reference.

Review requires:

- Founder Review.
- Architecture Review.
- confirmation that the document does not contradict Book Zero.
- confirmation that the document follows `00_READ_FIRST.md`.
- explicit handling of unresolved questions.

This README has passed Founder Review and Architecture Review and is Frozen as v1.0.

## Freeze Workflow

A document becomes authoritative only when it is Frozen.

Freezing requires:

- the document is marked Ready for Review.
- Founder Review is complete.
- Architecture Review is complete.
- unresolved questions are either resolved or explicitly deferred.
- the final status is changed to Frozen through the established governance process.

Changes to Frozen documents require the process established in `00_READ_FIRST.md`, including an appropriate decision record where required.

No document may be treated as canonical merely because it exists in the repository.

## Contribution Expectations

Contributors must:

- read Book Zero before proposing constitutional or architectural changes.
- read `00_READ_FIRST.md` before editing any governance or architecture document.
- preserve the authority hierarchy.
- avoid introducing new architectural principles through orientation text.
- record unresolved questions instead of inventing rules.
- distinguish between explanation, proposal, review, and approved authority.
- keep implementation details in the appropriate implementation repository.

Contributions should make the architecture more explainable, more traceable, and more faithful to the higher-authority documents.

## Relationship to meUus Projects

`meuus-architecture-governance` defines governance and architecture boundaries for the ecosystem. It does not replace the separate responsibilities of the implementation repositories.

`meuus.org` is the public institutional foundation of the meUus ecosystem. It should reflect approved institutional truth and public governance status.

`meuus.app` is the reflection, journey, and runtime application. It should inherit the architectural rules that apply to runtime systems without making canonical institutional or knowledge claims on its own. It remains subordinate to the governance and constitutional documents.

`meuussoul.com` is the canonical knowledge and learning platform. It should preserve canonical knowledge, books, learning materials, and provenance according to the governance established here.

The separation between these repositories helps protect governance stability while allowing each software project to evolve within its proper boundary.

## Unresolved Questions

The following are not decided by this README:

- the exact location and format of future decision records.
- the complete list and order of future architecture documents beyond what the Charter establishes.
- the exact implementation mechanisms by which `meuus.org`, `meuus.app`, and `meuussoul.com` inherit governance constraints.

These questions must be resolved through the established governance process, not by expanding this README beyond its orientation role.

## Constitutional Reminder

This repository exists not to control behavior, but to preserve institutional judgment.

Architecture exists to preserve judgment, not merely structure.

Nothing in future architecture, implementation, or documentation may silently contradict higher-authority documents. Any apparent conflict must be documented and resolved through the established governance process.

README.md is Frozen as v1.0.
