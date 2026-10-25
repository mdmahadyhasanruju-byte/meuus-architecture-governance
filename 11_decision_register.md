Document: 11_decision_register.md
Title: meUus Decision Register
Status: **Draft — v0.1. Not Frozen.**
Authority: **None until frozen.** This is a Procedure Register: it records decisions, it does not make them.
Depends on:
- Book Zero (identified 2026-10-08)
- 00_READ_FIRST.md
- README.md
- 01_master_architecture.md
- 04_authority_flow_and_decision_rights.md
- 05_evidence_status_and_truth_taxonomy.md
Supersedes: None
Purpose: Provide the operable record required by Rule 2 (Freeze Rule) and Rule 5 (Discoverable
Reasons for Every Decision) of `00_READ_FIRST.md`, which both reference this document by name.
Last Updated: 2026-10-08
Reviewed by:
- Founder: Pending
- Architecture: Pending

---

## 1. WHY THIS DOCUMENT EXISTS

`00_READ_FIRST.md` Rule 2 requires that any change to a Frozen document be entered in **"a new
entry in the Decision Register (11_decision_register.md)"**, together with justification,
Founder approval, Architecture Review confirmation, a version increment, and a public change-log
entry.

Rule 5 requires that every architectural decision have a reason discoverable from a named
source, and lists the **"Decision Register (explicit architectural decisions with rationale)"**
as one of those sources.

`04_authority_flow_and_decision_rights.md` (Frozen, v1.0) states in its Decision Rights Matrix:
*"Frozen architecture change … Required review or gate: **Freeze Rule, including required reviews
and decision record**."*

**This document did not exist.** Two Frozen documents required it by name. Until it existed,
Rule 2 had no operable mechanism and no freeze could be procedurally valid.

This document creates that mechanism. It does not change any Frozen text.

---

## 2. SCOPE

This register records **decisions**. It does not create authority, resolve unresolved questions,
approve claims, or grant status.

| This register may | This register may not |
|---|---|
| Record a decision that was made, with its reason and evidence | Decide anything |
| Record a decision's authority basis and approval state | Grant authority |
| Record an unresolved question and its disposition | Resolve an unresolved question by assumption |
| Record a superseded decision and its successor | Modify a Frozen document |
| Record that a required approval is **pending** | Present a pending approval as complete |

Per `05_evidence_status_and_truth_taxonomy.md`: **Approval authorizes a bounded use; it does not
create truth.** A register entry is a record, not a claim.

---

## 3. ENTRY FORMAT

Every entry uses exactly this structure. Fields must not be omitted. Where a field is unknown,
it says `Unknown` — it is never left blank and never inferred.

```
Entry number:
Date:
Title:
Decision:
Context:
Decision authority:        Founder / Architecture / Governance (Charter) / Implementation
Authority basis:           Rule, document, or Founder Direction that permits the decision
Authority state:           Decidable / Review-gated / Escalated / Frozen-change / Forbidden / Unresolved
Reason:                    Why this decision, discoverable without the original author
Evidence:                  What supports the decision, with source and scope
Evidence status:           Per 05 taxonomy — e.g. Founder-supplied, Repository-confirmed, Unknown
Alternatives considered:
What is NOT decided:       Explicit exclusions
Frozen documents affected: None / list — and whether the Freeze Rule is required
Founder approval:          Y / N / Pending — with date
Architecture Review:       Y / N / Pending — with date
Change-log entry:          Required: Y/N — and location
Supersedes:
Next action:
```

**Rules for entries:**

1. `Decision authority` must name an authority that exists per
   `04_authority_flow_and_decision_rights.md`. If none exists, the entry records the question
   as **Unresolved** rather than inventing a decider.
2. `Founder approval: Pending` is recorded as **Pending**. Pending is never written as Y.
3. An entry that would change a Frozen document must record `Frozen documents affected` and set
   the Freeze Rule as required. **The entry does not perform the freeze.** It records that the
   freeze is required and tracks it.
4. `What is NOT decided` is mandatory. It is the field that prevents a bounded decision from
   being read as broader than it is.

---

## 4. REGISTER STATE

| | |
|---|---|
| Entries recorded | **0** |
| Entries pending | 2 (see section 6) |
| Frozen documents modified by this document | **None** |
| Freeze Rule invoked | **No** |

