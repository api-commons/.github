# Releasing

Versions are independent semver per repo; cut a **suite milestone** when
coordinating a release across the whole stack.

## The engine

The linter engine is [OpenLint](https://github.com/openlint/openlint): the `openlint` CLI
and the `@openlint/openlint-*` packages. It's released by the OpenLint project, not here.

## Apps and sites (validator, api, mcp, pipeline, apicommons.org)

Not npm-published — released by deploy + tag.

1. `npm run check && npm run build` green.
2. Engine consumers: bump `@openlint/*` (or `openlint`) to the new engine release,
   `npm install`, re-run `check`.
3. Bump `version`, commit, tag, and let the host/Pages workflow deploy.

## Suite-milestone checklist (e.g. 1.1.0)

- [ ] Consumer apps on the published engine (`check` green on the new version).
- [ ] Coordinated `version` across the repos.
- [ ] Changelog + roadmap updated on apicommons.org.
- [ ] Catalog regenerated and every `--check` green
      (`sync:catalog`, `build:catalog`, `export:site`).
