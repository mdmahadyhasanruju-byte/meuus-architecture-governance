# meUusSoul Phase 1 Route/Content Map

## 1. Map Identity

- Map title: meUusSoul Phase 1 Route/Content Map
- Package name: meUusSoul Phase 1 ZIP Package
- ZIP file name: meuussoul-phase1.zip
- Related intake review path: reports/intake/meUusSoul_Phase_1_ZIP_intake_review.md
- Related source record path: sources/meuussoul-phase1/meUusSoul_Phase_1_ZIP_source_record.md
- Related ZIP inventory review path: reviews/zip-inventory/meUusSoul_Phase_1_ZIP_inventory_review.md
- Related technical compatibility review path: reviews/technical/meUusSoul_Phase_1_technical_compatibility_review.md
- Date created: 2026-07-11
- Status: Draft Route/Content Map
- Public status: Internal only
- Authority: Mapping Aid Only
- Canonical status: Not Canonical
- Publication status: Not Published
- Runtime status: Not Live
- Production status: Not Production Ready
- Deployment status: Not Approved
- Merge status: Not Approved

## 2. Governance Boundary

This map does not approve implementation.
This map does not approve merge.
This map does not approve deployment.
This map does not publish any route or content.
This map does not make package content canonical.
This map does not make package routes live.
This map does not amend Frozen governance.
This map only organizes likely routes/content for future review.

## 3. Package Route/Content Overview

- ZIP listed only: Yes
- ZIP extracted: No
- Files executed: No
- Dependencies installed: No
- Build/dev/start run: No
- Package appears to contain: public/, src/, README.md
- Likely route files exist under: src/routes/
- Likely authenticated route candidates exist under: src/routes/_authenticated/
- Likely content/data files exist under: src/data/ and src/data/content/
- Likely reusable components exist under: src/components/
- Likely styles exist under: src/styles/
- Likely public sitemap exists under: public/sitemap-soul.xml

## 4. Route Map Table

