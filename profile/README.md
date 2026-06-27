# API Commons

Open, machine-readable API operations — openly governed under
[apicommons.org](https://apicommons.org).

## Spotlight Rules

An **openly-governed, progressive build of the [Spectral](https://github.com/stoplightio/spectral)
API linter** — current on security, faster on cadence, with a real ruleset
specification, a curated rule catalog, and first-class editor, app, and CI
surfaces. Start at **[spotlight-rules.com](https://spotlight-rules.com)**.

### The suite

| Project | What it is |
| --- | --- |
| [**spotlight-cli**](https://github.com/api-commons/spotlight-cli) | The linter engine + CLI — a maintained Spectral fork. `npm i -g @spotlight-rules/spotlight-cli` |
| [**spotlight-spec**](https://github.com/api-commons/spotlight-spec) | The standalone ruleset format + JSON Schema (2020-12), and the rule catalog. |
| [**spotlight-vscode**](https://github.com/api-commons/spotlight-vscode) | Lint-on-save / lint-on-type in VS Code. |
| [**spotlight-validator**](https://github.com/api-commons/spotlight-validator) | Browser governance workbench — lint, tag-filter, AI-fix, utilities. [Try it ↗](https://validator.spotlight-rules.com) |
| [**spotlight-discovery**](https://github.com/api-commons/spotlight-discovery) | Browser artifact registry — search, provenance, save / commit / PR. [Try it ↗](https://discovery.spotlight-rules.com) |
| [**spotlight-api**](https://github.com/api-commons/spotlight-api) | OpenAPI-first HTTP service over the engine (`POST /lint`). |
| [**spotlight-mcp**](https://github.com/api-commons/spotlight-mcp) | MCP server exposing linting + rulesets to AI clients. |
| [**spotlight-pipeline**](https://github.com/api-commons/spotlight-pipeline) | Governance-gate CI for GitHub / GitLab / Bitbucket / Azure / AWS. |

### The rule catalog

One curated catalog of **733 rules across 12 artifact types** (OpenAPI, AsyncAPI,
Arazzo, JSON Schema, JSON Structure, JSON-LD, APIs.json, MCP, Plans, Rate-Limits,
FinOps, Agent Skills). Every rule carries a Title Case `title`, namespaced `tags`
(`format:` / `spec:` / `experience:` / `topic:` / `owasp:`), a canonical
`reference`, and an AI **`prompt`** that fixes the rule. Rules ship at `info` by
default — educate first, raise to `warn`/`error` to enforce. Browse them in the
[rule explorer](https://spotlight-rules.com/spec/).

### Get started

- **Lint anywhere** — [spotlight-rules.com/start](https://spotlight-rules.com/start)
  routes you to the right surface (CLI, editor, browser, HTTP, AI, or CI).
- **Coming from Spectral?** Your `spectral:` rulesets and `.spectral.*` files keep
  working alongside the `spotlight:` aliases.

Latest release: **1.1.0** — all 11 `@spotlight-rules/*` packages on npm.
Contributing, the script contract, and the release runbook live in
[CONTRIBUTING.md](https://github.com/api-commons/.github/blob/main/CONTRIBUTING.md)
and [RELEASE.md](https://github.com/api-commons/.github/blob/main/RELEASE.md).

Spotlight is a fork of the open-source [Stoplight Spectral](https://github.com/stoplightio/spectral)
codebase (Apache-2.0; attribution preserved throughout).

> Naming map: GitHub org **api-commons** · npm scope **@spotlight-rules** · site **spotlight-rules.com**.
