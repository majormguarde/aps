# APS

## Purpose

DSL source tree — the single location for the APS language definition and all normative specification artifacts.

## Responsibility

Define what APS is: formal grammar, data model, behavioral rules, and compatibility policy. All tooling and tests derive from this layer.

## Expected Contents

| Path | Description |
|------|-------------|
| `aps-v5.yaml` | Root specification entry point (placeholder) |
| `schema/` | Structural data model and validation rules |
| `rules/` | Decision and constraint definitions |
| `checks/` | Compliance check definitions |
| `validators/` | Field and format validators |
| `actions/` | Action definitions triggered by rule outcomes |
| `tests/` | Specification-level test fixtures |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`RFC/`](../RFC/) | Specification changes require an approved RFC before merge |
| [`builder/`](../builder/) | Builder consumes APS artifacts as primary input |
| [`tests/`](../tests/) | SDK conformance tests validate against rules defined here |
| [`templates/`](../templates/) | Authoring scaffolds for creating specification documents |
| [`knowledge/`](../knowledge/) | Informative reference; does not override this directory |
| [`examples/`](../examples/) | Illustrative samples; not authoritative |
| [`make/`](../make/) | Build scenarios and automation prompts for the DSL tree |

Specification content will be authored in Phase 1 of [ROADMAP.md](../ROADMAP.md). Only the empty `aps-v5.yaml` placeholder exists at the foundation stage.
