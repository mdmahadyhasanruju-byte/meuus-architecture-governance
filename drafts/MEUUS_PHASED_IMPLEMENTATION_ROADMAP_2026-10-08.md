# meUus Phased Implementation Roadmap

**Founder-authored. Adopted 8 October 2026 (Asia/Dhaka).**
**Status:** Working roadmap. Not frozen. Governs build sequencing only — it creates no
architecture and advances no capability claim.

**Governing sequence:**

```
Preserve → Define → Validate → Design → Build → Test → Prove → Operate → Expand → Continue
```

**Governing distinction, maintained at every phase:**

```
DISCOVERED ≠ DEFINED ≠ DESIGNED ≠ BUILT ≠ TESTED ≠ DEPLOYED ≠ PROVEN
```

**The roadmap tracks two things separately, always:**

| | |
|---|---|
| **What meUus intends to become** | the vision, held intact |
| **What meUus can currently prove exists** | the evidence, never inflated |

---

## ROADMAP PRINCIPLE

The implementation must follow the sequence above. At every phase, the maturity distinction
must hold. **No phase may be declared complete on intention.** A phase is complete when its
exit criteria are met with evidence a reviewer can inspect.

---

## PHASE 0 — PRESERVE THE FOUNDATION

**Purpose:** Protect the origin, founder's intent, terminology, conceptual evolution, and
available evidence before development begins.

### 0.1 Preserve the source narrative

Three separate records:

**Immutable raw source** — preserve the complete original text, original numbering, repeated
language, and markup if the original contains markup. **Do not edit or overwrite.**

**Readable transcription** — remove interface markup, preserve all meaningful wording,
maintain the same section sequence.

**Structured extraction** — extract concepts, principles, claims, decisions, proposed systems,
risks, and evidence requirements. **Link every extraction to the original section number.**

### 0.2 Establish the foundational registers

Source · Concept · Claim · Decision · Evidence · Assumption · Risk · Terminology · Timeline ·
Change log · Unresolved-question.

### 0.3 Classify each statement

Every material statement receives exactly one status:

```
Founder-discovered · Founder-defined · Historical recollection · Vision ·
Proposed capability · Preliminary requirement · Designed · Built · Tested ·
Deployed · Validated · Uncertain · Disputed · Superseded
```

### Deliverables

Preserved founder source · Readable transcription · Concept inventory · Controlled glossary ·
Evidence-gap list · Corrected archive foundation · Version-controlled master document.

### Exit criteria

- The raw source is safely preserved
- No meaningful content has been lost
- Every foundational concept has a unique ID
- Aspirations are clearly separated from implemented features
- File backups and version controls exist
- Current truth can be distinguished from historical material

---

## PHASE 1 — DEFINE THE MINIMUM meUus FOUNDATION

**Purpose:** Convert the broad ecosystem vision into a controlled, implementable foundation.

**Primary question:** What is the smallest authentic meUus experience that demonstrates the
central idea?

**Recommended minimum foundational journey:**

```
Person → Express Need → Understand → Learn → Choose → Act → Record Evidence → Review → Continue
```

### 1.1 Define the primary user

One priority user group to start. Suggested initial user: **a person in Bangladesh who has an
idea, need, question, or goal but requires structured guidance to understand, learn, plan, and
begin creating.** This does not exclude others. It establishes a buildable starting point.

### 1.2 Define the initial problem

Working statement: *people often have intentions, knowledge, needs, or ideas but lack a clear,
accessible, evidence-aware path from intention to informed action and creation.*

**This must be tested through interviews rather than treated as proven.**

### 1.3 Define the minimum promise

*meUus helps a person express a need or idea, understand what is required, develop a structured
path, use appropriate assistance, record progress, and continue from the current state.*

**Avoid promising that anyone can immediately build anything.**

### 1.4 Finalize the foundational principles

Human remains central · AI assists but does not become human authority · Claim ≤ Evidence ·
Automate execution, not responsibility · Privacy by default · Consent before memory ·
Accessibility from the beginning · No silent historical rewriting · No single point of failure
where practical · Justice as a governing question · Preserve → Verify → Correct → Continue.

### 1.5 Create the meUus controlled glossary

meUus · meUusSoulAI · #AnyOneCan# · Justice for All · Open Memory · Evidence · Proof ·
Opportunity · Agent · Automation · Creation · Contribution · Continuation · Development Lens
and Assessment System · Public door · Ecosystem · Human authority · Qualified professional.

