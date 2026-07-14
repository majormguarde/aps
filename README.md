# APS SDK

**Avangard Prompt Specification SDK** — an open specification and tooling framework for defining, validating, and building structured prompt systems at industrial scale.

APS SDK is not a prompt library. It is a development platform: a formal specification, reference implementations, validation tooling, and governance processes for teams that treat prompts as engineered artifacts.

## Overview

| Aspect | Description |
|--------|-------------|
| **Purpose** | Standardize how prompt specifications are authored, reviewed, versioned, and consumed |
| **Scope** | Specification, builder tooling, templates, knowledge base, and conformance tests |
| **Audience** | Platform engineers, solution architects, and teams integrating LLM workflows into production systems |

## Repository Structure

```
.
├── ADR/              Architecture Decision Records
├── RFC/              Specification change proposals
├── TASK/             Tracked work items and implementation plans
├── builder/          SDK build and code generation tooling
├── docs/             Supplementary documentation
├── knowledge/        Domain knowledge and reference material
├── specification/    Normative APS specification artifacts
├── templates/        Canonical templates for specification authoring
└── tests/            Conformance and regression tests
```

## Documentation

| Document | Description |
|----------|-------------|
| [ARCHITECTURE.md](ARCHITECTURE.md) | System architecture and component boundaries |
| [ROADMAP.md](ROADMAP.md) | Release planning and milestone timeline |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contribution workflow and governance |
| [CHANGELOG.md](CHANGELOG.md) | Version history |

## Getting Started

1. Read [ARCHITECTURE.md](ARCHITECTURE.md) to understand component boundaries.
2. Review the [ROADMAP.md](ROADMAP.md) for current development phase.
3. Follow [CONTRIBUTING.md](CONTRIBUTING.md) before submitting changes.

## Governance

Changes to the normative specification follow the RFC process documented in [RFC/README.md](RFC/README.md). Architectural decisions are recorded as ADRs in [ADR/README.md](ADR/README.md).

## License

License terms will be defined prior to the first public release.
