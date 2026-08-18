# API Commons

**Open, machine-readable API operations.** If we are going to take things to the next
level with APIs and AI, there are aspects of API operations we should stop competing on
and start sharing.

Everything here is openly governed at **[apicommons.org](https://apicommons.org)**, speaks
**[APIs.json](https://apisjson.org)**, and plugs into the wider
**[APIs.io](https://apis.io)** network.

Three kinds of thing live in this organization:

- **[Tools](#tools)** — browser-first apps that run locally, so your tokens never leave.
- **[Building blocks](#building-blocks)** — machine-readable schemas for one facet of API operations.
- **[Templates](#bases-starters--templates)** — bases and starters you copy and grow.

## Tools

Browser-first and backend-free — everything runs in your browser, so your tokens and
data never leave it. Full index at **[apicommons.org/tools](https://apicommons.org/tools/)**.

| Tool | What it does | Try it |
| --- | --- | --- |
| [**api-validator**](https://github.com/api-commons/api-validator) | Browser-first API governance validator for OpenAPI, AsyncAPI, Arazzo, and JSON Schema — powered by Spectral, with Swagger 2.0 parity. Search Git hosts for real artifacts, lint against a best-of-breed ruleset, edit rules, and commit or PR back. No backend | [validator.apicommons.org](https://validator.apicommons.org) |
| [**api-discovery**](https://github.com/api-commons/api-discovery) | Browser-first registry for API artifacts — search APIs.io + GitHub/GitLab/Bitbucket, keep provenance, save locally or commit/PR to git, and edit | [discovery.apicommons.org](https://discovery.apicommons.org) |
| [**api-documentation**](https://github.com/api-commons/api-documentation) | Standalone documentation for any APIs.json — rich, portable HTML docs for every API, property, and inline OpenAPI/Arazzo artifact. Supports APIs.json 0.11–0.21 | [documentation.apicommons.org](https://documentation.apicommons.org) |
| [**api-experience**](https://github.com/api-commons/api-experience) | A DX/AX visual layer for any APIs.json — see each REST operation flow to its MCP tool and Agent Skill, with a free/paid coverage scorecard | [experience.apicommons.org](https://experience.apicommons.org) |
| [**api-governance-graph**](https://github.com/api-commons/api-governance-graph) | Bind your API governance building blocks — policies, rules, pipelines, and specs — into one navigable graph with a Gaps view | [graph.apicommons.org](https://graph.apicommons.org) |
| [**api-governance-mcp**](https://github.com/api-commons/api-governance-mcp) | A Model Context Protocol (MCP) server that lints API artifacts against a best-of-breed API governance ruleset from any AI client. Powered by Spectral | — |
| [**api-platform**](https://github.com/api-commons/api-platform) | Define your company's API stack as an APIs.json (type: platform) — browse APIs.io, drag providers into groups, pick operations & properties per provider, export a merged OpenAPI stack for AI context | [platform.apicommons.org](https://platform.apicommons.org) |
| [**api-reusability**](https://github.com/api-commons/api-reusability) | Assess API reusability across your organization — discover (apis.io/GitHub/HAR/gateways), index as APIs.json, and score reuse per API and per org/team/domain. Runs in your browser | [reusability.apicommons.org](https://reusability.apicommons.org) |
| [**api-tags**](https://github.com/api-commons/api-tags) | API Tags — explore and normalize the tag vocabulary across an API catalog | [tags.apicommons.org](https://tags.apicommons.org) |
| [**codefirst-governance**](https://github.com/api-commons/codefirst-governance) | A browser-first tool that meets code-first API teams where they are — fingerprint the OpenAPI generator from a generated spec, separate the governance findings that must be fixed in code (because the spec is regenerated) from spec-authoring findings, and map each one to the exact code annotation that fixes it | [codefirst.apicommons.org](https://codefirst.apicommons.org) |
| [**component-library**](https://github.com/api-commons/component-library) | A browser-first tool for a versioned, reusable API model/component library — author or import a library of named JSON Schemas, see which OpenAPI specs consume each model, and classify a version bump as breaking or non-breaking across every consumer while surfacing near-duplicate model drift | [library.apicommons.org](https://library.apicommons.org) |
| [**context-gate**](https://github.com/api-commons/context-gate) | Consumer-centric API governance: choose what operations/fields your APIs expose to agents; emit a governed Tyk API + MCP surface and a Spectral ruleset (PII/secrets/compliance). Browser-first | [contextgate.apicommons.org](https://contextgate.apicommons.org) |
| [**governance-agent-export**](https://github.com/api-commons/governance-agent-export) | Export an API governance ruleset into agent-native artifacts — AGENTS.md, system prompt, remediation prompt pack, rule digest. Browser-first | [agents.apicommons.org](https://agents.apicommons.org) |
| [**governance-baseline**](https://github.com/api-commons/governance-baseline) | A browser-first tool to make Spectral/Spotlight governance adoptable on a legacy estate — snapshot a baseline of the violations you have today, then ratchet: fail only NEW violations while baselined ones are suppressed, track a warning budget, and burn the baseline down to zero | [baseline.apicommons.org](https://baseline.apicommons.org) |
| [**governance-certification**](https://github.com/api-commons/governance-certification) | Issue and verify tamper-evident API governance certificates — SHA-256 fingerprint lets consumers re-verify an API passed a ruleset at a profile. Browser-first | [certification.apicommons.org](https://certification.apicommons.org) |
| [**governance-coverage**](https://github.com/api-commons/governance-coverage) | Measure how much of your API description your governance rules actually check — coverage by section, dead rules, per-rule reach. Browser-first | [coverage.apicommons.org](https://coverage.apicommons.org) |
| [**governance-pipeline**](https://github.com/api-commons/governance-pipeline) | A reference API governance pipeline you can fork — PR-gated, path-filtered, SHA-pinned, OWASP security job, HTML report. The blueprint from the State of Spectral research | — |
| [**governance-pipeline-auditor**](https://github.com/api-commons/governance-pipeline-auditor) | Lint your linting — audit a repo's Spectral CI setup against an 8-point API governance maturity rubric. CLI + GitHub Action + | [auditor.apicommons.org](https://auditor.apicommons.org) |
| [**governance-scorecard**](https://github.com/api-commons/governance-scorecard) | A browser-first tool for the longitudinal view of API governance — ingest a series of Spectral snapshots over time, compute a 0–100 health score per spec, and see health trends and the growing problem lists so you can act before a spec goes the wrong direction | [scorecard.apicommons.org](https://scorecard.apicommons.org) |
| [**governance-waivers**](https://github.com/api-commons/governance-waivers) | Sanctioned, owned, expiring API governance exceptions — reconcile a machine-readable waivers file against Spectral output. Browser-first | [waivers.apicommons.org](https://waivers.apicommons.org) |
| [**mcp-install**](https://github.com/api-commons/mcp-install) | The universal install button for MCP servers — one button, every client. Hosted chooser, embeddable web component, and an open registry of MCP client install methods | [install.apicommons.org](https://install.apicommons.org) |
| [**rule-federation**](https://github.com/api-commons/rule-federation) | A federated API governance rule registry — a central baseline plus the domains that adopt it, as a matrix of inherit / override / waive / promote | [federation.apicommons.org](https://federation.apicommons.org) |
| [**ruleset-commons**](https://github.com/api-commons/ruleset-commons) | A registry of adoptable, provenanced API governance rulesets — adopt a real owned ruleset by reference instead of the defaults | [rulesets.apicommons.org](https://rulesets.apicommons.org) |
| [**spec-review**](https://github.com/api-commons/spec-review) | A browser-first, ref-resolving design-diff for OpenAPI (and AsyncAPI/Arazzo) — paste an old and a new spec, resolve $ref so reviewers see the real shape, and get a stakeholder-friendly, breaking-flagged change list plus a copyable Markdown summary for the PR | [review.apicommons.org](https://review.apicommons.org) |
| [**spectral-reporter**](https://github.com/api-commons/spectral-reporter) | Turn Spectral lint output into a rich, self-contained HTML API governance report — the newman-reporter-htmlextra for API governance. CLI + | [reporter.apicommons.org](https://reporter.apicommons.org) |
| [**spectral-ruleset-studio**](https://github.com/api-commons/spectral-ruleset-studio) | Turn a prose style guide into an owned, grounded, well-named Spectral ruleset | [studio.apicommons.org](https://studio.apicommons.org) |
| [**toolsmith**](https://github.com/api-commons/toolsmith) | Forge MCP tools and Agent Skills from your OpenAPI — a browser-first workbench for designing the agent layer of an API | [toolsmith.apicommons.org](https://toolsmith.apicommons.org) |

The governance tools grew out of a field study of 1,005 real-world CI pipelines — see
[*The State of Spectral in API Pipelines*](https://papers.apievangelist.com/papers/the-state-of-spectral-in-api-pipelines/)
for the research behind them.

## Rulesets

Adoptable, provenanced Spectral rulesets. Every rule carries a stable id, a description
quoting the specification it comes from, and a `documentationUrl` pointing at the
section — not a homepage. Built-in Spectral functions only, so they run anywhere
Spectral runs. Browse them all at **[rulesets.apicommons.org](https://rulesets.apicommons.org)**.

| Ruleset | What it governs |
| --- | --- |
| [**spectral-owasp-ruleset**](https://github.com/api-commons/spectral-owasp-ruleset) | A grounded Spectral ruleset for the OWASP API Security Top 10 — add a real security governance layer in one line |
| [**spectral-api-authorization-ruleset**](https://github.com/api-commons/spectral-api-authorization-ruleset) | A curated, owned, grounded Spectral ruleset for the API Authorization Profile — lint your OpenAPI and OAuth AS metadata against OAuth 2.1 / FAPI 2.0 at two tiers (normal/high) |
| [**spectral-problem-details-ruleset**](https://github.com/api-commons/spectral-problem-details-ruleset) | A curated, owned, grounded Spectral ruleset for RFC 9457 Problem Details for HTTP APIs |
| [**spectral-fhir-ruleset**](https://github.com/api-commons/spectral-fhir-ruleset) | A curated, owned, grounded Spectral ruleset for HL7 FHIR R4 and R5 RESTful APIs |

## Building blocks

Small, focused schemas describing one facet of running an API program — composed
together and referenced from an [APIs.json](https://apisjson.org) index.

| Block | What it describes |
| --- | --- |
| [**plans**](https://github.com/api-commons/plans) | The plans schema for the API Commons — machine-readable API access plans, tiers, and pricing |
| [**rate-limits**](https://github.com/api-commons/rate-limits) | The rate limits schema for the API Commons — a machine-readable way to publish the quotas an API enforces |
| [**versioning**](https://github.com/api-commons/versioning) | The versioning schema for the API Commons — a machine-readable way to publish how an API is versioned |
| [**features**](https://github.com/api-commons/features) | The features schema for the API Commons — a machine-readable way to publish what an API can do |
| [**benefits**](https://github.com/api-commons/benefits) | The benefits schema for the API Commons — a machine-readable way to publish the outcomes an API claims |
| [**integrations**](https://github.com/api-commons/integrations) | The integrations schema for the API Commons — a machine-readable way to publish an API's connector catalog |
| [**change-log**](https://github.com/api-commons/change-log) | The change log schema for the API Commons — a machine-readable way to publish an API's changelog |
| [**road-map**](https://github.com/api-commons/road-map) | The road map schema for the API Commons — a machine-readable way to publish an API's roadmap |
| [**lifecycle**](https://github.com/api-commons/lifecycle) | Machine-readable API lifecycle building blocks for the API Commons — the stages every API moves through |
| [**policies**](https://github.com/api-commons/policies) | Machine-readable API policy building blocks for the API Commons — the business rules behind API governance |
| [**rules**](https://github.com/api-commons/rules) | Machine-readable API governance rules for the API Commons — Spectral rulesets across many artifact types |
| [**guidance**](https://github.com/api-commons/guidance) | Machine-readable API guidance building blocks for the API Commons — the how-to layer that turns governance rules into help |
| [**experiences**](https://github.com/api-commons/experiences) | Machine-readable API experience building blocks for the API Commons — the developer experiences an API program offers |
| [**teams**](https://github.com/api-commons/teams) | Machine-readable team building blocks for the API Commons — the people layer of API operations |
| [**vocabulary**](https://github.com/api-commons/vocabulary) | Machine-readable API vocabulary building blocks for the API Commons — shared words and definitions for API operations |
| [**use-cases**](https://github.com/api-commons/use-cases) | Machine-readable API use-case building blocks for the API Commons |
| [**interface-license**](https://github.com/api-commons/interface-license) | The API Commons Interface License — apply an open license to your API's interface (its surface, not its implementation) |

## Bases, starters & templates

A **starter** is the smallest document that is still correct and worth copying. A
**base** is a full working template for a real domain — the whole error contract,
pagination, conditional writes, merge-patch. Every base errors the same way, using
[RFC 9457](https://www.rfc-editor.org/rfc/rfc9457) problem details, so adopting more
than one gives your clients a single error format.

| Repo | What it is |
| --- | --- |
| [**starters**](https://github.com/api-commons/starters) | The smallest correct version of each artifact in the API Commons stack — starter OpenAPI, APIs.json and JSON Schema you copy and grow |
| [**accounts**](https://github.com/api-commons/accounts) | A base Accounts API for the API Commons — the account lifecycle every service reinvents, described once |
| [**images**](https://github.com/api-commons/images) | A base Images API for the API Commons — upload, metadata, renditions and deletion, described once |
| [**videos**](https://github.com/api-commons/videos) | A base Videos API for the API Commons — upload, transcoding, playback renditions and captions, described once |
| [**train-travel**](https://github.com/api-commons/train-travel) | This is the repository for managing the APIs.json for the Train Travel API template |
| [**problem-details-for-http-apis**](https://github.com/api-commons/problem-details-for-http-apis) | This is a base for using Problem Details for HTTP APIs in your API |

## Specifications & examples

| Repo | What it is |
| --- | --- |
| [**api-onboarding**](https://github.com/api-commons/api-onboarding) | API Onboarding Descriptor (AID) — a machine-readable /.well-known/api-onboarding document describing what it takes to onboard with an API: account, plan gates, ToS, verification, registration mechanisms, and an executable flow |
| [**api-authorization**](https://github.com/api-commons/api-authorization) | API Authorization Profile — a jurisdiction-neutral, two-tier, machine-checkable profile for securing APIs with OAuth 2.1 and FAPI 2.0. An API Commons spec |
| [**json-api**](https://github.com/api-commons/json-api) | JSON:API artifacts for the API Commons — schemas and governance for the JSON:API standard |
| [**examples**](https://github.com/api-commons/examples) | Shared examples for the API Commons building blocks and the APIs.json ecosystem |
| [**snacks-twilio-messages**](https://github.com/api-commons/snacks-twilio-messages) | This is an API Snack for AI to send message with Twilio |

## Spotlight

An openly-governed build of the Spectral linter, and the ruleset format as a
standalone specification.

| Repo | What it is |
| --- | --- |
| [**spotlight-rules**](https://github.com/api-commons/spotlight-rules) | Website for Spotlight Rules — the openly-governed build of the Spectral API linter |
| [**spotlight-spec**](https://github.com/api-commons/spotlight-spec) | The Spectral ruleset format as a standalone specification and JSON Schema — normative, independently versioned, implementable by anyone |
| [**spotlight-tools**](https://github.com/api-commons/spotlight-tools) | Spectral CLI — a maintained, openly-governed API Commons build of the Spectral linter. Reference implementation of the Spectral ruleset specification |

## The hub

[**api-commons**](https://github.com/api-commons/api-commons) is the source for
[apicommons.org](https://apicommons.org) itself — the building blocks, the tool index,
the bases and starters, and the rule catalog.

## Licensing

Two licenses, split by what a thing *is*:

- **Artifacts** — schemas, rulesets, fixtures, examples, and API descriptions — are
  **CC BY-NC-SA 4.0** (Attribution–NonCommercial–ShareAlike).
- **Code** — the browser tools, validators, test harnesses, and packaging — is
  **Apache-2.0**.

Repos carrying both ship both: `LICENSE` for the artifacts, `LICENSE-CODE` for the code.
The [spectral](https://github.com/api-commons/spectral) and
[spotlight-tools](https://github.com/api-commons/spotlight-tools) builds keep the
Apache-2.0 they inherit from upstream.

## Get involved

Each repo releases independently. Shared conventions — branch/PR/merge, the common script
contract, and the security policy — live in
[CONTRIBUTING.md](https://github.com/api-commons/.github/blob/main/CONTRIBUTING.md) and
[SECURITY.md](https://github.com/api-commons/.github/blob/main/SECURITY.md).

Planned and in-flight work is tracked in
[**roadmap**](https://github.com/api-commons/roadmap).
[API Evangelist](https://apievangelist.com/services/) offers expert services when you
want help.
