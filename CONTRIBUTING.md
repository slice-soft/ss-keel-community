# Contributing to SliceSoft

Thank you for your interest in contributing to SliceSoft projects. This document covers the general workflow and standards that apply to **all repositories in the ecosystem**.

For repository-specific setup and requirements, refer to the `CONTRIBUTING.md` in each repo.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Ways to Contribute](#ways-to-contribute)
- [Development Workflow](#development-workflow)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Commit Messages](#commit-messages)
- [Reporting Issues](#reporting-issues)

---

## Code of Conduct

All contributors are expected to follow the [Code of Conduct](./CODE_OF_CONDUCT.md). Be respectful. We welcome contributors regardless of experience level, background, or origin. Constructive feedback is encouraged — personal attacks are not.

---

## Ways to Contribute

You don't need to write code to contribute:

- **Report a bug** — open an issue with a clear description and reproduction steps
- **Suggest a feature** — open an issue describing the problem you're trying to solve
- **Improve documentation** — fix typos, clarify examples, add missing content
- **Write tests** — increase coverage for existing functionality
- **Fix a bug** — pick an open issue labeled `good first issue` or `bug`
- **Implement a feature** — check the roadmap and open issues first to avoid duplicating work

---

## Development Workflow

1. **Open or find an issue** — all significant changes should have a corresponding issue before work begins
2. **Fork the repository** and create a branch from `main`
3. **Name your branch** descriptively — `fix/parse-body-error`, `feat/graceful-shutdown`, `docs/validation-examples`
4. **Make your changes** — keep them focused and minimal
5. **Write or update tests** — all new functionality must have tests where applicable
6. **Run the full test suite** before submitting
7. **Open a Pull Request** against `main`

---

## Pull Request Guidelines

- **One PR per concern** — do not mix bug fixes with new features
- **Add a semver label** — your PR must have one of: `patch`, `minor`, or `major`
  - `patch` — bug fix, typo, small improvement
  - `minor` — new feature, non-breaking change
  - `major` — breaking change
- **Fill out the PR description** — explain what changed and why, not just what
- **Link the related issue** — use `Closes #123` in the description
- **Keep the PR small** — large PRs are harder to review and slower to merge

---

## Commit Messages

SliceSoft follows **Conventional Commits** to support automated semantic versioning and auto-generated changelogs.

### Format

```
<type>(optional-scope): short descriptive summary
```

### Examples

```
feat: add GetEnvUint helper
fix: handle nil body in ParseBody
docs: add validation examples
test: add table-driven tests for route builder
refactor: simplify openapi path conversion
chore: update workflow permissions
```

### Rules

- Use present tense
- Keep messages concise but descriptive
- Do not use vague messages like `update`, `fix stuff`, or `wip`
- Do not mix unrelated concerns in a single commit
- Separate features, fixes, refactors, and docs into different commits

### Allowed Types

| Type | Usage |
|---|---|
| `feat` | new feature |
| `fix` | bug fix |
| `docs` | documentation changes |
| `test` | test additions or modifications |
| `refactor` | code restructuring without behavior change |
| `chore` | maintenance, tooling, config |
| `ci` | CI/CD updates |
| `perf` | performance improvements |
| `build` | build system or external dependency changes |

---

## Merge Strategy

SliceSoft uses **Squash & Merge**.

- The Pull Request title becomes the final commit in `main`
- The PR title **must** follow Conventional Commits format
- The semver label (`patch`, `minor`, `major`) must match the actual impact of the PR

### PR Title Format

```
<type>: high-level summary
```

Example:

```
feat: implement graceful shutdown
```

---

## Reporting Issues

When opening a bug report, include:

- The affected repository and version
- Minimal reproduction steps
- Expected vs actual behavior
- Error output if applicable

For security vulnerabilities, do **not** open a public issue. Follow the process in [SECURITY.md](./SECURITY.md).

---

*SliceSoft — Colombia 💙*
