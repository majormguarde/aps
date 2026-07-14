# Architecture

This document describes the architectural model of **APS SDK** (Avangard Prompt Specification SDK).

## Design Principles

1. **Specification-first** — The APS DSL source tree in `aps/` is the single source of truth. All tooling derives from it.
2. **Separation of concerns** — Specification, tooling, knowledge, and templates are independent layers with explicit contracts.
3. **Governed evolution** — Changes to the specification require RFC review; architectural decisions require ADRs.
4. **Testable conformance** — Every normative requirement must be verifiable through automated tests in `tests/`.
5. **Industrial readiness** — The SDK is designed for long-term maintenance, versioning, and multi-team collaboration.

## Repository Layout

```
.
├── ADR/              Architecture Decision Records
├── RFC/              Specification change proposals
├── TASK/             Tracked work items
├── aps/              APS DSL source tree
├── builder/          SDK build and code generation tooling
├── docs/             Supplementary documentation
├── examples/         Reference usage examples
├── knowledge/        Domain knowledge and reference material
├── make/             Build scenarios and automation prompts
├── templates/        Authoring scaffolds
└── tests/            SDK conformance and regression tests
```

Root-level documents (`README.md`, `ARCHITECTURE.md`, `ROADMAP.md`, `CONTRIBUTING.md`, `CHANGELOG.md`) provide project-wide context. Each directory contains a `README.md` describing its purpose, responsibility, expected contents, and relationships.

## System Context

```mermaid
flowchart TB
    subgraph governance [Governance]
        ADR[ADR/]
        RFC[RFC/]
        TASK[TASK/]
    end

    subgraph core [Core]
        APS[aps/]
        Builder[builder/]
        Tests[tests/]
    end

    subgraph support [Support]
        Templates[templates/]
        Knowledge[knowledge/]
        Examples[examples/]
        Docs[docs/]
        Make[make/]
    end

    subgraph consumers [Consumers]
        IDE[IDE Integrations]
        CI[CI/CD Pipelines]
        Apps[Application Runtimes]
    end

    RFC --> APS
    ADR --> core
    TASK --> core
    APS --> Builder
    APS --> Tests
    Templates --> APS
    Make --> APS
    Knowledge --> APS
    Examples --> APS
    Builder --> consumers
    Tests --> CI
```

## APS DSL Source Tree

The `aps/` directory is the sole location for the APS language:

```
aps/
├── aps-v5.yaml       Root specification entry point
├── schema/           Structural data model
├── rules/            Decision and constraint definitions
├── checks/           Compliance check definitions
├── validators/       Field and format validators
├── actions/          Action definitions
└── tests/            Specification-level test fixtures
```

## Component Boundaries

### Governance

| Directory | Responsibility | Expected Contents |
|-----------|---------------|-------------------|
| `ADR/` | Record irreversible architectural decisions | Numbered ADR documents |
| `RFC/` | Propose and review specification changes | Numbered RFC documents |
| `TASK/` | Track implementation work with acceptance criteria | Numbered task documents |

### Core

| Directory | Responsibility | Expected Contents |
|-----------|---------------|-------------------|
| `aps/` | Define normative APS language: schema, rules, checks, validators, actions | DSL source artifacts (Phase 1) |
| `builder/` | Validate inputs and generate distributable SDK artifacts | Build pipeline, CLI, API (Phase 2) |
| `tests/` | Verify SDK conformance against the APS language | Schema, semantic, builder, regression tests (Phase 3) |

### Support

| Directory | Responsibility | Expected Contents |
|-----------|---------------|-------------------|
| `templates/` | Provide authoring scaffolds for specification and governance documents | Structural templates (Phase 4) |
| `knowledge/` | Host non-normative reference material | Glossaries, domain mappings, guides (Phase 4) |
| `examples/` | Illustrate correct usage without defining requirements | Sample artifacts and patterns (Phase 4) |
| `docs/` | Supplement root documentation with detailed guides | Authoring, builder, testing, migration guides |
| `make/` | Host build scenarios and automation prompts | Scenarios, prompts |

## Dependency Flow

```
RFC/ ──proposes──▶ aps/ ──consumed by──▶ builder/
                    │                        │
                    ├──validated by──▶ tests/ ├──output──▶ consumers
                    │
templates/ ──scaffolds──▶ aps/
make/ ──automates──▶     aps/
knowledge/ ──informs──▶   aps/
examples/ ──illustrates ▶ aps/

ADR/ ──governs──▶ all layers
TASK/ ──tracks──▶ all layers
```

## Foundation Stage Constraints

At the current foundation stage, the repository contains **infrastructure only**:

| Excluded | Reason |
|----------|--------|
| APS YAML specification content | Only empty `aps/aps-v5.yaml` placeholder is permitted |
| Builder implementation | Tooling begins in Phase 2 |
| Conformance tests | Test suite begins in Phase 3 |
| DSL runtime | Out of SDK scope |
| Rule engine | Out of SDK scope |
| Prompt content | Out of SDK scope |

## Versioning Strategy

APS SDK follows [Semantic Versioning](https://semver.org/):

- **MAJOR** — Breaking changes to the normative specification
- **MINOR** — Backward-compatible specification additions
- **PATCH** — Bug fixes, documentation, and non-normative updates

Specification versions and SDK package versions are aligned but tracked independently.

## Extension Points

Future integrations (IDE plugins, language server, package registries) consume the builder output API. Extension contracts will be defined in `aps/` as the SDK matures.
