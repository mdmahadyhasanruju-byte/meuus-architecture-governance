# Language & Knowledge Hub PR #61 Human Preview Correction Request

## 1. Correction Identity

- Correction title: Language & Knowledge Hub PR #61 Human Preview Correction Request
- PR number: `#61`
- PR title: Language & Knowledge Hub static public-preview pages
- PR URL: `https://github.com/mdmahadyhasanruju-byte/meuus-growth-connect/pull/61`
- Candidate repository path: `C:\Users\Lenovo\Documents\GitHub\meuus-growth-connect-lf`
- Source branch: `feature/language-knowledge-static-preview`
- Base branch: `main`
- Local preview URL: `http://localhost:8080/`
- Related domain: `meuussoul.com`
- Related current public gateway: `meuus.org/soul`
- Date created: 2026-07-12
- Status: Human Preview Correction Request
- Public status: Internal only
- Authority: Correction Request Only
- Canonical status: Not Canonical
- Publication status: Not Published
- Runtime status: Not Live
- Production status: Not Production Ready
- Deployment status: Not Approved

## 2. Human Preview Result

- Local preview reviewed: Yes
- All 7 routes opened: Yes
- Status block visible: Yes
- Disclaimer block visible: Yes
- Advanced-system boundary visible: Yes
- Claim <= Evidence reminder visible: Yes
- Visual/text issue found: Yes
- Founder decision: Request corrections

## 3. Issue Summary

All 7 route URLs open and metadata titles change, but the visible page body appears to remain the same Language & Knowledge Hub home content for every route. Child route-specific content for status, daily log, error log, draft set, and other child pages does not visibly render.

This means the current implementation is not ready for merge consideration. Metadata alone is not sufficient; each route must visibly render the correct route-specific public-preview body.

## 4. Required Correction

- Each approved route must render its own route-specific body content.
- `/language-knowledge` must render hub home content.
- `/language-knowledge/status` must render status/review boundary content.
- `/language-knowledge/start-with-one-word` must render one-word page content.
- `/language-knowledge/words-to-understanding` must render words-to-understanding content.
- `/language-knowledge/daily-learning-log` must render daily learning log template content.
- `/language-knowledge/error-log` must render error log template content.
- `/language-knowledge/draft-set` must render draft set index content.
- Shared safety blocks may remain shared, but route body content must differ correctly.
- Metadata alone is not sufficient.

## 5. Possible Technical Cause To Inspect

Codex should inspect:

- whether TanStack nested routes require an `Outlet`
- whether the parent route component is swallowing child route rendering
- whether route file naming created nested child routes under `language-knowledge`
- whether child routes are registered correctly in `routeTree.gen.ts`
- whether `LanguageKnowledgePreview` receives correct page data per route
- whether child routes use the parent component without overriding content
- whether pathless/layout routes are needed
- whether route definitions should be flat instead of nested

Do not prescribe a fix blindly. Inspect first, then correct the route-specific rendering problem on the safe branch.

## 6. Merge Status

- Merge approval: BLOCKED
- Publication approval: NOT APPROVED
- Deployment approval: NOT APPROVED
- Indexing approval: NOT APPROVED
- DNS/redirect change: NOT APPROVED

## 7. Required Next Action

Next Recommended Action:
Correct PR #61 route-specific rendering on safe branch without merging

## 8. Explicit Prohibitions

- Do not merge PR #61.
- Do not publish.
- Do not deploy.
- Do not change DNS or redirects.
- Do not mark pages canonical.
- Do not mark pages production-ready.
- Do not claim Language & Knowledge Hub pages are live.
- Do not claim vocabulary is verified.
- Do not claim Arabic/Quran/Seerah material is religious authority.
- Do not claim Legal Hub material is legal advice.
- Do not claim AI/DLAS/accounts/payments/certification are live.
- Do not add `reports/recommendations/` unless separately instructed.
- Do not create Document 08.
