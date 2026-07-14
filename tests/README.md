# Tests

This directory contains the **APS SDK** conformance and regression test suite.

## Purpose

Automated tests verify that specification artifacts, builder outputs, and reference implementations comply with the normative specification in `specification/`.

## Test Categories

| Category | Scope |
|----------|-------|
| Schema validation | Structural correctness of specification inputs |
| Semantic validation | Behavioral compliance with normative rules |
| Builder integration | End-to-end build pipeline verification |
| Regression | Protection against unintended breaking changes |

## Directory Conventions

```
tests/
├── schema/       Schema validation tests
├── semantic/     Semantic rule tests
├── builder/      Builder pipeline tests
└── regression/   Regression test fixtures
```

Subdirectories will be created as the test suite is implemented in Phase 3 of the [ROADMAP](../ROADMAP.md).

## Requirements

- Every normative requirement in `specification/` must have a corresponding test.
- Tests must be deterministic and runnable in CI without external dependencies unless explicitly documented.
- Test fixtures must not contain secrets or environment-specific configuration.

## Boundaries

| Included | Excluded |
|----------|----------|
| Conformance test definitions | Builder implementation |
| Test fixtures and assertions | Domain-specific business logic |
| CI configuration references | Normative specification text |