### Deliverables

Foundation charter · Problem statement · Initial user definition · Minimum value proposition ·
Controlled terminology register · Principle-to-feature traceability matrix · Non-goals list ·
Preliminary success criteria.

### Exit criteria

First user group defined · initial problem documented · first product boundary clear · core
terms have controlled definitions · non-goals prevent uncontrolled expansion · **founder
approval recorded**.

---

## PHASE 2 — DISCOVERY AND HUMAN VALIDATION

**Purpose:** Determine whether the proposed system addresses real human needs and whether
intended users can understand it.

### 2.1 Discovery interviews

Participant categories: students · job seekers · workers · educators · small-business
operators · people with limited digital literacy · people with limited reading or writing
capability · creators · community organizers · technical users.

**Do not treat a small discovery group as representative of everyone.**

### 2.2 Test the foundational questions

How do people currently seek help? · Where do people lose track of progress? · What prevents an
idea from becoming action? · What kinds of explanations are understandable? · When is voice
more useful than text? · What information are people willing to preserve? · What should never
be remembered automatically? · When do people want a human instead of AI? · What would count as
evidence of progress? · What causes people to stop?

### 2.3 Test the hardest-user hypothesis

Prototype: voice input · Bangla input and output · simple-language explanations · visual
guidance · low-bandwidth access · assisted onboarding · human-support escalation.

### 2.4 Journey maps

"I do not understand" · "I want to learn" · "I have a problem" · "I have an idea" · "I want to
build" · "I need help continuing previous work".

### Deliverables

Interview protocol · consent process · anonymized research notes · user-need inventory ·
accessibility findings · initial journey maps · validated and invalidated assumptions · revised
scope recommendation.

### Exit criteria

Target users understand the basic proposition · at least one meaningful journey is validated ·
major accessibility barriers documented · privacy expectations documented · unsupported
assumptions removed or reclassified · initial user requirements approved.

---

## PHASE 3 — GOVERNANCE, RIGHTS, PRIVACY, AND SAFETY BY DESIGN

**Purpose:** Establish operating boundaries **before** collecting sensitive memory, connecting
external tools, or allowing an agent to act.

### 3.1 Authority model

What the user can authorize · what AI may suggest · what requires explicit approval · what may
be automated · what requires a qualified professional · what must never be automated · who can
stop an agent · who reviews failures · who can correct records · who can appeal a decision.

### 3.2 Data classification model

Public · registered-user private · internal operational · confidential · highly restricted ·
legal-sensitive · financial-sensitive · personal memory · evidence record · deletion-restricted
due to lawful obligations.

### 3.3 Memory controls

The user must be able to understand: what is remembered · why · where stored · who can access
it · how to correct it · how to export it · how to delete it where appropriate · what cannot be
deleted and why · which AI or tool may use it.

### 3.4 Agent-permission model

```
Permission → Scope → Authentication → Action → Logging → Result → Failure Handling
```

### 3.5 Human-involvement framework

| Level | Pattern |
|---|---|
| AI Assisted | AI suggests. Human decides. |
| AI + Human Review | AI prepares. An authorized human reviews before action. |
| AI + Qualified Professional | AI organizes or explains. A qualified person verifies or decides. |
| Controlled Automation | The system acts only within an explicit, revocable, logged authorization. |

### Deliverables

Governance charter · role and permission matrix · data-classification standard · consent model ·
memory-control policy · agent-authority matrix · human-review policy · incident-handling process
· appeal and correction process · preliminary legal-review register.

### Exit criteria

No critical action lacks an accountable human owner · sensitive data has defined access rules ·
memory is consent-based · agent actions are scoped and logged · external-service use has
approval rules · failure and escalation processes exist.

---

## PHASE 4 — TECHNICAL FOUNDATION

**Purpose:** Build the secure foundation required for the first limited product.

### Recommended architecture

**Experience layer** — web application · mobile-responsive · Bangla and English foundations ·
voice pathway where feasible · accessibility support.

**Application layer** — user journey · goals · projects · tasks · learning paths · creation
records · evidence records · review and continuation.

**Identity layer** — authentication · user profiles · role-based access · consent records ·
session control · account recovery.

**Data layer** — structured database · file storage · evidence metadata · version history ·
audit records · backup and recovery.

**AI layer** — provider abstraction · prompt and instruction registry · context permission
controls · output-status classification · human-review triggers · usage monitoring.

