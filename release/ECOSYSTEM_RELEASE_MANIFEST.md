# meUus Ecosystem Release Manifest

**Updated:** 4 October 2026
**Scope:** four public domains, their canonical code sources, and production release paths.

This is the operational map for ongoing work. The root `D:\MEUUS_ECOSYSTEM` is an organizing workspace, not a Git repository. The four directories under `00_DOMAIN_REPOSITORIES` are source snapshots, not Git checkouts. A feature is not “live” until its exact repository commit or provider version is linked to the production hostname and checked there.

## Four-domain map

| Domain / role | Live deployment evidence | Canonical source / GitHub | Release status and next action |
|---|---|---|---|
| [meuus.org](https://meuus.org) — Understand / public trust | Cloudflare Worker `meuus-growth-connect`; production branch `main`; Cloudflare Build settings show `bun run build` and `npx wrangler deploy`. Historical production version `3c876c8c-3280-4c28-80f2-3ce65823d4cc` (24 Aug 2026); the saved snapshot's 5 client assets match the pinned live assets. | `mdmahadyhasanruju-byte/meuus-growth-connect`; exact `package.json` and `wrangler.jsonc` Git object matches against the domain snapshot. | Git-based production wiring is confirmed. Confirm current serving version against the latest `main` commit; Worker preview builds are not enabled yet. |
| [meuussoul.com](https://meuussoul.com) — Learn / learning library | Cloudflare Worker `meuussoul-com`; historical production version `99520d9f-47c7-446a-9570-1328fdd1132e` (18 Aug 2026); 20/20 saved client assets match the pinned live assets. Cloudflare DNS dashboard separately showed `www` proxied to ChatGPT Sites and the Worker route on `soulai.meuussoul.com`. | Existing private GitHub repo `mdmahadyhasanruju-byte/meuus-soul` has branch `recovery/import-reconciled-soul-source`; its README explicitly labels it a recovered static foundation, not proof of production source. Best vinext source pack exists at `C:\Users\Lenovo\Desktop\meUus_R57_LEARN_Final_Candidate\20260825-062906\source`; the `.com` snapshot is a later copy. Hash comparison excluding generated/dependency/cache trees found 48 differing file entries across 448 paths, so neither source may be blindly substituted for the other. | Resolve hostname roles from current provider config before touching DNS: LEARN Worker, `www`, apex, and SoulAI route must be recorded independently. Reconcile the recovery repo, source pack and snapshot against live requirements; then connect the verified source to the correct Worker. Client artifacts match the pinned version; the server bundle from the source pack was not verified. |
| [meuus.app](https://www.meuus.app) — Reflect / Act | Vercel production deployment `dpl_JCV4By46j6NYpzL6ZESXYBR5sbH6`; production restored by rollback on 3 Oct 2026 to retain the authenticated app. A bounded landing-page candidate was rolled back because it omitted the authenticated app. | Vercel project `meuus-app-ai` is connected to `mdmahadyhasanruju-byte/meuus-app-ai`, but that connection does not prove the current production deployment came from that repo. Production provenance names canonical source pack `D:\MEUUS_R61B_20260923-003329\app-source`, which is not present. A different candidate branch `candidate/dlas-full100-packaged-20260912-final` at `9877d4537b49642542967fcf248c4f188418d778` has local edits (`CanonicalWorkspace.tsx` modified and `LanguageHub.tsx` untracked). | Recover the canonical R61B app source from its sealed source or authoritative backup, compare it to current production and the GitHub repo, then reconcile on a feature branch. Keep the authenticated app in the acceptance scope. Do not promote the candidate branch until it contains the full app and checks pass. |
| [rujbel.org](https://rujbel.org) — Remember / founder archive | Cloudflare Worker `rujbel-founder-archive`, production custom domain confirmed. Historical live version `09c5b80b-8bb3-40c4-abea-5ea62b8099b5`. | No verified GitHub repo. Domain snapshot is at `00_DOMAIN_REPOSITORIES/04_rujbel.org`. The provenance-named source `D:\MEUUS_R61B_20260923-003329\founder-source` is absent, so the snapshot is the available recovery copy, not yet re-confirmed against the full server bundle. | Review snapshot against the historical release record and live behavior, scan/exclude `.wrangler` local state and generated/dependency content, create/choose the dedicated repo, then connect it to the Worker. |

## Repository state observed in this workspace

- The `.org` Git-connected repo is also present as a local candidate at `01_Production_Active/E_Active_Projects/meUus-Ecosystem/main/01-apps/meuus.org-candidates/meuus-growth-connect-lf`, branch `fix/meuussoul-privacy-authority-boundaries`, commit `3358618`. It points to the `.org` repo but is not the connected `main` production branch.
- The separate `meuus-app-phase-one` checkout at `01_Production_Active/E_Active_Projects/meUus-Ecosystem/main/01-apps/meuus.app-candidates/meuus-app-phase-one` points to a different repo from the Vercel project. It has a modified `next-env.d.ts` and untracked `package-lock.json`; do not treat it as the current production app without review.
- The `meuus-app-ai` candidate worktree has unpublished DLAS/Education changes. Preserve those edits; do not overwrite or silently blend them into the recovered canonical app.
- Several other archived `meuus-growth-connect-*` directories exist. Their names alone do not establish a production source. Use remotes, commit ancestry, pinned provider versions, and build output fingerprints to classify them.
- GitHub's signed-in account also has private repo `mdmahadyhasanruju-byte/meuus-org` on branch `recovery/import-reconciled-org-source`. Its README labels it recovered static source, not the live production source. This is a recovery candidate/duplicate; the deployed `.org` source remains the connected `meuus-growth-connect` repo unless a deliberate migration is reviewed.
- The existing public repo `mdmahadyhasanruju-byte/ruju` contains only a README and is not a founder archive runtime repo. It must not be counted as the `rujbel.org` production repo.

## Repository hygiene before migration

- All four domain slots are currently non-Git source trees. The `.org`, `.com`, and `rujbel.org` slots each contain `.wrangler` local state; their `.gitignore` files exclude `.wrangler`, but those cache/config trees still must not be forced into a remote.
- The `.app` slot contains a 55.2 MB `packages/nextgen/.antigravity/*.pbtxt` file. The canonical-source record says next-gen is not deployed; review and exclude that generated IDE artifact from the runtime repo rather than pushing it with production code.
- A path-only check found no top-level `.env`, private-key, or credential-named files outside dependency trees in the domain slots. This is not a full secret scan; run a proper secret scanner on the staged Git index before the first push.

## Required target: four distinct runtime repositories

| Target repository | Domain | Current status |
|---|---|---|
| `mdmahadyhasanruju-byte/meuus-growth-connect` | `meuus.org` | Connected to Cloudflare production builds. |
| `mdmahadyhasanruju-byte/meuus-app-ai` | `meuus.app` | Connected to Vercel project; production-source reconciliation remains. |
| `mdmahadyhasanruju-byte/meuus-soul` (candidate; private) | `meuussoul.com` | Existing recovery branch only; README says static recovery source, not verified live source. |
| Dedicated founder archive repo (name to verify/create) | `rujbel.org` | Missing; `ruju` is README-only and not a runtime repo. Snapshot and pinned live version identified. |

Do not count governance repos, typo duplicates, the separate Phase One app, or archived branches as one of these four runtime repositories.

## Release workflow

1. Work in the canonical repository, in a feature branch. Keep source snapshots read-only during migration.
2. Compare the proposed source against the live provider version: capture the current commit/version and verify route, build entry, assets, and host bindings. Never copy secrets into Git.
3. Exclude `node_modules`, `.git`, `.wrangler` state/cache, `dist`, `build`, `.next`, `.vercel`, generated files, logs, `.env*`, keys, and provider credentials unless a specific generated artifact is intentionally required and reviewed.
4. Run the repository's documented build and relevant checks. A preview must be tied to a visible commit SHA and must preserve the full current product surface.
5. Merge to the explicitly configured production branch; let Vercel/Cloudflare deploy from Git. Avoid CLI production uploads after this migration.
6. Verify the custom host, feature flow, logs/errors, and provider's deployment SHA/version. Record the release and rollback version in that domain's runbook.

## Current external-operation access

GitHub CLI is authenticated as `mdmahadyhasanruju-byte` with the `repo` and `workflow` scopes, confirmed on 4 October 2026. The owner explicitly approved the GitHub `repo` scope. This enables private repository inspection and reviewed branch pushes. It does not prove a particular repository is the canonical runtime source; map and source verification remain required before any deployment.

## Current acceptance state

- [x] Four domain roles and production hostnames identified.
- [x] `.org` source repo and Cloudflare Git build connection identified.
- [x] `.app` Vercel repo connection and current production deployment identified.
- [x] `.com` and `rujbel.org` live Worker versions pinned by local provenance.
- [x] GitHub CLI identity and repository write scope verified; user authorized repository work.
- [ ] All four canonical repositories exist, are writable, and have reviewed source.
- [ ] Every production deployment is Git-triggered from its mapped repo and stable branch.
- [ ] `.app` production source is reconciled with its GitHub source while preserving the authenticated app.
- [ ] `.com` route mapping and source repo are resolved; Worker is Git-connected.
- [ ] `rujbel.org` source repo is created/selected and Worker is Git-connected.
- [ ] Each domain passes preview-to-production commit/version and runtime checks.

Detailed evidence, caveats, and AbacusAI reference-product direction are in [`ECOSYSTEM_STATUS_AND_NEXT_STEPS_2026-10-03.md`](ECOSYSTEM_STATUS_AND_NEXT_STEPS_2026-10-03.md). The dated source snapshots and provenance are under `00_DOMAIN_REPOSITORIES/`.
