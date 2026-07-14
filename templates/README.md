# Templates

This directory contains canonical templates for authoring **APS SDK** specification artifacts.

## Purpose

Templates provide structural scaffolds that ensure consistency across specification documents, RFCs, ADRs, and knowledge base entries.

## Content Types

| Template | Purpose |
|----------|---------|
| Specification sections | Standard structure for normative specification documents |
| Schema definitions | Canonical format for schema artifacts |
| Authoring scaffolds | Starter structures for new specification modules |

## Boundaries

| Property | Rule |
|----------|------|
| Content | Structural only — no domain logic or sample data |
| Authority | Templates inform authoring; `specification/` remains normative |
| Maintenance | Template changes follow the RFC process when they affect normative structure |

## Relationship to Other Directories

```
templates/       →  authoring scaffolds
specification/   →  normative output
builder/         →  consumes specification
```

## Development

Templates will be created in Phase 4 of the [ROADMAP](../ROADMAP.md).
