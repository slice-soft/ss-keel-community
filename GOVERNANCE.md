# Governance Model — SliceSoft

## Overview

SliceSoft is an organization that builds open source tools focused on modularity, clarity, and automation. This document defines how decisions are made, how contributions are evaluated, and how projects in the ecosystem evolve over time.

---

## Project Ownership

SliceSoft is currently led and maintained by the Core Maintainer:

- **Juan Camilo Farfán** (juancadev-io)

The Core Maintainer has final decision authority over:

- Architectural changes across any project
- Breaking changes and major releases
- Ecosystem roadmap direction
- Quality standards and conventions
- Inclusion of new projects in the ecosystem

Additional maintainers may be appointed as projects grow.

---

## Decision Making Process

SliceSoft follows a structured but pragmatic decision model.

### Minor Changes

- Documentation improvements
- Non-breaking enhancements
- Internal refactors
- Test additions

These may be merged after review by a maintainer.

### Major Changes (RFC Required)

The following require a formal discussion before merging:

- Breaking API changes
- Architectural changes to existing systems
- Redesign of contracts between components
- Core lifecycle changes in any project
- New addon categories or projects in the ecosystem

For these cases, contributors must:

1. Open a discussion issue labeled `RFC`
2. Describe the motivation, proposal, and impact
3. Allow community feedback
4. Wait for maintainer approval before implementation

---

## Release Process

Releases are generated through automated workflows using `release-please`.

Each release:

- Must include a CHANGELOG entry
- Must follow Conventional Commits
- Must pass all CI checks
- Generates a version tag automatically

Breaking changes must be clearly documented. The versioning policy is defined in [VERSIONING.md](./VERSIONING.md).

---

## Ecosystem Governance

Projects under the `slice-soft` organization must:

- Follow the conventions defined in this repository
- Use the CI/CD workflows from `ss-pipeline` where applicable
- Use the design tokens from `ss-design-system` for web interfaces
- Maintain the same license (MIT)
- Include documentation and examples

Experimental or community projects may exist but are not considered officially supported unless explicitly listed in the documentation.

---

## Code Standards

All contributions must:

- Follow idiomatic practices for the relevant language
- Include tests where applicable
- Maintain backward compatibility unless part of a major version
- Avoid unnecessary reflection or implicit magic

SliceSoft prioritizes clarity over abstraction.

---

## Community Conduct

All repositories in the SliceSoft ecosystem follow the official [Code of Conduct](./CODE_OF_CONDUCT.md).

Respectful collaboration is mandatory.

---

## Long-Term Vision

SliceSoft aims to build tools that:

> Outlive the projects that use them. Code that any developer can read, maintain, and extend.

Governance will evolve as projects and the community grow.
