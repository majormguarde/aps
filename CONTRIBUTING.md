# Contributing

Thank you for your interest in contributing to **APS SDK** (Avangard Prompt Specification SDK).

## Code of Conduct

All participants are expected to maintain a professional and respectful collaboration environment. Report concerns to the repository maintainers.

## Development Workflow

### Branch Strategy

| Branch | Purpose |
|--------|---------|
| `main` | Stable, release-ready state |
| `develop` | Integration branch for ongoing work |
| `feature/*` | Feature development |
| `fix/*` | Bug fixes |
| `rfc/*` | Specification change proposals |
| `adr/*` | Architecture decision drafts |

### Process

1. Fork the repository or create a branch from `develop`.
2. Make changes following the conventions in this document.
3. Ensure tests pass (when the test suite is available).
4. Open a pull request against `develop`.
5. Address review feedback.
6. Merge after approval from at least one maintainer.

### Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>

[optional body]
```

| Type | Usage |
|------|-------|
| `feat` | New feature or specification addition |
| `fix` | Bug fix |
| `docs` | Documentation only |
| `refactor` | Code restructuring without behavior change |
| `test` | Test additions or corrections |
| `chore` | Maintenance tasks |

**Examples:**

```
feat(specification): add schema versioning section
docs(adr): record builder pipeline decision
fix(builder): correct validation error reporting
```

## Specification Changes

Changes to normative specification content **must** go through the RFC process:

1. Create a branch prefixed with `rfc/`.
2. Add an RFC document to `RFC/` following the template in [RFC/README.md](RFC/README.md).
3. Open a pull request for review.
4. After approval, implement the change in `specification/` in a separate PR.

## Architectural Decisions

Irreversible or high-impact architectural choices require an ADR:

1. Create a branch prefixed with `adr/`.
2. Add an ADR document to `ADR/` following the template in [ADR/README.md](ADR/README.md).
3. Open a pull request for review and discussion.

## Task Tracking

Implementation work should be documented in `TASK/` before significant development begins. See [TASK/README.md](TASK/README.md) for the task document format.

## Documentation Standards

- Use proper Markdown headings (`#`, `##`, `###`).
- Write in clear, professional English.
- Keep normative specification language precise and unambiguous.
- Link related documents (ADR, RFC, TASK) using relative paths.

## Pull Request Checklist

- [ ] Branch is up to date with `develop`
- [ ] Changes are scoped to a single concern
- [ ] Documentation is updated where applicable
- [ ] RFC or ADR is included for specification or architectural changes
- [ ] Commit messages follow Conventional Commits
- [ ] No secrets, credentials, or environment-specific configuration committed

## Questions

Open a GitHub Issue for questions, bug reports, or feature requests.
