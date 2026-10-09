# Contributing to KomikHQ

Thank you for your interest in contributing to **KomikHQ**. We are committed to building high-performance, edge-distributed infrastructure for digital comic reading and delivery.

This document outlines the workflow, coding standards, and expectations for contributing across all repositories within the KomikHQ organization.

---

## Code of Conduct

All contributors and participants are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md). Please report any violations to organization maintainers promptly.

---

## Development Principles

1. **Edge-First and Performance-Conscious**: Strive for minimal bundle sizes, zero layout shifts, and sub-second responses.
2. **Strict Type Safety**: All TypeScript code must pass strict type checks (`tsc --noEmit`). Avoid using `any` unless explicitly justified in code comments.
3. **Modular and Readable**: Keep functions focused, self-documenting, and free of redundant side-effects.

---

## Branching Strategy

We follow a structured branch naming convention:

- `feat/<scope>-<description>`: New features or capabilities (e.g., `feat/reader-infinite-scroll`)
- `fix/<scope>-<description>`: Bug fixes (e.g., `fix/api-cors-headers`)
- `perf/<scope>-<description>`: Performance optimizations
- `refactor/<scope>-<description>`: Code restructuring without functional changes
- `docs/<scope>-<description>`: Documentation changes or additions
- `chore/<scope>-<description>`: Tooling, dependency updates, or pipeline adjustments

---

## Commit Message Conventions

We adhere strictly to [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short description in present tense>

[optional body explaining motivation and context]

[optional footer(s), e.g., Closes #123]
```

### Examples
- `feat(api): add edge caching headers for chapter manifests`
- `fix(reader): resolve horizontal scroll jitter on mobile safari`
- `perf(db): optimize chapter index queries using compound keys`

---

## Pull Request Workflow

1. **Fork or Branch**: Create a descriptive branch from `main`.
2. **Develop and Verify**:
   - Run type checks (`pnpm typecheck` or `npm run typecheck`).
   - Run linter (`pnpm lint` or `npm run lint`).
   - Test locally with realistic data.
3. **Submit Pull Request**:
   - Provide a clear summary and motivation.
   - Reference related issues (`Fixes #<issue_number>`).
   - Complete the standard Pull Request checklist.
4. **Code Review**: Address feedback constructively. Once approved by maintainers and CI passes, your changes will be merged via Squash and Merge.

---

## Reporting Bugs and Requesting Features

- Please use the official [GitHub Issue Forms](https://github.com/komikhq/.github/issues/new/choose) to report bugs or suggest enhancements.
- For sensitive security vulnerabilities, do not create a public issue. Refer to [SECURITY.md](SECURITY.md) instead.