| Route/File Path | Likely Public URL / Route Purpose | Public or Authenticated? | Related Components/Data | Status Label Needed | Main Risk | Review Needed |
|---|---|---|---|---|---|---|
| src/routes/soul.index.tsx | /soul index or landing page | Public candidate | SoulLayout, SoulSidebar, hubs, pillars | Draft / Not Live | May imply public meUusSoul launch or full platform readiness | Claim/status label review; content provenance review |
| src/routes/soul.ai.tsx | /soul/ai AI learning or AI overview page | Public candidate | soul components; possible hub data | Future / Planned; Not Live | May imply meUus AI or meYoo runtime is live | AI/DLAS status review; technical claim review |
| src/routes/soul.dlas.tsx | /soul/dlas DLAS overview page | Public candidate | soul components; possible pillar data | Not Validated Assessment; Learning / Reflection Only | May imply validated assessment, diagnosis, scoring, or authority | Qualified boundary review; claim/status review |
| src/routes/soul.learn.tsx | /soul/learn learning page | Public candidate | src/data/content/learn-manuscript.ts | Draft; Learning / Reflection Only | Manuscript/content overclaim or unverified learning claims | Provenance review; public-expression review |
| src/routes/soul.earn.tsx | /soul/earn earning or work/skill page | Public candidate | src/data/content/earn-manuscript.ts | Draft; Future / Planned where applicable | May imply paid levels, services, income, or availability | Claim/status review; business/legal boundary review |
| src/routes/soul.eq.tsx | /soul/eq emotional intelligence page | Public candidate | src/data/content/eq-manuscript.ts | Learning / Reflection Only; Not Therapy or Treatment | May imply therapy, mental-health support, or treatment | Qualified boundary review; sensitivity review |
| src/routes/soul.knowledge-before-action.tsx | /soul/knowledge-before-action principle page | Public candidate | soul components; content/data unknown | Source Candidate | Principle may become public without provenance | Provenance and public-expression review |
| src/routes/soul.support.tsx | /soul/support support page | Public candidate | soul components; content/data unknown | Not Live; Learning / Reflection Only | May imply support service availability | Service/status review; safety boundary review |
| src/routes/soul.language.tsx | /soul/language language/localization page | Public candidate | soul components; content/data unknown | Draft | Localization claims may be incomplete | Localization and content review |
| src/routes/soul.start.tsx | /soul/start starting-point page | Public candidate | soul components; content/data unknown | Draft / Prototype where applicable | May imply live onboarding or journey system | Status label review |
| src/routes/soul.human-development.tsx | /soul/human-development human development page | Public candidate | soul components; content/data unknown | Learning / Reflection Only | May imply personal development outcomes | Claim/sensitivity review |
| src/routes/soul.professionalism.tsx | /soul/professionalism professional development page | Public candidate | soul components; content/data unknown | Learning / Reflection Only | May imply professional advice or credentialing | Professional boundary review |
| src/routes/soul.resources.tsx | /soul/resources resource page | Public candidate | soul components; content/data unknown | Source Candidate | Resource provenance may be unclear | Source/provenance review |
| src/routes/soul.founder.tsx | /soul/founder founder page | Public candidate with sensitivity limits | soul components; content/data unknown | Draft; Internal Only where applicable | Founder/private material exposure | Founder/sensitivity review |
| src/routes/soul.community.tsx | /soul/community community page | Public candidate | soul components; content/data unknown | Future / Planned; Not Live | May imply active community or services | Current-state verification |
| src/routes/soul.seerah.tsx | /soul/seerah Seerah learning page | Public candidate | soul components; content/data unknown | Learning / Reflection Only; Not Religious Authority | Religious authority or interpretation risk | Religious boundary review |
| src/routes/soul.truth.tsx | /soul/truth truth/evidence page | Public candidate | soul components; content/data unknown | Source Candidate | Governance/canonical authority confusion | Documents 05-07 boundary review |
| src/routes/soul.roadmap.tsx | /soul/roadmap roadmap page | Public candidate | soul components; content/data unknown | Future / Planned; Not Live | Future plans may read as commitments | Status/current-state review |
| src/routes/soul.journey.tsx | /soul/journey journey page | Public candidate | soul components; content/data unknown | Prototype / Future / Planned; Not Therapy or Treatment | May imply live journey program or transformation guarantee | Claim/status and sensitivity review |
| src/routes/soul.book.tsx | /soul/book book/manuscript page | Public candidate | soul components; content/data unknown | Draft; Source Candidate | Manuscript/publication/canonical confusion | Manuscript package alignment review |
| src/routes/soul.pillars.tsx | /soul/pillars pillars index page | Public candidate | src/data/pillars.ts | Draft; Source Candidate | Pillars may imply live services | Claim/status review |
| src/routes/soul.pillars.$slug.tsx | /soul/pillars/:slug pillar detail page | Public candidate | src/data/pillars.ts | Draft; Source Candidate | Dynamic pages may expose unreviewed pillar content | Provenance and route review |
| src/routes/soul.quran.tsx | /soul/quran Quran learning page | Public candidate | soul components; content/data unknown | Learning / Reflection Only; Not Religious Authority | Religious authority/fatwa implication | Religious boundary review |
| src/routes/soul.what.tsx | /soul/what overview/explanation page | Public candidate | soul components; content/data unknown | Draft; Not Live | May overstate what meUusSoul currently is | Claim/status review |
| src/routes/soul.research.tsx | /soul/research research page | Public candidate | soul components; content/data unknown | Research blueprint / Draft | May imply completed validation | Evidence/research review |
| src/routes/_authenticated/soul.eq.lab.tsx | Authenticated EQ lab route; exact URL depends target router | Authenticated candidate | EQ content/data; lab components unknown | Internal Only; Demo / Prototype | Private or sensitive emotional content exposure | Auth boundary review; qualified review |
| src/routes/_authenticated/soul.journey.lab.tsx | Authenticated Journey lab route; exact URL depends target router | Authenticated candidate | Journey content/data unknown | Internal Only; Demo / Prototype | May imply live guided program | Auth and status review |
| src/routes/_authenticated/soul.earn.lab.tsx | Authenticated Earn lab route; exact URL depends target router | Authenticated candidate | Earn content/data | Internal Only; Demo / Prototype | May imply paid/service/income functionality | Auth and business/legal review |
| src/routes/_authenticated/soul.learn.lab.tsx | Authenticated Learn lab route; exact URL depends target router | Authenticated candidate | Learn content/data | Internal Only; Demo / Prototype | May expose draft learning manuscripts | Auth and provenance review |
| src/routes/_authenticated/soul.eq.deeper.tsx | Authenticated deeper EQ route; exact URL depends target router | Authenticated candidate | EQ content/data | Internal Only; Not Therapy or Treatment | Therapy/mental-health implication | Qualified boundary review |
| src/routes/_authenticated/soul.dlas.deeper.tsx | Authenticated deeper DLAS route; exact URL depends target router | Authenticated candidate | DLAS content/data unknown | Internal Only; Not Validated Assessment | Assessment/scoring/diagnosis implication | Qualified review; DLAS boundary review |
| src/routes/_authenticated/soul.dlas.lab.tsx | Authenticated DLAS lab route; exact URL depends target router | Authenticated candidate | DLAS content/data unknown | Internal Only; Demo / Prototype; Not Validated Assessment | May imply live assessment tool | Auth, safety, and claim/status review |
| src/routes/_authenticated/soul.learn.deeper.tsx | Authenticated deeper Learn route; exact URL depends target router | Authenticated candidate | Learn content/data | Internal Only; Learning / Reflection Only | Draft content exposure | Auth and provenance review |
| src/routes/_authenticated/soul.earn.deeper.tsx | Authenticated deeper Earn route; exact URL depends target router | Authenticated candidate | Earn content/data | Internal Only; Draft | Paid/service implication | Auth and claim/status review |
| src/routes/_authenticated/soul.journey.deeper.tsx | Authenticated deeper Journey route; exact URL depends target router | Authenticated candidate | Journey content/data unknown | Internal Only; Prototype / Demo | May imply guided transformation system | Auth and sensitivity review |

