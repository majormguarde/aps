# Builder

This directory contains the **APS SDK** build and code generation tooling.

## Purpose

The builder consumes normative specification artifacts from `specification/` and produces validated, distributable SDK outputs.

## Responsibilities

| Area | Description |
|------|-------------|
| Validation | Verify specification inputs against schema and semantic rules |
| Generation | Produce schemas, parsers, and package artifacts |
| CLI | Command-line interface for local and CI usage |
| API | Programmatic interface for IDE and pipeline integrations |

## Boundaries

| Included | Excluded |
|----------|----------|
| Build pipeline implementation | Normative specification text |
| Validation engine | Conformance test definitions |
| Output format definitions | Domain-specific business logic |

## Dependencies

```
specification/  →  builder/  →  distributable artifacts
templates/      ↗
```

## Development

Builder implementation will begin in Phase 2 of the [ROADMAP](../ROADMAP.md). No builder code exists at this stage.
