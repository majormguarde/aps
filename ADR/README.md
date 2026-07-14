# Architecture Decision Records

This directory contains Architecture Decision Records (ADRs) for **APS SDK**.

## Purpose

ADRs document significant architectural decisions: context, options considered, decision, and consequences. They provide a durable audit trail for future contributors.

## When to Write an ADR

Create an ADR when a decision:

- Affects multiple components or teams
- Is difficult or expensive to reverse
- Establishes a pattern others must follow
- Resolves a technical disagreement

## Naming Convention

```
NNNN-short-descriptive-title.md
```

| Part | Rule |
|------|------|
| `NNNN` | Sequential four-digit number (e.g. `0001`) |
| Title | Lowercase, hyphen-separated |

**Example:** `0001-specification-first-architecture.md`

## Document Template

```markdown
# NNNN. Title

- **Status:** Proposed | Accepted | Deprecated | Superseded by [NNNN](NNNN-title.md)
- **Date:** YYYY-MM-DD
- **Authors:** name

## Context

What is the issue or force driving this decision?

## Decision

What is the change being proposed or enacted?

## Consequences

What becomes easier or harder as a result?
```

## Lifecycle

| Status | Meaning |
|--------|---------|
| Proposed | Under review |
| Accepted | Approved and in effect |
| Deprecated | No longer recommended |
| Superseded | Replaced by a newer ADR |

## Index

| ADR | Title | Status |
|-----|-------|--------|
| — | — | — |
