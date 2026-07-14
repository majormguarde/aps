# Specification

## Purpose

Normative APS specification artifacts — the single source of truth for the SDK language, schema, semantics, and versioning.

## Responsibility

Define what APS is: formal grammar, data model, behavioral rules, and compatibility policy. All tooling and tests derive from this layer.

## Expected Contents

| Artifact | Description |
|----------|-------------|
| Language definition | Grammar, syntax, and construct definitions |
| Schema | Structural data model and validation rules |
| Semantics | Behavioral rules and constraints |
| Versioning | Compatibility policy and migration rules |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`RFC/`](../RFC/) | Specification changes require an approved RFC before merge |
| [`builder/`](../builder/) | Builder consumes specification artifacts as primary input |
| [`tests/`](../tests/) | Conformance tests validate against normative rules defined here |
| [`templates/`](../templates/) | Authoring scaffolds for creating specification documents |
| [`knowledge/`](../knowledge/) | Informative reference; does not override this directory |
| [`examples/`](../examples/) | Illustrative samples; not authoritative |

Specification content will be authored in Phase 1 of [ROADMAP.md](../ROADMAP.md). No specification files exist at the foundation stage.
