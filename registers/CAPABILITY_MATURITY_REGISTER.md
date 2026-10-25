Document: CAPABILITY_MATURITY_REGISTER.md
Title: meUus Capability Maturity Register
Status: **Draft — v0.1. Not Frozen.**
Authority: **None.** This is a status register. It records what is claimed and what is evidenced.
It does not grant status.
Depends on:
- 05_evidence_status_and_truth_taxonomy.md
- 11_decision_register.md
- BOOK_ZERO_CONCEPT_REGISTER.md
- MEUUS_PHASED_IMPLEMENTATION_ROADMAP_2026-10-08.md
Supersedes: None
Purpose: Satisfy Phase 0 exit criterion 4 of the meUus Phased Implementation Roadmap —
"aspirations are clearly separated from implemented features" — by recording every named
capability with its actual maturity and the evidence behind that maturity.
Last Updated: 2026-10-08
Reviewed by:
- Founder: Pending

---

## 1. WHY THIS EXISTS

The roadmap requires that **aspirations are clearly separated from implemented features**, and
that two things are tracked separately at all times:

| | |
|---|---|
| **What meUus intends to become** | the vision |
| **What meUus can currently prove exists** | the evidence |

The Final Document tags every *section* by authority level. That separates authority. **It does
not separate maturity.** A capability can be architecturally approved and completely unbuilt.

This register closes that gap. It is the per-capability answer to *"what actually exists?"*

---

## 2. THE MATURITY SCALE

Per the roadmap's progress dashboard. Every capability receives exactly one.

```
Not started · Research · Defined · Designed · In development · Built · Testing ·
Blocked · Pilot · Deployed · Validated · Superseded
```

**Rules for assigning a level:**

1. A level is assigned only from evidence. **Never from intention.**
2. `Deployed` requires an observed public surface. `Validated` requires operational evidence at
   a stated scope and time. Per `05_evidence_status_and_truth_taxonomy.md`, **public visibility
   does not prove operation** and **repository presence does not prove runtime capability.**
3. `Built` does **not** imply `Tested`. `Tested` does **not** imply `Deployed`.
4. Where evidence is absent, the level is **`Not started`** or **`Unknown`** — never inferred
   from a plan, a prototype, a design, or an aspiration.
5. A capability named in Book Zero, the Final Document, or the roadmap **is not therefore
   built.** Being named is `Defined`, at most.

---

## 3. THE REGISTER

### 3.1 Governance and foundation

| ID | Capability | Maturity | Evidence | Source |
|---|---|---|---|---|
| CAP-G-001 | Book Zero identified | **Defined** | Founder confirmation 2026-10-08; `00_BOOK_ZERO.md` | `00_BOOK_ZERO.md` |
| CAP-G-002 | Book Zero extracted | **Built** | 19 chapters, 110,390 words, verbatim | `_intake/book-zero/` |
| CAP-G-003 | Book Zero **frozen** | **Not started** | No Freeze Rule executed | — |
| CAP-G-004 | Decision Register operable | **Built** | `11_decision_register.md` exists; **0 entries recorded** | `11_decision_register.md` |
| CAP-G-005 | Change log | **Built** | `CHANGE_LOG.md` exists, one dated entry | `CHANGE_LOG.md` |
| CAP-G-006 | Concept register | **Built** | 105 concepts with unique IDs | `registers/BOOK_ZERO_CONCEPT_REGISTER.md` |
| CAP-G-007 | Concept register complete | **Not started** | Completeness explicitly recorded as Unknown | same |
| CAP-G-008 | Evidence taxonomy | **Defined** | Frozen Document 05 | `05_evidence_status_and_truth_taxonomy.md` |
| CAP-G-009 | Authority flow and decision rights | **Defined** | Frozen Document 04 | `04_authority_flow_and_decision_rights.md` |
| CAP-G-010 | Documents 08, 09, 10 | **Not started** | Direct repository inspection: do not exist | `11_decision_register.md` §6 |
| CAP-G-011 | Architecture Review of 8 Oct artifacts | **Not started** | Not performed | — |
| CAP-G-012 | Chapter 35 — Justice | **Designed** | Draft, 2,058 words, not founder-approved | `_intake/book-zero/` |

### 3.2 The four public doors

