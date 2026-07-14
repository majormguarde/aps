# Tasks

This directory contains task documents for tracked implementation work in **APS SDK**.

## Purpose

Task documents define scoped work items with clear acceptance criteria before implementation begins. They bridge roadmap milestones and pull requests.

## When to Write a Task

Create a task document when:

- Work spans multiple pull requests
- Acceptance criteria need explicit agreement before coding
- A roadmap milestone requires decomposition into deliverables

## Naming Convention

```
NNNN-short-descriptive-title.md
```

| Part | Rule |
|------|------|
| `NNNN` | Sequential four-digit number (e.g. `0001`) |
| Title | Lowercase, hyphen-separated |

**Example:** `0001-repository-foundation.md`

## Document Template

```markdown
# TASK NNNN: Title

- **Status:** Open | In Progress | Done | Cancelled
- **Assignee:** name
- **Created:** YYYY-MM-DD
- **Related:** [RFC NNNN](../RFC/NNNN-title.md), [ADR NNNN](../ADR/NNNN-title.md)

## Objective

What this task achieves.

## Scope

### In Scope

- Item

### Out of Scope

- Item

## Acceptance Criteria

- [ ] Criterion

## Implementation Notes

Technical guidance for the implementer.
```

## Lifecycle

| Status | Meaning |
|--------|---------|
| Open | Defined, not yet started |
| In Progress | Actively being implemented |
| Done | All acceptance criteria met |
| Cancelled | No longer required |

## Index

| Task | Title | Status |
|------|-------|--------|
| — | — | — |