**Operational layer** — logging · error monitoring · security monitoring · deployment controls ·
backup testing · incident handling.

### Core technical workstreams

Architecture · authentication · authorization · database · storage · evidence and provenance ·
AI-provider abstraction · prompt management · agent permission controls · observability ·
security · backup and recovery · testing · deployment · technical documentation.

### Deliverables

Architecture decision record · data model · role-based access model · threat model · backup plan
· recovery procedure · development environment · staging environment · testing framework ·
initial production-readiness checklist.

### Exit criteria

Authentication works · authorization is tested · sensitive data is protected by role · logs do
not expose restricted content · backups can be restored · AI context access is controlled ·
development, staging and production are separated · critical technical decisions documented.

---

## PHASE 5 — MINIMUM VIABLE meUus JOURNEY

**Purpose:** Deliver **one complete human-development journey** rather than many disconnected
features.

### The nine steps

| Step | What happens |
|---|---|
| **1 Express** | The user communicates a need, problem, question, idea, learning goal, or creation goal |
| **2 Understand** | meUus helps clarify meaning, wanted outcome, missing information, constraints, risks |
| **3 Learn** | Required knowledge list, simple explanations, learning sequence, evidence sources, questions needing expert help |
| **4 Choose** | The user selects goal, scope, approach, level of AI assistance, memory permission, human-review requirement |
| **5 Plan** | Milestones, tasks, dependencies, evidence requirements, review points, next action |
| **6 Act** | The user completes the next authorized action |
| **7 Record** | What was attempted, what was created, what evidence exists, what changed, what remains uncertain |
| **8 Review** | Actual result, difference from intention, lessons, risks, corrections |
| **9 Continue** | Resume from current truth, latest verified progress, open decisions, next action |

### MVP features

Account and consent · personal goal or project · guided intake · AI-supported clarification ·
basic learning plan · milestones and tasks · evidence attachment · decision record · progress
review · continuation summary · export · memory inspection and correction.

### Explicit MVP exclusions

Unless separately approved: open public marketplace · autonomous financial actions · full
multi-provider AI routing · public justice adjudication · medical or legal decision-making ·
open agent marketplace · complex value distribution · unrestricted personal-memory ingestion ·
full nine-pillar implementation · organization-wide automation.

### Exit criteria

One user can move from idea to structured action · the journey can be resumed without losing
context · evidence can be attached to progress · AI output is distinguishable from verified
information · the user can inspect remembered information · critical actions require approval ·
the journey works on low-powered or mobile devices where targeted.

---

## PHASE 6 — meUusSoulAI AND CONTROLLED AGENT CAPABILITY

**Purpose:** Introduce AI orchestration and action-oriented assistance **without removing human
authority.**

### Initial meUusSoulAI capabilities

Understand intent · clarify goals · retrieve permitted context · recommend a workflow · generate
a plan · identify missing knowledge · select an approved tool · prepare an action · request
authorization · record the result · support continuation.

### Initial agent set

| Agent | Chain |
|---|---|
| Research | Question → sources → comparison → evidence → report |
| Learning | Goal → curriculum → lesson → exercise → feedback → progress |
| Builder | Idea → requirements → architecture → build support → testing |
| Documentation | Sources → structured record → version → review |
| QA | Requirement → test cases → observed result → defect → retest |
| Accessibility | Complex content → simplification → translation → voice or visual alternative |

### Agent control requirements

Every agent must have: defined purpose · permitted tools · prohibited actions · data-access
scope · approval requirements · failure conditions · logging · evaluation method · human owner ·
emergency stop mechanism.

### Exit criteria

Agents cannot act outside assigned scope · tool access follows least privilege · sensitive
actions require approval · agent outputs preserve provenance · failed actions are visible ·
actions can be audited · **the system records what AI did and what the human approved.**

---

## PHASE 7 — LEARNING, CREATION, EVIDENCE, AND PROFILE

**Purpose:** Connect human development to demonstrated capability.

```
Learn → Attempt → Create → Test → Improve → Publish → Contribute
```

**Features:** learning pathways · practical challenges · project submissions · evidence
attachments · review criteria · feedback · revision history · capability records · portfolio and
profile controls · public and private visibility · attribution records.

**Recognition should not depend only on ranking first.** Categories: beginner creation ·
improvement · accessibility · social usefulness · local-language contribution · documentation
quality · evidence quality · teamwork · helping others.