| ID | Capability | Maturity | Evidence | Source |
|---|---|---|---|---|
| CAP-D-001 | meuus.org public surface | **Deployed** | HTTP 200, 8 Oct 2026, Cloudflare, 63,107 bytes | `VERIFICATION_2026-10-08.md` |
| CAP-D-002 | meuus.org `/dlas` route | **Not started** | HTTP 404, 8 Oct 2026 | same |
| CAP-D-003 | meuussoul.com public surface | **Deployed** | HTTP 200, 46,533 bytes | same |
| CAP-D-004 | meuussoul.com `/dlas` route | **Deployed** | HTTP 200, 20,192 bytes | same |
| CAP-D-005 | meuussoul.com `/knowledge/language` | **Deployed** | HTTP 200, 29,982 bytes | same |
| CAP-D-006 | www.meuus.app application | **Deployed** | HTTP 200; **full application confirmed in the lazy chunk** (DLAS, Assessment, Dashboard, meYoo, Growth Paths present) | `VERIFICATION_2026-10-08.md` §7 |
| CAP-D-007 | rujbel.org founder archive | **Deployed** | HTTP 200, 27,853 bytes | same |
| CAP-D-008 | Rujbel isolated review Worker | **Deployed** | HTTP 200, workers.dev, 14 routes previously 200 | same |
| CAP-D-009 | **Commit-to-production provenance — all four** | **Blocked** | None of the four has a reviewed commit mapped to production | `ECOSYSTEM_RELEASE_MANIFEST.md` |
| CAP-D-010 | meuus.org PR #68 merge | **Blocked** | Green checks, unmerged, draft | GitHub API 8 Oct |
| CAP-D-011 | meuus-soul PR #1 merge | **Blocked** | Green CI, no `main` branch, no Cloudflare preview | same |
| CAP-D-012 | meuus-app-ai PR #3 | **Blocked** | Two Vercel checks failed — "Canceled from the Vercel Dashboard"; head unsigned | same |
| CAP-D-013 | rujbel PR #1 merge | **Blocked** | Green CI, unmerged, no Git build connection | same |

### 3.3 Engineering and release

| ID | Capability | Maturity | Evidence | Source |
|---|---|---|---|---|
| CAP-E-001 | meUus app source builds | **Built** | `vite build`, 1526 modules, 2.10s, exit 0 — 8 Oct 2026 | `VERIFICATION_2026-10-08.md` §7 |
| CAP-E-002 | meUus workspace typecheck | **Testing** | Recorded PASS at Entry 018 (2026-09-23); **not re-run this session** | `docs/decision-log.md` |
| CAP-E-003 | Commit signing | **Not started** | No key exists. GPG broken (`keyboxd` missing); `~/.ssh` empty; no signing config | `CONTINUE_PROMPT_meUus_2026-10-08.md` §5 |
| CAP-E-004 | Live E2E (`verify-ecosystem.mjs`) | **Not started** | Never run. Requires founder authorisation | same |
| CAP-E-005 | Secret hygiene | **Not started** | Live API key in `firebase-applet-config.json`; SQL credentials in `.env` | same |
| CAP-E-006 | Git version control of 8 Oct artifacts | **Not started** | All untracked; nothing committed | `git status` 8 Oct |
| CAP-E-007 | Backup and restore test | **Not started** | No evidence of a restore test | — |

### 3.4 Product and journey

| ID | Capability | Maturity | Evidence | Source |
|---|---|---|---|---|
| CAP-P-001 | Landing page | **Deployed** | In the live `.app` bundle | source inspection |
| CAP-P-002 | Authentication | **Deployed** | Auth page and AuthContext present and built | source inspection |
| CAP-P-003 | Dashboard | **Deployed** | Present in the live lazy chunk | `VERIFICATION_2026-10-08.md` §7 |
| CAP-P-004 | StartingPoint | **Deployed** | Page present in source and built | source inspection |
| CAP-P-005 | DLAS surface | **Deployed** | Present in live bundle; per-tier question banks absent | same |
| CAP-P-006 | DLAS per-tier question banks (21/50/75/100) | **Not started** | Await founder-authored content. Never to be fabricated | `docs/decision-log.md` Entry 018 |
| CAP-P-007 | **The nine-step MVP journey as one journey** | **Unknown** | The roadmap's nine steps are not implemented as a single flow. Whether the existing pages constitute them is **unassessed** | — |
| CAP-P-008 | Consent and memory controls | **Not started** | No implementation found | — |
| CAP-P-009 | Evidence attachment in product | **Not started** | No implementation found | — |

