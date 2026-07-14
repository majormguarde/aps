# Request for Comments

This directory contains RFCs (Request for Comments) for changes to the **APS SDK** normative specification.

## Purpose

RFCs provide a structured review process for specification changes before they are merged into `specification/`.

## When to Write an RFC

Create an RFC when proposing:

- New specification sections or constructs
- Breaking changes to existing specification behavior
- Deprecation of specification features
- Changes to versioning or compatibility policy

## Naming Convention

```
NNNN-short-descriptive-title.md
```

| Part | Rule |
|------|------|
| `NNNN` | Sequential four-digit number (e.g. `0001`) |
| Title | Lowercase, hyphen-separated |

**Example:** `0001-schema-versioning-format.md`

## Document Template

```markdown
# RFC NNNN: Title

- **Status:** Draft | Review | Accepted | Rejected | Withdrawn
- **Author:** name
- **Created:** YYYY-MM-DD
- **Updated:** YYYY-MM-DD

## Summary

One-paragraph overview of the proposal.

## Motivation

Why is this change needed?

## Detailed Design

Technical specification of the proposed change.

## Backward Compatibility

Impact on existing implementations and migration path.

## Alternatives Considered

Other approaches and why they were not chosen.

## Unresolved Questions

Open items requiring further discussion.
```

## Review Process

1. Author submits RFC as a pull request with branch prefix `rfc/`.
2. Maintainers and stakeholders review within the PR discussion.
3. RFC status is updated based on review outcome.
4. Accepted RFCs are implemented in `specification/` via a separate pull request.

## Index

| RFC | Title | Status |
|-----|-------|--------|
| — | — | — |
