# API Commons

Open, machine-readable API operations — a set of browser-first tools and
machine-readable building blocks, openly governed under
[apicommons.org](https://apicommons.org). Everything here speaks
[APIs.json](https://apisjson.org) and plugs into the wider
[APIs.io](https://apis.io) network.

## Tools

Browser-first, backend-free tools for discovering, documenting, validating,
governing, and reporting on the APIs you produce and consume. Most run
entirely in your browser — your tokens and data never leave it.

| Tool | What it does | Try it |
| --- | --- | --- |
| [**api-discovery**](https://github.com/api-commons/api-discovery) | A browser-first registry for API artifacts. Search APIs.io and code across GitHub/GitLab/Bitbucket, keep provenance, save locally, and commit or PR back with your own token. Roll it all into a single APIs.json 0.21 index. | [discovery.apicommons.org](https://discovery.apicommons.org) |
| [**api-documentation**](https://github.com/api-commons/api-documentation) | Standalone documentation for any APIs.json — rich HTML docs for every API, property, and inline artifact, with OpenAPI as a full reference and Arazzo as step-by-step timelines. | [documentation.apicommons.org](https://documentation.apicommons.org) |
| [**api-validator**](https://github.com/api-commons/api-validator) | A governance validator for OpenAPI (3.x **and Swagger 2.0**), AsyncAPI, Arazzo, and JSON Schema, powered by Spectral. Search Git hosts for real artifacts, lint against a best-of-breed ruleset, edit rules, and commit or PR back. | [validator.apicommons.org](https://validator.apicommons.org) |
| [**api-reusability**](https://github.com/api-commons/api-reusability) | Assess how reusable the APIs across your organization really are — discover, index as APIs.json, then score reusability and duplication rolled up by org, team, or domain. | [reusability.apicommons.org](https://reusability.apicommons.org) |
| [**mcp-install**](https://github.com/api-commons/mcp-install) | The universal install button for MCP servers — one button, every client. One-click deep links, ready-to-run CLI commands, and per-OS config snippets, driven by an open registry of client install methods. | [install.apicommons.org](https://install.apicommons.org) |
| [**api-governance-mcp**](https://github.com/api-commons/api-governance-mcp) | The AI surface of the validator — a Model Context Protocol server that lets any AI client lint OpenAPI, AsyncAPI, Arazzo, JSON Schema, APIs.json, MCP, and more, conversationally. | `npx @api-common/api-governance-mcp` |
| [**spectral-reporter**](https://github.com/api-commons/spectral-reporter) | Turn a Spectral lint run into a beautiful, self-contained HTML governance report — the `newman-reporter-htmlextra` for API governance. SARIF output and trend reports over time. | [reporter.apicommons.org](https://reporter.apicommons.org) |
| [**governance-pipeline-auditor**](https://github.com/api-commons/governance-pipeline-auditor) | Lint your linting. Scan a repo's Spectral CI setup and score it against an 8-point governance maturity rubric, then get a prioritized punch-list of fixes. CLI, GitHub Action, and browser. | [auditor.apicommons.org](https://auditor.apicommons.org) |
| [**spectral-ruleset-studio**](https://github.com/api-commons/spectral-ruleset-studio) | Turn a prose style guide into an owned, grounded, well-named Spectral ruleset — for OpenAPI 3.x, Swagger 2.0, or both. Twenty grounded starter templates included. | [studio.apicommons.org](https://studio.apicommons.org) |
| [**ruleset-commons**](https://github.com/api-commons/ruleset-commons) | A registry of adoptable, provenanced governance rulesets — adopt a real owned ruleset by reference instead of running the linter's defaults. National, industry, security, and company rulesets. | [rulesets.apicommons.org](https://rulesets.apicommons.org) |
| [**governance-pipeline**](https://github.com/api-commons/governance-pipeline) | A reference API governance pipeline you can fork — PR-gated, path-filtered, SHA-pinned, a dedicated OWASP security job, and a human-readable report. A composite GitHub Action. | [pipeline.apicommons.org](https://pipeline.apicommons.org) |
| [**spectral-owasp-ruleset**](https://github.com/api-commons/spectral-owasp-ruleset) | A grounded Spectral ruleset for the OWASP API Security Top 10 — add a real security governance layer in one line. | `npm i -D @api-common/spectral-owasp-ruleset` |

The governance tools (validator, governance-mcp, reporter, auditor, ruleset
studio, ruleset commons, governance pipeline, and the OWASP ruleset) grew out
of a field study of 1,005 real-world CI pipelines — see
[*The State of Spectral in API Pipelines*](https://papers.apievangelist.com/papers/the-state-of-spectral-in-api-pipelines/)
for the research behind them.

## Building blocks

Machine-readable API building blocks — small, focused schemas that describe
one facet of running an API program, meant to be composed together and
referenced from an [APIs.json](https://apisjson.org) index.

| Block | What it describes |
| --- | --- |
| [**guidance**](https://github.com/api-commons/guidance) | The how-to layer that turns governance rules into help. |
| [**policies**](https://github.com/api-commons/policies) | The business rules behind API governance. |
| [**rules**](https://github.com/api-commons/rules) | Spectral rulesets across many artifact types. |
| [**lifecycle**](https://github.com/api-commons/lifecycle) | The stages every API moves through. |
| [**experiences**](https://github.com/api-commons/experiences) | The developer experiences an API program offers. |
| [**teams**](https://github.com/api-commons/teams) | The people layer of API operations. |
| [**vocabulary**](https://github.com/api-commons/vocabulary) | Shared words and definitions for API operations. |
| [**use-cases**](https://github.com/api-commons/use-cases) | Named use cases an API serves. |
| [**plans**](https://github.com/api-commons/plans) | Machine-readable API access plans, tiers, and pricing. |
| [**change-log**](https://github.com/api-commons/change-log) | A machine-readable way to publish an API's changelog. |
| [**road-map**](https://github.com/api-commons/road-map) | A machine-readable way to publish an API's roadmap. |
| [**json-api**](https://github.com/api-commons/json-api) | Schemas and governance for the JSON:API standard. |
| [**interface-license**](https://github.com/api-commons/interface-license) | Apply an open license to your API's interface — its surface, not its implementation. |

## Standards, templates & examples

| Repo | What it is |
| --- | --- |
| [**api-onboarding**](https://github.com/api-commons/api-onboarding) | The API Onboarding Descriptor (AID) — a machine-readable `/.well-known/api-onboarding` document describing what it takes to onboard with an API: account, plan gates, ToS, verification, registration, and an executable flow. |
| [**problem-details-for-http-apis**](https://github.com/api-commons/problem-details-for-http-apis) | A base for using [RFC 9457 Problem Details](https://www.rfc-editor.org/rfc/rfc9457.html) for HTTP APIs in your own API. |
| [**agent-skills**](https://github.com/api-commons/agent-skills) | Reference agent skills (`SKILL.md`) for the API Commons / APIs.io ecosystem. |
| [**train-travel**](https://github.com/api-commons/train-travel) | An OpenAPI + APIs.json template for a Train Travel API — handy for demos and testing. |
| [**examples**](https://github.com/api-commons/examples) | Shared examples for the API Commons building blocks and the APIs.json ecosystem. |
| [**snacks-twilio-messages**](https://github.com/api-commons/snacks-twilio-messages) | An API Snack for AI — send a message with Twilio, described as a minimal, composable capability. |

## The hub

[**api-commons**](https://github.com/api-commons/api-commons) is the source
for [apicommons.org](https://apicommons.org) itself — the building blocks,
the tool family above, and the wider index.

## Get involved

Each repo above releases independently. Shared contribution conventions —
branch/PR/merge, the common script contract, and our security policy — live in
[CONTRIBUTING.md](https://github.com/api-commons/.github/blob/main/CONTRIBUTING.md)
and [SECURITY.md](https://github.com/api-commons/.github/blob/main/SECURITY.md).
Everything here is open source and free to fork — Apache-2.0 throughout,
except the [api-commons](https://github.com/api-commons/api-commons) hub
content, which is CC BY 3.0. [API Evangelist](https://apievangelist.com/services/)
offers expert services when you want help.
