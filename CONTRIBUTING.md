# Contributing to API Commons projects

Thanks for contributing! These conventions are shared across the API Commons tools.

## Workflow

- **Branch → PR → merge.** Work on a short-lived branch, open a PR, let CI pass,
  squash-merge. `main` is protected and requires green CI.
- **Keep PRs focused** and say what changed and why.
- **Security** — see [SECURITY.md](./SECURITY.md); never file public issues for
  vulnerabilities.

## The script contract

Every repo exposes the same npm scripts (those that apply); CI runs them with
`--if-present`, so one workflow fits all:

| Script | Purpose |
| --- | --- |
| `lint` | static lint |
| `typecheck` | `tsc --noEmit` |
| `check` | the repo's **invariant gate** — the truth-keeper |
| `test` | unit / integration tests |
| `build` | production build |

Run `npm run check && npm run build` before you push. Each repo's `check`:

- **validator** — `check:catalog` (the bundle matches `all-rules.yaml`) ·
  `check:rulesets` (every format constructs + runs against the real engine) ·
  `check:skill-sync`
- **spec** — schema in sync with the engine · examples validate
- **api / mcp** — dogfood selfcheck / stdio smoke
- **cli** — jest

## Commit messages — Conventional Commits

Use `type(scope): summary` — `feat`, `fix`, `docs`, `chore`, `refactor`, `test`,
`ci`, `build`. This drives changelogs and semver. Breaking changes use `feat!:`
or a `BREAKING CHANGE:` footer.

## The rule catalog

The catalog is the product. Its single source of truth and pipeline are documented
in [api-validator](https://github.com/api-commons/api-validator) (`rules/all-rules.yaml`, read by apicommons.org): edit `all-rules.yaml`, regenerate
(`sync:catalog`, `export:site`, `build:catalog`), and commit the artifacts — the
`--check` gates enforce that they stay in sync.

## Releasing

See [RELEASE.md](./RELEASE.md).

By contributing you agree your contributions are licensed Apache-2.0 (the tools build on
[OpenLint](https://openlint.org), a community fork of Stoplight Spectral; attribution preserved).
