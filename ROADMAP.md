# Roadmap

Development timeline for **APS SDK** (Avangard Prompt Specification SDK).

Status labels: **Planned** · **In Progress** · **Completed**

## Phase 0 — Project Foundation

**Status:** Completed

Establish repository structure, governance processes, and architectural baseline.

| Deliverable | Status |
|-------------|--------|
| Top-level directory structure (ADR, RFC, TASK, aps, builder, docs, examples, knowledge, make, templates, tests) | Completed |
| APS DSL source tree skeleton (`aps/` with schema, rules, checks, validators, actions, tests) | Completed |
| Directory README files with purpose, responsibility, contents, and relationships | Completed |
| Root documentation (README, ARCHITECTURE, ROADMAP, CONTRIBUTING, CHANGELOG) | Completed |
| Governance workflow documentation (ADR, RFC, TASK) | Completed |
| Foundation constraints enforced (empty `aps-v5.yaml` placeholder only, no implementation) | Completed |

Tracked in [TASK-0002](TASK/0002-complete-aps-sdk-foundation.md).

## Phase 1 — Specification Core

**Status:** Planned

Define the normative APS specification in `aps/`: grammar, schema, semantics, and versioning.

| Deliverable | Status |
|-------------|--------|
| `aps-v5.yaml` specification structure | Planned |
| Schema definitions in `aps/schema/` | Planned |
| Rules and checks in `aps/rules/`, `aps/checks/` | Planned |
| Version compatibility policy | Planned |

## Phase 2 — Builder Tooling

**Status:** Planned

Implement the builder pipeline that validates and generates artifacts from `aps/` inputs.

| Deliverable | Status |
|-------------|--------|
| Builder architecture and CLI skeleton | Planned |
| Schema validation engine | Planned |
| Artifact generation pipeline | Planned |
| Package distribution format | Planned |

## Phase 3 — Conformance Suite

**Status:** Planned

Build automated tests that enforce specification compliance.

| Deliverable | Status |
|-------------|--------|
| Test framework and directory conventions | Planned |
| Schema conformance tests | Planned |
| Semantic conformance tests | Planned |
| CI integration | Planned |

## Phase 4 — Templates and Knowledge Base

**Status:** Planned

Provide authoring scaffolds and reference material for adopters.

| Deliverable | Status |
|-------------|--------|
| Authoring templates | Planned |
| Glossary and terminology | Planned |
| Integration guides | Planned |
| Reference examples | Planned |
| Make scenarios and prompts | Planned |

## Phase 5 — First Public Release

**Status:** Planned

Publish APS SDK v1.0.0 with stable specification, builder, tests, and documentation.

| Deliverable | Status |
|-------------|--------|
| Stable specification v1.0 | Planned |
| Builder v1.0 | Planned |
| Full conformance suite | Planned |
| License and release artifacts | Planned |

## Out of Scope

The following are explicitly excluded from the APS SDK repository:

- Domain-specific business logic
- DSL runtime
- Rule engine
- Prompt content libraries
- Runtime prompt execution engines

These belong in downstream consumer projects that depend on APS SDK.