**Exit criteria:** capability claims connect to demonstrated work · users control profile
visibility · evidence status is visible · review and correction are supported · attribution
survives revisions · recognition criteria are understandable.

---

## PHASE 8 — OPPORTUNITY AND COLLABORATION

**Purpose:** Connect demonstrated capability with legitimate opportunities.

**Pathways:** collaborative projects · mentorship · internships · employment discovery ·
freelance work · grants · competitions · scholarships · teaching · research collaboration ·
entrepreneurship.

**Safeguards:** no guaranteed success claims · clear opportunity-source attribution · scam and
abuse reporting · identity verification where appropriate · user-controlled visibility ·
transparent selection criteria where available · conflict-of-interest disclosure · record of
application and outcome.

**Exit criteria:** opportunities have identifiable sources · users understand applicable terms ·
capability records link to evidence · reporting and moderation processes work · sensitive
personal information is protected.

---

## PHASE 9 — MARKETPLACE AND VALUE DISTRIBUTION

**Purpose:** Enable legitimate exchange **only after** identity, evidence, governance, disputes
and financial controls are sufficiently mature.

```
Creation → Listing → Agreement → Payment → Delivery → Acceptance → Distribution → Record → Dispute Process
```

**Required foundations:** seller or provider verification · buyer protection · product and
service classification · agreements · intellectual-property declarations · attribution · payment
integration · tax and fee handling · refund process · dispute process · evidence retention ·
fraud controls · transaction records.

**Value-distribution ledger.** Every distribution should explain: gross customer payment ·
provider or API costs · platform costs · payment fees · applicable taxes · creator or contributor
entitlement · adjustments or refunds · final remaining balance.

**Exit criteria:** financial flows are traceable · distribution rules are understandable · users
accept applicable terms · dispute handling exists · attribution and rights are recorded ·
**financial and regulatory reviews completed for the intended operating jurisdiction.**

---

## PHASE 10 — MULTI-AI, LOCAL AI, AND ADVANCED AUTOMATION

**Purpose:** Increase resilience, choice, privacy and capability **after** the core experience is
stable.

**Capabilities:** provider abstraction · model selection policy · cost-aware routing ·
privacy-aware routing · local-model support · offline or degraded-mode support · cross-model
verification for defined use cases · provider fallback · approved automation templates · agent
performance monitoring.

**Routing considerations:** task type · required capability · sensitivity · user consent · cost ·
availability · language · latency · evidence requirements · human-review requirements · provider
terms · legal restrictions.

**Exit criteria:** the system can change providers without rewriting the product · restricted
information follows approved routing rules · provider failures have defined fallback behaviour ·
costs are monitored · local and cloud boundaries are understandable · automated actions are
reversible where appropriate.

---

## PHASE 11 — NINE-PILLAR EXPANSION

**Purpose:** Expand into specialized domains **only after shared infrastructure is proven.**

**Do not build all nine simultaneously.** Use readiness and evidence to determine the order.

**Shared foundation** — all pillars reuse: identity · consent · memory · evidence · learning ·
creation · profiles · opportunity · governance · AI controls · agent controls · audit systems.

**Pillar readiness assessment** — for every pillar: human need · target population · risk level ·
qualified-professional requirement · legal implications · data sensitivity · evidence requirement
· operational owner · funding requirement · pilot feasibility · success measure · harm-prevention
measures.

**The nine pillars:** Legal Hub · Business Hub · Unemployment Buster · Mind Beautifier · Drug
Buster · Family Harmony · Green Solutions · Idea Lab · aLive Bangladesh.

**Important boundary.** High-risk domains must not be launched merely because the AI interface
can generate answers. Domains involving health, legal rights, substance use, family conflict, or
other sensitive matters require carefully defined professional, legal, safeguarding and
escalation systems.

**Exit criteria per pillar:** approved scope · accountable owner · qualified oversight where
required · data-protection review · safety model · evidence model · pilot protocol · escalation
process · measurable outcomes · **stop conditions**.

---

## PHASE 12 — JUSTICE, ACCOUNTABILITY, AND INSTITUTIONAL GOVERNANCE

**Purpose:** Operationalize justice as a governing question — **not** as an undefined slogan or
an automated judgment engine.

**For every major feature or policy:** who is affected? · who benefits? · who bears risk? · who
authorizes? · who is responsible? · what evidence supports the decision? · what rights apply? ·
how can someone challenge the result? · who reviews the challenge? · how are uninvolved people
protected? · what consequence is legitimate? · how is the decision documented?