## 5. Content/Data Map Table

| Data/File Path | Content Domain | Likely Used By | Public Risk | Provenance Need | Status Label Needed | Review Needed |
|---|---|---|---|---|---|---|
| src/data/content/learn-manuscript.ts | Learn manuscript/content | soul.learn.tsx; authenticated learn routes | Draft manuscript content may be exposed as public-approved learning material | Source origin, author, version, and evidence status | Draft; Source Candidate; Learning / Reflection Only | Content provenance review; claim/status review |
| src/data/content/earn-manuscript.ts | Earn manuscript/content | soul.earn.tsx; authenticated earn routes | May imply services, earnings, paid levels, or operational offering | Source origin, business approval, claim evidence | Draft; Future / Planned where applicable | Claim/status review; legal/business boundary review |
| src/data/content/eq-manuscript.ts | Emotional intelligence manuscript/content | soul.eq.tsx; authenticated EQ routes | May imply therapy, treatment, diagnosis, or emotional support service | Source origin, sensitivity status, qualified boundary | Learning / Reflection Only; Not Therapy or Treatment | Sensitivity and qualified review |
| src/data/hubs.ts | Hub data and navigation/content structure | Soul index, hub pages, navigation components | May expose unreviewed public content and status claims | Source and status of each hub | Draft; Source Candidate; Not Live where applicable | Content map and status label review |
| src/data/pillars.ts | Pillar data and dynamic pillar content | soul.pillars.tsx; soul.pillars.$slug.tsx | Pillars may imply active services or canonical doctrine | Source and governance relationship of each pillar | Draft; Source Candidate | Documents 05-07 alignment review |

## 6. Component Map Table

| Component/File Path | Likely Purpose | Likely Used By | Compatibility Risk | Design-System Risk | Review Needed |
|---|---|---|---|---|---|
| src/components/soul/MarkdownLite.tsx | Lightweight markdown/content renderer | Manuscript/content pages | Markdown rendering compatibility and unsafe content handling | May style rich text differently from target system | Security, accessibility, and rendering review |
| src/components/soul/SoulLayout.tsx | Soul page layout wrapper | Public Soul routes and authenticated Soul routes | May assume route/layout conventions not present in target repo | Layout may conflict with current site shell | Framework and design-system review |
| src/components/soul/LegacyLibraryBanner.tsx | Banner for legacy/source-library context | Source/library or content pages | May reference legacy status not aligned with current governance | Banner tone/status labels may conflict | Claim/status and UI review |
| src/components/soul/SoulSidebar.tsx | Sidebar navigation for Soul pages | SoulLayout and route pages | Navigation may expose unapproved routes | Navigation hierarchy may conflict with live site | Route and public/private boundary review |
| src/components/soul/knowledge.tsx | Knowledge/source library component or section | Soul knowledge/truth/resources routes | May imply canonical source library authority | Source-of-Truth styling may overstate authority | Provenance and canonical-boundary review |
| src/components/soul/ChapterReader.tsx | Chapter/manuscript reading component | Learn/Earn/EQ/book content routes | May expose draft manuscript content publicly | Reader UI may make drafts feel published | Publication/status label review |
| src/components/site/SoulMegaMenu.tsx | Site-level Soul navigation mega menu | Main site navigation | May surface unapproved routes in global nav | Could conflict with existing navigation patterns | Navigation, route, and design-system review |
| src/components/soul/ | Soul component group | Soul route set | Group may depend on local assumptions and imports | Could introduce a parallel design system | Component inventory and target repo comparison |
| src/components/site/ | Site component group | Site shell/navigation | May overlap with existing site components | Global navigation/design conflict | UI/design-system review |

## 7. Public Asset / Sitemap Map

| Public Asset Path | Likely Purpose | Exposure Risk | SEO/Sitemap Risk | Review Needed |
|---|---|---|---|---|
| public/sitemap-soul.xml | Sitemap entries for Soul routes | Could expose unapproved routes or future pages | May signal public availability before approval | SEO/sitemap review; route approval review |
| public/ | Public asset folder | Any file placed here may become publicly accessible after deploy | Public files can bypass route-level review if copied blindly | Public asset inventory and deployment review |

## 8. Public/Private Boundary Map

