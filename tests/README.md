# Tests

## Purpose

Conformance and regression test suite that verifies APS SDK artifacts comply with the normative specification.

## Responsibility

Provide automated, deterministic validation of specification artifacts, builder outputs, and reference implementations.

## Expected Contents

| Category | Description |
|----------|-------------|
| Schema validation | Structural correctness of specification inputs |
| Semantic validation | Behavioral compliance with normative rules |
| Builder integration | End-to-end build pipeline verification |
| Regression | Fixtures protecting against unintended breaking changes |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`aps/`](../aps/) | Tests validate against normative rules defined in the DSL source tree |
| [`builder/`](../builder/) | Builder integration tests verify pipeline output |
| [`examples/`](../examples/) | Examples may inform test fixtures |
| [`RFC/`](../RFC/) | Accepted RFCs require corresponding test coverage |

Test suite implementation begins in Phase 3 of [ROADMAP.md](../ROADMAP.md). No tests exist at the foundation stage.
