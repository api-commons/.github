# Releasing

Versions are independent semver per repo; cut a **suite milestone** when
coordinating a release across the whole stack.

## CLI — the engine (11 npm packages, `spotlight-cli`)

Commits follow Conventional Commits.

**Automated:** `npm run release` (multi-semantic-release derives versions from the
commits since the last tag, publishes, and tags).

**Manual coordinated** (what we run for a milestone):

1. `npm ci && npm run build && npm test` — must be green.
2. Bump every package to the target version (leave inter-package `^` ranges — they
   satisfy the new minor/patch).
3. `npm publish --workspaces --access public --dry-run`, review, then publish.
4. `git tag -a vX.Y.Z -m "Spotlight X.Y.Z" && git push --tags`.
5. `npm deprecate '@spotlight-rules/spotlight-*@<old>' 'Superseded by X.Y.Z'`.
6. Record it in `spotlight-rules/changelog.md`.

## Apps + spec + site (validator, discovery, api, mcp, spec, rules)

Not npm-published — released by deploy + tag.

1. `npm run check && npm run build` green.
2. Engine consumers: bump `@spotlight-rules/*` to the new engine, `npm install`,
   re-run `check`.
3. Bump `version`, commit, tag, and let the host/Pages workflow deploy.

## Suite-milestone checklist (e.g. 1.1.0)

- [ ] CLI built, tested, published; old version deprecated.
- [ ] Consumer apps on the published engine (`check` green on the new version).
- [ ] Coordinated `version` across the repos.
- [ ] Changelog + roadmap updated on spotlight-rules.com.
- [ ] Catalog regenerated and every `--check` green
      (`sync:catalog`, `build:catalog`, `export:site`).