### A. Public Route Candidates

Likely public route candidates include:
- Soul index
- AI page
- DLAS page
- Learn page
- Earn page
- Emotional Intelligence page
- Quran, Seerah, Journey, Research, Pillars, Founder, Roadmap, Resources, Support, and related Soul pages

These routes are not live and are not approved by this map.

### B. Authenticated Route Candidates

Likely authenticated route candidates include:
- src/routes/_authenticated/soul.eq.lab.tsx
- src/routes/_authenticated/soul.journey.lab.tsx
- src/routes/_authenticated/soul.earn.lab.tsx
- src/routes/_authenticated/soul.learn.lab.tsx
- src/routes/_authenticated/soul.eq.deeper.tsx
- src/routes/_authenticated/soul.dlas.deeper.tsx
- src/routes/_authenticated/soul.dlas.lab.tsx
- src/routes/_authenticated/soul.learn.deeper.tsx
- src/routes/_authenticated/soul.earn.deeper.tsx
- src/routes/_authenticated/soul.journey.deeper.tsx

These require auth boundary review before any merge or deployment.

### C. Content That Must Not Become Public Accidentally

- Unverified manuscripts
- AI/DLAS future-system claims
- Paid/level/service claims
- Authenticated-only pages
- Internal source-library or draft material
- Content without provenance/status labels
- Emotional intelligence, recovery, legal, religious, or personal context material without proper boundaries

## 9. Status Label Requirements

Required labels before any public, merge, or deployment consideration:
- Draft
- Prototype
- Demo
- Future / Planned
- Not Live
- Learning / Reflection Only
- Not Legal Advice
- Not Therapy or Treatment
- Not Religious Authority
- Not Validated Assessment
- Source Candidate
- Internal Only where applicable

## 10. Route/Content Risk Table

| Risk Area | Example | Severity | Control Needed | Notes |
|---|---|---|---|---|
| Route conflict | ZIP route overlaps existing /soul routes | High | Target repo route comparison | Do not merge until route tree is compared |
| Public/private route exposure | _authenticated routes become public accidentally | Critical | Auth boundary review | Private routes need verified protection |
| AI page implying live AI | soul.ai.tsx suggests meUus AI is available | High | Future / Planned and Not Live labels | Must not imply runtime AI or meYoo is live |
| DLAS page implying validated assessment | soul.dlas.tsx or authenticated DLAS lab sounds diagnostic | Critical | Not Validated Assessment label; qualified review | No scoring, diagnosis, or assessment authority |
| Learn/Earn/EQ content overclaim | Manuscript files become public learning/service promises | High | Claim/status review | Draft content must not read as approved public copy |
| Manuscript content without provenance | learn/earn/eq manuscript files lack source controls | High | Content provenance review | Source, version, and authority status needed |
| Status labels missing | Pages omit draft/prototype/future labels | High | Required status label pass | Labels must be visible before public use |
| Sitemap exposing unapproved routes | public/sitemap-soul.xml lists future routes | High | SEO/sitemap review | Sitemap must not publish unapproved URLs |
| Authenticated routes without auth | Lab/deeper routes rely on unavailable auth system | Critical | Target auth system comparison | Do not deploy private routes without auth verification |
| Content bundle size/performance | Large manuscript content files ship to client bundle | Medium | Performance and bundle review | Large TS content files may affect load time |
| Design-system mismatch | Soul layout/sidebar/mega menu conflict with live design | Medium | UI/design-system review | Avoid parallel or conflicting navigation patterns |
| Accessibility gaps | Reader/sidebar/menu components lack accessible behavior | Medium | Accessibility review | Keyboard, focus, contrast, and semantic structure needed |
| SEO overclaim | Page metadata or sitemap implies official public availability | High | Public-expression and SEO review | Public wording must match actual status |
| Translation/localization mismatch | Language or spiritual content loses meaning or authority boundaries | Medium | Localization and sensitivity review | Requires careful Bangla/English alignment where applicable |

## 11. Required Next Reviews Before Merge

A. Claim/status label review
B. Content provenance review
C. UI/design-system review
D. Deployment risk review
E. Target repo comparison
F. Merge plan
G. Isolated branch test
H. Typecheck/build test only after merge plan approval
I. Founder approval
J. Architecture approval

## 12. Next Recommended Action

Next Recommended Action:
Create meUusSoul Phase 1 claim/status label review

## 13. Explicit Prohibitions

- Do not publish from this map.
- Do not treat mapped routes as live.
- Do not merge this package yet.
- Do not deploy this package.
- Do not run build/dev/install commands.
- Do not overwrite live meUusSoul files.
- Do not expose authenticated/private route candidates.
- Do not treat package content as public-approved.
- Do not mark production-ready.
- Do not mark canonical.
- Do not create Document 08.
