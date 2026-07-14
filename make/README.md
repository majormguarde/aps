# Make

## Purpose

Build automation — scenarios and prompts for assembling, validating, and publishing the APS DSL source tree.

## Responsibility

Host make scenarios and AI-assisted prompts used during specification authoring and SDK build workflows.

## Expected Contents

| Path | Description |
|------|-------------|
| `scenarios/` | Automated build and validation scenarios |
| `prompts/` | Prompts for AI-assisted specification authoring |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`aps/`](../aps/) | Primary target — make scenarios operate on the DSL source tree |
| [`builder/`](../builder/) | Builder pipeline invoked by make scenarios |
| [`tests/`](../tests/) | Scenarios may trigger conformance test runs |
| [`docs/`](../docs/) | Operational guides reference make workflow |

Content will be populated as corresponding roadmap phases begin.
