# meUus Ecosystem: Verified Status and Next Moves

**Prepared:** 4 October 2026 (updated after workspace, provenance, and dashboard checks)
**Purpose:** establish a dependable path for four domains and four code repositories to operate as one ecosystem, with ongoing work flowing through GitHub and repeatable deployments rather than disconnected laptop copies.

## Executive conclusion

The four-domain product architecture is already clear, and the public sites exist. The current blocker is the release chain: `.org` has a verified GitHub source and Cloudflare Git build connection, and `.app` has a Git-connected Vercel project, but `.app` production is currently a CLI deployment. The `.com` SoulAI Worker and `rujbel.org` Worker show no Git connection in their Cloudflare Builds settings. Some local folders are snapshots without Git history, and the newer app preview is on a candidate branch that has not been promoted to production. Consequently, work can exist locally or in a preview while the public domain continues serving a different build.

This is a source-of-truth and release-process gap, not evidence that the product work has no value. The safe next move is to establish the canonical repositories and their deploy connections first, then promote features through reviewed builds. This report does not claim the four-repository integration is complete.

## The intended four-part ecosystem

| Domain | Intended role | Current observed status | Hosting / source evidence | Open point |
|---|---|---|---|---|
| [meuus.org](https://meuus.org) | Understand; public trust, principles, and orientation | Public foundation site is live. Its current public copy says there is no public AI analysis and no live DLAS scoring runtime; SoulAI messaging is paused during privacy/governance review. | Cloudflare Worker `meuus-growth-connect` Visit points to `https://meuus.org/`. Worker Builds shows Git repo `mdmahadyhasanruju-byte/meuus-growth-connect`, production branch `main`, root `/`, `bun run build`, `npx wrangler deploy`. Config/package fingerprints exactly match the `.org` snapshot. Provenance pins live version `3c876c8c-3280-4c28-80f2-3ce65823d4cc` (24 Aug); 5/5 public client assets match that pin. | Verify the current serving version against `main`; Cloudflare’s rebuild hook was last triggered about two months ago. Worker preview builds are not enabled. |
| [meuussoul.com](https://meuussoul.com) | Learn; learning library | Public learning home is live with English/Bangla navigation and learning resources. | Provenance pins Worker `meuussoul-com` version `99520d9f-47c7-446a-9570-1328fdd1132e` (18 Aug) and 20/20 matching client assets. Current Cloudflare DNS/settings separately show `www` proxied to ChatGPT Sites and the Worker Visit/route at `soulai.meuussoul.com`; the Learn/SoulAI hostname map needs reconciliation. | Best available source pack exists on Desktop and the domain snapshot, but neither is a Git checkout. Resolve live hostname roles, confirm server bundle/current version, then create/select and connect a dedicated GitHub repo. |
| [meuus.app](https://www.meuus.app) | Reflect and Act; authenticated bounded pilot | Production alias resolves to a Vercel deployment. The live client bundle inspected during this review does not contain the DLAS, Education System, Language Hub, or SoulAI feature labels seen in the newer preview work. | Vercel Settings → Git confirms project `meuus-app-ai` connected to `mdmahadyhasanruju-byte/meuus-app-ai`. Current production deployment `dpl_JCV4By46j6NYpzL6ZESXYBR5sbH6` is READY and has `source: cli`. Separate READY Git preview is branch `candidate/dlas-full100-packaged-20260912-final`, commit `9877d4537b49642542967fcf248c4f188418d778`; custom-domain assignment was skipped. | Reconcile production CLI source with the connected Git repo and explicitly choose a production branch; resolve candidate build/check and unpublished changes before promotion. |
| [rujbel.org](https://rujbel.org) | Remember/Prove; founder archive | Public founder archive is live and describes the wider ecosystem as in development. | Worker `rujbel-founder-archive` Domains shows production custom domain `rujbel.org`; provenance pins live version `09c5b80b-8bb3-40c4-abea-5ea62b8099b5`. Settings → Builds offers Connect, with no Git repository connected. | Available source is the domain snapshot; the provenance-named R61B source pack is absent. Reconcile the snapshot with the pinned live version, then create/select a repo and connect a reviewed production branch. |

These domain descriptions are the intended responsibilities in `00_DOMAIN_REPOSITORIES/README.md`. Public pages are useful status evidence, but do not establish which repository produced a deployment.

## Repository and source-of-truth audit

### Confirmed

- The four domain directories exist under `00_DOMAIN_REPOSITORIES`, but none is a Git checkout. They are snapshots and cannot themselves provide a commit/push/deploy workflow.
- The active app copies under `01_Production_Active/MEUUS_PRODUCTION_20260927/01-apps` are also plain folders rather than Git checkouts. The root `project_inventory.csv` is now a four-domain ledger, updated with the latest verified mapping and remaining gaps.
- A separate Git checkout exists deeply under the DLAS packaging tree: `01_Production_Active/MEUUS_PRODUCTION_20260927/services/dlas/DLAS-100Q-PACK/full-code/full-codex-context-reset-do-not/work/MEUUS_DLAS_FULL100_PACKAGED_20260912_FINAL`. It is on branch `candidate/dlas-full100-packaged-20260912-final`, at commit `9877d4537b49642542967fcf248c4f188418d778`, with origin `https://github.com/mdmahadyhasanruju-byte/meuus-app-ai.git`.
- That candidate checkout has uncommitted edits in `apps/web/src/pages/CanonicalWorkspace.tsx` and an untracked `apps/web/src/features/education/LanguageHub.tsx`. These are not in the cited Git commit or the currently verified production deployment. They must be integrated into the chosen canonical repo before they can become a dependable release.
- The `.app` Vercel preview is Git-connected to `meuus-app-ai`; the live `.app` production deployment is marked as a CLI deployment. This is a direct, concrete example of preview and production having different release paths.
- The current production `.app` HTML loads a Vite bundle. The downloaded live bundle did not include strings for DLAS, meUus Education System, Language Hub, or meUusSoulAI. The signed-in Git preview UI does expose DLAS. This is consistent with the differing source/deployment evidence above.
- A separate GitHub repo, `mdmahadyhasanruju-byte/meuus-growth-connect`, is confirmed, writable, and its package and Wrangler config blobs exactly match the `.org` domain snapshot. Cloudflare Settings → Builds directly confirms this repo is connected to `meuus-growth-connect`, with production branch `main`, root `/`, build `bun run build`, and deploy `npx wrangler deploy`.
- Vercel Settings → Git directly confirms project `meuus-app-ai` is connected to `mdmahadyhasanruju-byte/meuus-app-ai`. This connection does not change the fact that the current production deployment source is `cli`.
- Other repositories are present, but this review did not confirm a clean, authoritative one-to-one mapping for all four domain runtimes. A governance-only repository is not a runtime repository. Repository name similarity is not sufficient proof of deployment ownership.

### Not yet verified

1. The final four repository names and which account/team owns each.
2. The exact GitHub repo for the `.com` SoulAI Worker and `rujbel.org` runtime; `.org` is confirmed as `mdmahadyhasanruju-byte/meuus-growth-connect`, and `.app` Vercel is connected to `mdmahadyhasanruju-byte/meuus-app-ai`.
3. Which commit/version is currently live on each Cloudflare Worker; `.org` has a Git build connection, while `.com` and `rujbel.org` do not show one in Builds.
4. Which `.app` branch should become the canonical production branch. The preview candidate commit shows a failed status check in the GitHub view, and its local working tree includes unpublished changes.
5. Whether production has additional runtime bindings/secrets not represented in the local snapshots. Never copy or expose secret values in a report or Git repository.

## DLAS, Education, Language Hub, and SoulAI status

- The `.app` public production bundle inspected here does not show these newer feature labels.
- The signed-in preview exposes DLAS instruments. Its visible product boundaries say they are private reflection instruments, not diagnosis, scoring, AI interpretation, or professional judgment. Keep those boundaries explicit in product copy and technical behavior.
- The current candidate checkout has local edits for a meUus Education System entry and Language Hub, including English/Bangla/Arabic starter material. They are uncommitted and the build was not verified.
- A meUusSoulAI panel/menu edit was previously made in this candidate worktree. It is not proof that the production domain contains the feature or that the AI runtime is operational.
- An earlier build attempt failed because dependencies such as Vite, `lucide-react`, and `@supabase/supabase-js` were unavailable in the working environment. Therefore this report cannot claim these changes compile or are production-ready.
- Public `.org` copy currently says SoulAI messaging is paused during privacy/governance review. Align AI availability and claims across the domain, preview, and app only after the runtime, data handling, consent, and operational limits are verified.

## Product direction: AbacusAI Bot + meUus

The supplied ZIP is a useful product reference: its README describes an Electron desktop assistant with persistent chats, tools/connectors, routines, and Windows/macOS/Linux packaging. Its mobile access is through messaging integrations; it is not, by that description, a native mobile app. Treat it as a feature reference, not as a replacement for meUus’s identity, architecture, or safety boundaries. Preserve its MIT license notices if code is ever reused, and review connector permissions before adopting any behavior.

A pragmatic meUus product sequence is:

1. **Reliable web product first:** make the canonical meUus.app repo deploy reproducibly, then ship the core learning/reflection flows.
2. **Installable mobile/desktop web client:** make the responsive app a tested PWA where supported. This gives a real install path without claiming a native app.
3. **Desktop packaging:** evaluate Electron (closest to the reference) after the web app and APIs are stable; package Windows/macOS/Linux with signed, repeatable releases.
4. **Native mobile or messaging companions:** decide separately after identity, consent, data storage, connector permissions, and support expectations are defined. Do not describe the ZIP’s messaging access as a native app.
5. **Assistant capabilities:** add persistent conversations, connectors, and scheduled routines only with explicit permission boundaries, per-user data controls, revocation, and auditability.

## The operating model that will prevent laptop-only work

Keep four independently deployable runtime repositories, one per domain, and a small ecosystem manifest that maps each domain to its exact repository, production project/Worker, production hostname, and deployment method. Do not make the ecosystem manifest a fifth runtime app.

For each repository:

- `main` (or another explicitly chosen stable branch) is the production source of truth.
- Changes are made in a Git checkout, committed, and pushed to the named GitHub remote. A pull request produces a preview; a successful merge triggers the matching production deployment.
- The production host is connected to that repository. Vercel/Cloudflare build settings, root directory, build command, output directory, environment names, and custom domains are documented in the repository’s deployment runbook.
- Secrets live only in host secret storage. Local `.env` files stay ignored and out of commits.
- Keep snapshot/backup folders read-only or clearly marked as archives. Do not treat copied folders or dashboard edits as the publishing workflow.
- Every feature is considered live only after verifying its production URL and the deployment commit/version shown by the host.

## Recommended next moves, in order

### P0 — establish the four canonical repository/deployment pairs

1. Create a small verified map with exactly four rows: `domain | GitHub owner/repo | canonical branch | hosting project/Worker | production hostname | last verified commit/version`.
2. Confirm the final repository names and owner for `.com` and `rujbel.org` from GitHub and the matching project dashboards. Do not infer a mapping from similar names.
3. For `.app`, choose whether `meuus-app-ai` is the canonical repo. If yes, reconcile the production CLI deployment with that repo and its stable branch. First resolve the failed check and unpublished changes; do not assign the production domain to an unverified candidate build.
4. Recover or select a real Git checkout for each other domain. If an authoritative remote does not exist, create it from the reviewed domain snapshot while preserving history/licensing decisions and leaving secrets/build artifacts out.

### P1 — make deploys flow from Git

5. Keep the verified `.org` Git connection and verify its live deployment SHA; connect `.com` SoulAI and `rujbel.org` Workers to their verified repositories. Map each domain to the correct project. Enable preview deployments for pull requests and production deployment only from the stable branch.
6. Record build settings and required secret *names* (never values) in a runbook. Confirm successful CI/build and verify a preview URL before production.
7. For `.app`, move the desired DLAS/Education/Language Hub/SoulAI changes into the canonical checkout, review the diff, restore dependencies, and get a clean build/check before merge. Current worktree edits are not yet released.

### P2 — define how the four sites act as one ecosystem

8. Publish a shared navigation/identity map: Understand (`.org`) → Learn (`.com`) → Reflect/Act (`.app`) → Remember (`rujbel.org`), with clear links back and consistent naming.
9. Document account boundaries. Today `.com` is a public learning surface and `.app` has a sign-in/pilot boundary; do not imply shared accounts or shared data until identity integration is actually implemented and verified.
10. Keep public status, AI availability, DLAS boundaries, and privacy statements consistent with the deployed behavior.

### P3 — ship the downloadable product in stages

11. Validate responsive/PWA installability on representative desktop and mobile browsers.
12. Once web releases are stable, produce a signed desktop package and update process; then assess native mobile or messaging integrations as separate deliverables.
13. Add routines/connectors only after permission, data retention, revocation, and support behavior have been designed and tested.

## Release acceptance checklist

A domain is considered connected when all are true:

- [ ] The repository is known and the owner can push to it.
- [ ] The deployed project/Worker is linked to that repository and stable branch.
- [ ] A PR preview builds from a visible commit SHA.
- [ ] Merge creates a production deployment from the same repository and branch.
- [ ] The custom hostname serves that deployment.
- [ ] A deployed feature is checked on the public hostname after release.
- [ ] Required secret names, rollback method, and owner are documented without exposing secret values.

The ecosystem is considered connected only when all four domain rows pass this checklist and the manifest is kept current.

## Evidence and confidence notes

**Directly observed:** local directory structure and Git metadata; the app preview branch/SHA; Vercel deployment source, aliases, and Settings → Git repository; Cloudflare `.org` Git build settings and `.com`/`rujbel.org` unconnected Build settings; public page copy and visible app navigation; contents of the supplied ZIP’s README.
**Historical only:** Worker names/versions and source locations in local provenance files dated August/September 2026. Some cited source-pack paths no longer exist. These files do not prove current live Worker versions.
**Unresolved:** final four-repository map (especially `.com` and `rujbel.org`), live Cloudflare deployment SHAs, `.app` production branch/source reconciliation, and successful build of the local candidate changes.

No Git commit, push, repository creation, Cloudflare change, domain assignment, or production deployment was made as part of this audit. A deployment change would be premature while production and the candidate source are not reconciled and the candidate checks are failing/unverified.

## Workspace re-audit — 4 October 2026

The current domain snapshots carry stronger release provenance than the earlier draft captured:

- `.org` provenance pins Worker version `3c876c8c-3280-4c28-80f2-3ce65823d4cc` (24 Aug 2026) and records a 5/5 public client asset SHA match. Its Cloudflare Build settings now confirm the same-name GitHub repo and production `main` configuration. The production version still needs a fresh provider-side check against `main`.
- `.com` provenance pins Worker `meuussoul-com` version `99520d9f-47c7-446a-9570-1328fdd1132e` (18 Aug 2026), with 20/20 client assets matching. The desktop source pack named by provenance exists, and the domain snapshot is an expanded copy with the generated `dist` tree. The server bundle may be newer than the deployed build, so this does not prove the whole source tree is an exact production source.
- `.app` provenance pins the current Vercel production deployment and records the 3 October rollback that restored the authenticated app after a narrower landing-page candidate omitted it. The canonical source pack path in provenance, `D:\MEUUS_R61B_20260923-003329\app-source`, is absent. The Vercel project is Git-connected to `meuus-app-ai`, but the current production rollback and Git candidate must be compared before choosing the canonical content.
- `rujbel.org` provenance pins Worker version `09c5b80b-8bb3-40c4-abea-5ea62b8099b5`. Its source-pack path is absent; the domain snapshot is the available local recovery tree and still needs comparison to the pinned live server build.

The workspace also has separate Git checkouts that must not be mistaken for canonical production sources:

- `meuus-app-phase-one` points to `mdmahadyhasanruju-byte/meuus-app-phase-one`, not the Vercel-connected `meuus-app-ai`; it has a modified `next-env.d.ts` and untracked `package-lock.json`.
- `meuus-growth-connect-lf` points to the `.org` repo but is on feature branch `fix/meuussoul-privacy-authority-boundaries`, commit `3358618`, not production `main`.
- `meuus-app-ai` candidate branch `candidate/dlas-full100-packaged-20260912-final` has local DLAS/Education changes that remain unpublished. Preserve them while recovering the full authenticated app source.
- Archived `meuus-growth-connect-*` folders exist; folders with a familiar name are not proof of a domain/release mapping.
- GitHub account inspection found private recovery repositories `mdmahadyhasanruju-byte/meuus-org` and `mdmahadyhasanruju-byte/meuus-soul`. Their default visible branches are respectively `recovery/import-reconciled-org-source` and `recovery/import-reconciled-soul-source`; each README says recovered static source and explicitly says it is not proof of the live deployment source. `meuus-org` is therefore a duplicate/recovery candidate while the actual `.org` Worker is connected to `meuus-growth-connect`; `meuus-soul` is a possible `.com` repo candidate but still needs code/source reconciliation.
- The account also has public `mdmahadyhasanruju-byte/ruju`, but it contains only a README and is not a `rujbel.org` runtime repository. This resolves a name-based false lead, not the missing archive repo.
- GitHub CLI access is now verified as `mdmahadyhasanruju-byte` with `repo` and `workflow` scopes (4 October 2026); the owner explicitly approved the `repo` scope. Repository inspection and reviewed branch pushes are available. This clears the GitHub authentication blocker, but does not resolve canonical-source and production provenance gaps for `.app`, `.com`, and `rujbel.org`.

Git reported “dubious ownership” on the nested local checkouts under the sandbox identity. Their status was read using a command-scoped safe-directory override only; no global Git trust setting was changed. The workspace root itself is not a Git repository.

The living four-domain matrix and workflow now appear in [`ECOSYSTEM_RELEASE_MANIFEST.md`](ECOSYSTEM_RELEASE_MANIFEST.md). `00_DOMAIN_REPOSITORIES/README.md` was corrected to call these folders snapshots rather than repositories and warns that generated/dependency trees must not be pushed wholesale. No remote repositories, provider settings, hostnames, or production deployments were changed.

## Sources

- Public sites: [meuus.org](https://meuus.org), [meuussoul.com](https://meuussoul.com), [meuus.app](https://www.meuus.app), [rujbel.org](https://rujbel.org)
- Domain architecture: `D:\MEUUS_ECOSYSTEM\00_DOMAIN_REPOSITORIES\README.md`
- Active source inventory: `D:\MEUUS_ECOSYSTEM\01_Production_Active\MEUUS_PRODUCTION_20260927\01-apps\README.md`
- Candidate Git checkout: `D:\MEUUS_ECOSYSTEM\01_Production_Active\MEUUS_PRODUCTION_20260927\services\dlas\DLAS-100Q-PACK\full-code\full-codex-context-reset-do-not\work\MEUUS_DLAS_FULL100_PACKAGED_20260912_FINAL`
- Verified app candidate repository: [mdmahadyhasanruju-byte/meuus-app-ai](https://github.com/mdmahadyhasanruju-byte/meuus-app-ai)
- Verified related candidate repository: [mdmahadyhasanruju-byte/meuus-growth-connect](https://github.com/mdmahadyhasanruju-byte/meuus-growth-connect)

## Follow-up audit — additional source and account evidence (3 October 2026)

A second pass over the provenance records and connected project listings sharpened the diagnosis above:

- The `.org` and `.com` source packs referenced by their provenance records do exist on the Desktop. Both are ordinary directories without `.git`, so they are recoverable source/artifact copies but cannot currently serve as a commit-and-push source of truth. Their provenance pins Cloudflare Worker versions from August 2026 and records client asset hash comparisons made during September consolidation. Treat those as valuable release evidence, not proof of a fresh deployment today.
- `.org` is identified in its Worker config as `meuus-growth-connect`, and current dashboard evidence now confirms the repo/build link. `.com` provenance identifies Worker `meuussoul-com` and a dual-hosted ChatGPT Sites project; current DNS/dashboard evidence separates `www` ChatGPT Sites from the `soulai` Worker.
- `rujbel.org` provenance pins Worker `rujbel-founder-archive` version `09c5b80b-8bb3-40c4-abea-5ea62b8099b5` and a source pack beneath `D:\MEUUS_R61B_20260923-003329`; that R61B directory is absent from this machine now. The domain snapshot includes a production Wrangler config naming the same Worker.
- The `.app` domain snapshot has `.vercel/project.json` naming Vercel project `meuus-app-ai` and project ID `prj_m6qMDCMpGIEVduaCHAtvQLtYzI7G`. That corroborates the production project identity. It does not make the snapshot a Git checkout. Vercel lists several related projects (`meuus-app-ai`, `meuus-app-ai-deploy`, `meuus-ecosystem-app`, and multiple growth-connect-named projects), so project names alone cannot safely identify canonical deployment targets.
- GitHub search exposes `mahadyhasan1-sys/meUus-ecosystem` as a public repo, but the connected GitHub identity has pull-only permission (`push: false`). It is therefore not currently a viable write target for the four runtime repositories. The connected identity is admin/push on `mdmahadyhasanruju-byte/meuus-growth-connect`.
- The GitHub connector returns 404 for direct metadata lookup of `mdmahadyhasanruju-byte/meuus-app-ai`, even though Vercel deployment metadata identifies that repository as the preview source and the signed-in browser previously showed it. Treat its source relation as Vercel-reported, with the connector lookup inconsistency noted; do not infer that the repository is absent.

### Revised concrete state

The verified state is: `.org` Worker ↔ `mdmahadyhasanruju-byte/meuus-growth-connect` with Git builds from `main`; `.app` Vercel project ↔ `mdmahadyhasanruju-byte/meuus-app-ai`, but production currently comes from CLI; `.com` SoulAI Worker and `rujbel.org` Worker do not show Git connections. `www.meuussoul.com` separately points to ChatGPT Sites. The next work is to verify `.org` live SHA, reconcile `.app` production with its linked repo, and identify/connect the two remaining Worker sources. The four-domain/four-repository objective is not finished yet.

This follow-up supersedes the earlier broad statement that the non-app provenance paths were all missing: the `.org` and `.com` Desktop source packs are present; the cited R61B production pack for `.app`/`rujbel.org` remains absent.

### Repository mapping update — exact `.org` source fingerprint

The `.org` mapping can now be narrowed. GitHub `mdmahadyhasanruju-byte/meuus-growth-connect` has a Cloudflare Worker config and package manifest whose Git blob IDs exactly match the `.org` domain snapshot (`wrangler.jsonc`: `a092e4099ca3492c222d1a9c3fbef460fb8e4881`; `package.json`: `813042a81340053f87817991182c2251d6697054`). Its default branch is `main`, and the connected account has push/admin permission. This is strong evidence that `meuus-growth-connect` is the `.org` code repository. Cloudflare Settings → Builds later confirmed the production Worker is configured to build and deploy from that GitHub repository. Its currently serving commit/version still needs verification.

GitHub repository search also found these same-account candidates:

- `mdmahadyhasanruju-byte/meuus` — README is a generic Next.js starter and advertises `meuus.vercel.app`; it is not confirmed as any of the four intended domain runtimes.
- `mdmahadyhasanruju-byte/meuus-main` — empty README; role unknown.
- `mdmahadyhasanruju-byte/meuus-growth-connect` — exact `.org` config/package fingerprint match described above.
- `mdmahadyhasanruju-byte/meuus-architecture-governance` — governance-only by its README; explicitly not an implementation/runtime repository, so do not count it among the four.
- `mdmahadyhasanruju-byte/meuus-groeth-connect` — likely typo/duplicate; its README fetch returned 404, so do not treat it as an authoritative runtime source.
- `mahadyhasan1-sys/meUus-ecosystem` — a separate-account public repository with read-only permission for the connected identity; not suitable for current pushes without account permission changes.

This confirms the `.org` domain-to-repository pair and identifies duplicates that should not be silently promoted. Later dashboard verification confirmed `.app` Vercel Git repo connection; production remains CLI source. `.com` Worker and `rujbel.org` mappings remain unresolved. No repo or hosting configuration was changed.

### Live dashboard routing check — Cloudflare (latest observations supersede earlier notes)

Read-only inspection of the signed-in Cloudflare dashboard confirmed that Worker `meuus-growth-connect` has Visit link `https://meuus.org/`. Its Settings → Builds page directly shows Git repo `mdmahadyhasanruju-byte/meuus-growth-connect`, production branch `main`, root `/`, build command `bun run build`, and deploy command `npx wrangler deploy`. A rebuild hook for `main` was last triggered about two months ago, so verify the latest production deployment commit/version and whether it matches current `main`. The earlier statement that `.org` had no visible Git build connection was incomplete and is superseded by this check.

For `meuussoul-com`, the Cloudflare dashboard Worker `Visit` link is `https://soulai.meuussoul.com/`, while the `.com` DNS page shows `www.meuussoul.com` as a proxied CNAME to `custom-domains.chatgpt.site` and `soulai.meuussoul.com` as a Worker route. The apex has two DNS-only A records. This means the learning site hostname, the SoulAI Worker hostname, and the Cloudflare Worker settings are not a single self-evident route. Resolve which hostname is canonical for the LEARN site and document each subdomain’s role before connecting or replacing deployments. Do not point the main domain at the SoulAI Worker by assumption.

The `rujbel-founder-archive` Worker has a production custom domain `rujbel.org` in its Domains tab. Its Settings → Builds page offers Connect rather than showing a Git repository, so its production code is not currently shown as Git-connected.

For `.com`, Worker `meuussoul-com` Visit points to `https://soulai.meuussoul.com/`; its Settings → Builds page offers Connect and shows no Git repo. DNS separately routes `www.meuussoul.com` to ChatGPT Sites, and the apex has two DNS-only A records. Keep the LEARN site and SoulAI Worker mappings distinct until their roles are confirmed. No dashboard fields were edited.

### Live dashboard routing check — Vercel

Vercel project `meuus-app-ai` Settings → Git shows it connected to `mdmahadyhasanruju-byte/meuus-app-ai` (connected June 11). This confirms the Git integration exists. The currently assigned production deployment is nevertheless marked `source: cli`; the Git-connected candidate preview is on `candidate/dlas-full100-packaged-20260912-final` at `9877d4537b49642542967fcf248c4f188418d778`, and Vercel skipped custom-domain assignment. Thus `.app` needs production-source reconciliation, not a new Git connection.
