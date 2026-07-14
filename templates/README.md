# Templates

## Purpose

Canonical scaffolds for authoring APS SDK specification artifacts and governance documents.

## Responsibility

Ensure structural consistency across specification documents, RFCs, ADRs, and knowledge base entries without embedding domain logic.

## Expected Contents

| Artifact | Description |
|----------|-------------|
| Specification scaffolds | Standard structure for normative specification sections |
| Governance scaffolds | Templates for RFC, ADR, and TASK documents |
| Schema scaffolds | Canonical format for schema artifact authoring |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`specification/`](../specification/) | Templates produce content that lands in the normative layer |
| [`builder/`](../builder/) | Builder may consume template-generated artifacts |
| [`RFC/`](../RFC/), [`ADR/`](../ADR/), [`TASK/`](../TASK/) | Governance templates standardize proposal and decision documents |
| [`examples/`](../examples/) | Examples demonstrate template usage |

Templates will be created in Phase 4 of [ROADMAP.md](../ROADMAP.md).