---

## 5. ENTRIES

*No decisions are recorded yet.*

This is stated plainly rather than filled with placeholder entries. An empty register is
**Unknown**, not **Empty-and-fine**. `05_evidence_status_and_truth_taxonomy.md` rule 9: *missing
evidence remains missing evidence.*

---

## 6. PENDING ITEMS REQUIRING REGISTER ENTRIES

These are known matters that will require an entry when decided. They are listed here so they are
not lost, **not** because they are decided.

### Pending 1 — Book Zero identification

| Field | Value |
|---|---|
| Matter | Whether the manuscript *Be The Starting Point — meUus* constitutes Book Zero |
| Founder statement | Confirmed 8 October 2026 |
| Authority state | **Review-gated** |
| Why gated | Rule 10 reserves foundational human values to Book Zero, and Rule 2 requires a decision record for placing content there. Identifying Book Zero defines what may inherit from it, which affects every Frozen document's dependency chain |
| What is NOT decided | That Book Zero is frozen; that the extraction boundary is approved; that Chapter 35 is accepted; that the manuscript may be published |
| Frozen documents affected | **None directly** — but every one of 01–07 declares `Depends on: Book Zero`, so the dependency becomes resolvable once this is recorded |
| Required before entry | Founder approval recorded; Architecture Review confirmation; the extracted artifact filed in this repository |
| Raise as | Entry 001, when review completes |

### Pending 2 — Absence of Documents 08, 09, 10

| Field | Value |
|---|---|
| Matter | Whether documents 08, 09 and 10 were ever written, and whether their absence is an accepted institutional risk |
| Evidence | Direct repository inspection 8 October 2026: only `00_READ_FIRST.md` and `01`–`07` exist, plus `README.md` |
| Authority state | **Unresolved** |
| Why it matters | `01_master_architecture.md` and `05_evidence_status_and_truth_taxonomy.md` reference "later documents" and Document 11 by name. Subject areas reserved for later documents (per `04_authority_flow…` §Matters Reserved) have no home |
| What is NOT decided | That 08–10 should be written; what they should contain; that their absence is acceptable |
| Frozen documents affected | None — recording an absence modifies no text |
| Required before entry | Founder decision: write them, or accept the absence explicitly |
| Raise as | Entry 002 |

---

## 7. WHAT THIS DOCUMENT DOES NOT DO

- It does **not** modify `00_READ_FIRST.md` or any Frozen document.
- It does **not** freeze itself.
- It does **not** resolve the Pending items — it records them.
- It does **not** create architecture, authority, or claims.
- It does **not** grant canonical knowledge status to anything.
- It does **not** authorise any freeze. It records that a freeze is required when one is.

`04_authority_flow_and_decision_rights.md` §Matters Reserved for Later Documents: *"This
document does not decide … Decision rights for any future domain not approved by the Founder."*
This register inherits that boundary. It does not assign decision rights.

---

## 8. QUESTIONS UNRESOLVED

- Should this register be Frozen, and if so at which version?
- Does this register require an entry in itself for its own creation?
  - **Disposition:** Deferred to Governance Review. Recorded rather than assumed.
- Which Frozen document, if any, should formally declare a dependency on this register?
- What is the change-log location referenced by Rule 2's "public change log entry"?
  - **Disposition:** Deferred to Founder Review.
- Are entries append-only, and may an entry be corrected without superseding it?
  - **Disposition:** Deferred to Architecture Review.

---

## 9. RISKS

| Risk | Control |
|---|---|
| A register entry is read as approval | Section 3 field `Founder approval` must read Pending until it is not; `What is NOT decided` is mandatory |
| The register becomes a decision-maker | Section 2 table: this register may not decide anything |
| Pending items are mistaken for decisions | Section 6 is titled Pending and each row states its authority state |
| An empty register is read as compliance | Section 4 states entries = 0 and section 5 states Unknown, not fine |
| Silent drift through a register entry | Rule 2 still requires the full Freeze Rule; an entry alone freezes nothing |

---

## 10. STATUS

- Rule 2 mechanism: **created by this document, pending review**
- Rule 5 source: **created by this document, pending review**
- Entries recorded: **0**
- Frozen documents modified: **None**
- Founder approval: **Pending**
- Architecture Review: **Pending**
- Frozen: **No**
