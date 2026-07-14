# ADR

## Purpose

Architecture Decision Records document irreversible architectural choices made during APS SDK development.

## Responsibility

Capture the context, decision, and consequences of significant design choices so future contributors understand why the system is structured as it is.

## Expected Contents

| Artifact | Description |
|----------|-------------|
| `NNNN-short-title.md` | Individual ADR documents with status, context, decision, and consequences |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`RFC/`](../RFC/) | RFCs propose specification changes; ADRs record architectural decisions that may enable or constrain them |
| [`TASK/`](../TASK/) | Tasks reference ADRs when implementation depends on a recorded decision |
| [`aps/`](../aps/) | ADRs may mandate structural constraints on APS DSL artifacts |
| [`ARCHITECTURE.md`](../ARCHITECTURE.md) | Root architecture document; ADRs provide the decision history behind it |

Submission process: [CONTRIBUTING.md](../CONTRIBUTING.md).