**Required systems:** complaint procedure · correction procedure · appeal mechanism · content and
conduct rules · conflict-disclosure rules · dispute-resolution framework · incident register ·
decision-audit process · independent-review pathway · governance-change process · emergency
suspension authority.

**Critical boundary.** meUus must not claim to deliver universal legal or moral justice
automatically. It can operationalize procedural protections, evidence discipline, accountable
decision-making, review, correction, and lawful handoff.

**Exit criteria:** major decisions are reviewable · users can challenge material errors ·
corrections remain historically traceable · authority is documented · conflicts of interest are
disclosed · serious matters have lawful escalation · **automated systems do not become final
authority over disputed human rights.**

---

## PHASE 13 — GLOBAL ADAPTATION AND FEDERATION

**Purpose:** Extend beyond the initial proof context without assuming one design works for every
language, culture, or jurisdiction.

```
Bangladesh proof context → documented learning → adaptable core → localized implementation
```

**Localization dimensions:** language · literacy · accessibility · culture · law · payments ·
education · employment · identity systems · data protection · professional authority · community
governance · available technology · connectivity.

**Exit criteria:** each localization has accountable leadership · legal assumptions are
reassessed · translations are reviewed · accessibility is tested locally · data boundaries are
documented · local communities can provide correction and feedback · **global branding does not
erase local context.**

---

## CROSS-PHASE WORKSTREAMS

These continue through every phase.

| Workstream | Contents |
|---|---|
| **Evidence** | Every claim has a status · important claims link to evidence · insufficient evidence remains visible · source provenance preserved |
| **Security** | Threat modeling · access control · monitoring · incident response · backup and recovery · credential protection |
| **Privacy** | Data minimization · consent · inspection · correction · export · appropriate deletion · purpose limitation |
| **Accessibility** | Bangla · simple language · voice · visual explanation · keyboard accessibility · low-bandwidth pathways · assisted interaction |
| **Governance** | Authority · accountability · appeals · corrections · auditability · stop conditions |
| **Documentation** | Current state · history · decisions · evidence · changes · risks · next action |
| **Sustainability** | Operating cost · AI-provider cost · infrastructure cost · support capacity · revenue or funding logic · maintenance responsibility |

---

## RECOMMENDED BUILD ORDER

**Foundation**
1. Preservation and evidence system
2. Controlled terminology
3. Initial user research
4. Governance and privacy
5. Secure technical foundation

**First working product**
6. Express a need or idea → Understand → Learn → Plan → Act → Record evidence → Review → Continue

**Capability expansion**
7. meUusSoulAI
8. Controlled agents
9. Learning and creation
10. Profile and proof
11. Opportunity

**High-complexity expansion**
12. Collaboration
13. Marketplace
14. Value distribution
15. Multi-AI orchestration
16. Local AI
17. Advanced automation

**Institutional expansion**
18. Nine pillars
19. Justice and appeal systems
20. Global localization
21. Federated ecosystem development

---

## FIRST 90-DAY EXECUTION CYCLE

**This is a suggested planning cycle, not a claim that all work can be completed within 90 days.**

### Days 1–30 — Preserve and Define

Preserve the meUus foundational source · create structured concept and claim registers ·
complete controlled glossary · define the initial user · define the initial problem · establish
MVP boundaries · create non-goals · draft governance principles · inventory existing code,
designs, domains and files · **identify what is actually built.**

**Decision gate.** Proceed only if the team can state: who the first user is · what the first
problem is · what the first journey is · what is excluded · what evidence will demonstrate
progress.

### Days 31–60 — Research and Design

Conduct structured user discovery · test Bangla and voice requirements · map the first user
journey · design consent and memory controls · draft data model · draft permission model · create
technical architecture · create interface prototype · test prototype with intended users · revise
requirements.

**Decision gate.** Proceed only if intended users can understand and complete the proposed
journey.

### Days 61–90 — Build the Vertical Slice

Build one complete path: **Express → Understand → Plan → Act → Record → Review → Continue.**

Include: authentication · consent · one personal project · AI-supported clarification ·
milestones · evidence attachment · decision log · continuation summary · user-controlled memory
· basic audit record · backup and recovery test.

**Decision gate.** Proceed to pilot only if: critical access controls pass testing · the journey
works end to end · AI content is properly labeled · evidence can be preserved · users can inspect
stored information · failures are logged · backups can be restored.

---

## PROGRESS DASHBOARD

**Status vocabulary:**

