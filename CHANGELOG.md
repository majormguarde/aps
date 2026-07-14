# Changelog

All notable changes to **APS SDK** (Avangard Prompt Specification SDK) are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- `aps/` DSL source tree with schema, rules, checks, validators, actions, tests subdirectories
- Empty `aps/aps-v5.yaml` placeholder as root specification entry point
- `make/` directory with scenarios and prompts subdirectories

### Changed

- APS language consolidated into `aps/` — single location for all specification artifacts
- Repository structure normalized to approved architecture (ADR, RFC, TASK, aps, builder, docs, examples, knowledge, make, templates, tests)
- README, ARCHITECTURE, ROADMAP updated to reflect new layout

### Removed

- `specification/` directory (content migrated to `aps/README.md`)

## [0.1.0-foundation] — 2026-07-14

### Added

- Complete APS SDK foundation architecture ([TASK-0002](TASK/0002-complete-aps-sdk-foundation.md))
- Top-level directories: ADR, RFC, TASK, builder, docs, examples, knowledge, templates, tests
- Directory README files with purpose, responsibility, expected contents, and relationships
- Root README with vision, architecture diagram, component overview, and development workflow
- Foundation stage constraints documented in ARCHITECTURE.md

### Removed

- Legacy `avangard-aps/` prototype structure
