# Specification

This directory contains the normative **APS SDK** specification artifacts.

## Purpose

The specification defines the formal language, schema, semantics, and versioning rules of APS. It is the single source of truth for all tooling and conformance tests.

## Contents

| Artifact Type | Description |
|---------------|-------------|
| Language definition | Grammar, syntax, and construct definitions |
| Schema | Structural data model and validation rules |
| Semantics | Behavioral rules and constraints |
| Versioning | Compatibility policy and migration rules |

## Authority

- All builder tooling in `builder/` derives from this specification.
- All conformance tests in `tests/` validate against this specification.
- Changes require an approved RFC in `RFC/`.

## Boundaries

| Included | Excluded |
|----------|----------|
| Normative specification text | Executable code |
| Schema definitions | Builder implementation |
| Semantic rule definitions | Domain-specific business rules |
| Version compatibility matrix | Prompt content libraries |

## Development

Specification content will be authored in Phase 1 of the [ROADMAP](../ROADMAP.md).

## Versioning

Specification versions follow [Semantic Versioning](https://semver.org/). Version history is tracked in [CHANGELOG.md](../CHANGELOG.md).