### 3.5 Capability layer — AI, agents, automation

**Every capability in this section is named in Book Zero, the Final Document, or the roadmap.**
**Being named is `Defined`, at most. None is `Built`.**

| ID | Capability | Maturity | Evidence |
|---|---|---|---|
| CAP-A-001 | AI provider abstraction | **Not started** | No implementation found |
| CAP-A-002 | Multi-AI orchestration | **Not started** | — |
| CAP-A-003 | Agent runtime | **Not started** | — |
| CAP-A-004 | Agent permission model (L0–L5) | **Defined** | Named in the workspace `AgentCoreProvider`; **not verified as enforcing** |
| CAP-A-005 | Automation engine | **Not started** | — |
| CAP-A-006 | Local AI support | **Not started** | — |
| CAP-A-007 | Tool layer | **Not started** | — |
| CAP-A-008 | meUusSoulAI | **Not started** | Named only. SoulAI is **paused** pending governance review |
| CAP-A-009 | Open Memory | **Not started** | — |
| CAP-A-010 | Knowledge vault / document ingestion | **Not started** | — |

### 3.6 Shared world — value, rights, governance

| ID | Capability | Maturity | Evidence |
|---|---|---|---|
| CAP-S-001 | Profile and proof | **Not started** | — |
| CAP-S-002 | Opportunity pathways | **Not started** | — |
| CAP-S-003 | Marketplace | **Not started** | — |
| CAP-S-004 | Value-distribution ledger | **Not started** | — |
| CAP-S-005 | Attribution records | **Not started** | — |
| CAP-S-006 | Complaint and correction procedure | **Not started** | — |
| CAP-S-007 | Appeal mechanism | **Not started** | — |
| CAP-S-008 | Incident register | **Not started** | — |
| CAP-S-009 | Nine-pillar domain services | **Not started** | Named as directions in Book Zero Ch 24 |

---

## 4. THE SUMMARY COUNT

**Counted mechanically** from the maturity column of every row in section 3, not by hand:

| Maturity | Count |
|---|---|
| **Deployed** | 12 |
| **Built** | 5 |
| **Blocked** | 5 |
| **Defined** | 4 |
| **Designed** | 1 |
| **Testing** | 1 |
| **Unknown** | 1 |
| **Not started** | 31 |
| **Total recorded** | **60** |

**Read this honestly.** Of the capabilities recorded:

- **12 are deployed** — every one is a public surface or a page. **None has a reviewed commit
  mapped to production.**
- **31 have not been started** — more than half the register, and it is where almost all of the
  vision lives.
- **1 is Unknown** — the nine-step MVP journey, which the roadmap treats as the first proof.

**Note on the count itself.** The first version of this summary was written by hand and was
**wrong** — it understated `Not started` by six and overstated three other levels. The figures
above are now produced mechanically from the maturity column of every row. **A register that
cannot count its own rows accurately is not yet a reliable instrument**, and that error is
recorded rather than quietly corrected.

**The largest single finding: the capabilities that are deployed and the capabilities that are
vision share almost no overlap.** The four doors are live. The ecosystem they are doors into is
not built.

---

## 5. WHAT THIS REGISTER DOES NOT DO

- It does **not** grant status. Status comes from evidence.
- It does **not** verify that the capability list is complete. **Completeness is Unknown.**
- It does **not** assess the four domains' content, accessibility, or quality. Only existence.
- It does **not** modify any Frozen document.
- It does **not** record decisions. Those belong in `11_decision_register.md`.
- It does **not** claim any deployed surface is correct, safe, or complete.

**Every `Deployed` level in this register rests on an HTTP response and a bundle inspection on
8 October 2026. That is a time-limited observation, not a standing truth.**

---

## 6. STATUS

| | |
|---|---|
| Capabilities recorded | **60** (counted mechanically from the maturity column) |
| Phase 0 criterion 4 ("aspirations separated from implemented features") | **PARTIALLY MET** — separation achieved; completeness Unknown |
| Frozen documents modified | **NONE** |
| Claims advanced | **NONE** |
| Founder approval | **Pending** |
| Frozen | **No** |
