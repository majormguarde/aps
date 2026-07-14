# Builder

## Purpose

The builder is the SDK tooling layer that validates specification inputs and generates distributable artifacts.

## Responsibility

Provide the build pipeline, validation engine, CLI, and programmatic API for consuming APS specification artifacts.

## Expected Contents

| Artifact | Description |
|----------|-------------|
| Build pipeline | Source that parses, validates, and generates SDK outputs |
| CLI | Command-line interface for local and CI usage |
| API | Programmatic interface for IDE and pipeline integrations |
| Configuration | Builder-specific settings (not normative specification files) |

## Relationships

| Directory | Relationship |
|-----------|--------------|
| [`aps/`](../aps/) | Primary input — builder consumes APS DSL source artifacts |
| [`templates/`](../templates/) | Authoring scaffolds that feed into the build pipeline |
| [`tests/`](../tests/) | Conformance tests verify builder output against the specification |
| [`examples/`](../examples/) | Illustrative inputs for builder validation during development |

Implementation begins in Phase 2 of [ROADMAP.md](../ROADMAP.md). No builder code exists at the foundation stage.