```
Not started · Research · Defined · Designed · In development · Built · Testing ·
Blocked · Pilot · Deployed · Validated · Superseded
```

**For every capability, record:** capability ID · phase · owner · intended user · requirement ·
current status · evidence · risks · dependencies · approval · next action · target review date.

---

## PRIORITY RISKS

| # | Risk | Control |
|---|---|---|
| 1 | **Scope expansion** — trying to build the full ecosystem at once | One validated user journey before broad expansion |
| 2 | **Vision presented as implementation** — proposed features appear operational | Mandatory maturity labels and evidence references |
| 3 | **Sensitive memory collection** — personal information becomes excessive or inaccessible | Consent, minimization, inspection, correction, export, appropriate deletion |
| 4 | **AI authority confusion** — generated content treated as professional or final authority | Clear status labeling and qualified-human escalation |
| 5 | **Autonomous agent harm** — agents act beyond user intention | Scoped permissions, approval gates, logs, limits, emergency stopping |
| 6 | **Provider dependence** — core services fail if one provider changes | Provider abstraction, exportability, backups, fallback planning |
| 7 | **Evidence weakness** — confident claims exceed actual proof | Claim ≤ Evidence |
| 8 | **Justice overclaim** — the platform appears to define or deliver universal justice | Justice as a governing and procedural principle, with lawful human review |
| 9 | **Sustainability failure** — costs exceed available resources | Cost tracking, usage limits, staged rollout, sustainable operating model |
| 10 | **Founder dependency** — essential knowledge remains only with the founder | Documentation, decision records, delegated authority, continuity planning, controlled knowledge transfer |

---

## IMMEDIATE ACTION LIST

1. Register the ecosystem narrative as a controlled meUus source
2. Produce the raw and readable versions
3. Extract and identify all concepts
4. Create the meUus terminology register
5. Inventory everything already built
6. Separate current reality from proposed capability
7. Define the first user group
8. Select the first end-to-end journey
9. Write explicit MVP exclusions
10. Draft consent, memory, authority and evidence requirements
11. Review the existing technical architecture
12. Build or repair the first vertical slice
13. Test with intended users
14. Record evidence
15. Continue only after the phase gate is passed

---

## FINAL IMPLEMENTATION SEQUENCE

```
Foundation → Human Validation → Governance → Technical Core → MVP Journey →
meUusSoulAI → Controlled Agents → Learning and Creation → Profile and Proof →
Opportunity → Marketplace → Multi-AI and Automation → Nine Pillars →
Justice Governance → Global Adaptation
```

---

## WHAT THIS ROADMAP DOES

It protects the full meUus vision **without trying to implement every idea simultaneously.**

It makes the individual human journey the first proof.

It places governance **before** powerful automation.

It separates aspirations from deployed capabilities.

It gives every expansion phase a clear, evidence-based gate.

---

## STATUS OF THIS ROADMAP AGAINST THE CURRENT RECORD

Recorded honestly on 8 October 2026, so the roadmap and reality can be compared.

**Items that already have artifacts on this machine** (per the 8 October verification and the
governance repository):

- Phase 0 — source preservation: **partially done.** The Book Zero manuscript is preserved in
  75 files; an extraction was produced 8 October; the governance repository holds 152 commits.
- Phase 0 — registers: **partially done.** A source register, intake review, and claim-risk
  registers exist. **The Decision Register (11) is referenced by two frozen documents and does
  not exist.** This blocks Rule 2 (Freeze Rule).
- Phase 3 — governance: **substantially done at the conceptual level.** Frozen documents 01–07
  define authority flow, evidence taxonomy, domain responsibility and public expression.
- Phase 4 — technical foundation: **partially built.** Source exists for all four domains; the
  `www.meuus.app` production build is live and verified.
- Phase 5 — MVP journey: **not built as a single journey.** The existing app has Landing, Auth,
  Dashboard and StartingPoint pages. Whether these constitute the nine-step journey in section
  Phase 5 has not been assessed.
- Phases 6–13: **not started**, except as conceptual material in the Book Zero manuscript and
  the 8 October complete model.

**The blocking item, stated plainly:** Phase 0's exit criteria are not met, because the Decision
Register does not exist and Book Zero is not yet filed as a numbered artifact. Per this
roadmap's own rule, **later phases should not be declared started while an earlier phase's exit
criteria remain unmet.**

**No claim in this section exceeds what was directly observed on 8 October 2026.**
