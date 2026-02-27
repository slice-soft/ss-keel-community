

# Keel Governance Model

## Overview

Keel is an enterprise-ready, modular and opinionated Go application framework maintained by the SliceSoft organization.

This document defines how decisions are made, how contributions are evaluated, and how the framework evolves over time.

---

## Project Ownership

Keel is currently led and maintained by the Core Maintainer:

- Juan Camilo Farfán (juancadev-io)

The Core Maintainer has final decision authority over:

- Architectural changes
- Breaking changes
- Major releases
- Roadmap direction
- Addon approval and ecosystem standards

As the project grows, additional maintainers may be appointed.

---

## Decision Making Process

Keel follows a structured but pragmatic decision model.

### Minor Changes

- Documentation improvements
- Non-breaking enhancements
- Internal refactors
- Test additions

These may be merged after review by a maintainer.

### Major Changes (RFC Required)

The following require a formal discussion before merging:

- Breaking API changes
- Dependency Injection architecture changes
- Module system redesign
- Core lifecycle changes
- New official addon categories

For these cases, contributors must:

1. Open a discussion issue labeled `RFC`
2. Describe motivation, proposal and impact
3. Allow community feedback
4. Wait for maintainer approval before implementation

---

## Release Process

Releases are generated through automated workflows.

Each release:

- Must include a CHANGELOG entry
- Must follow Conventional Commits
- Must pass CI checks
- Must generate a version tag

Breaking changes must be clearly documented. Versioning policy is defined in [VERSIONING.md](./VERSIONING.md).

---

## Addon Ecosystem Governance

Official addons under the `ss-keel-*` namespace must:

- Follow Keel module conventions
- Maintain compatibility with supported core versions
- Include documentation and examples
- Follow the same license (MIT)

Experimental or community addons may exist but are not considered officially supported unless explicitly listed in the documentation.

---

## Code Standards

All contributions must:

- Follow idiomatic Go practices
- Include tests when applicable
- Maintain backward compatibility unless part of a major version
- Avoid unnecessary reflection or magic

Keel prioritizes clarity over abstraction.

---

## Community Conduct

All repositories in the Keel ecosystem follow the official [Code of Conduct](./CODE_OF_CONDUCT.md).

Respectful collaboration is mandatory.

---

## Long-Term Vision

Keel aims to become:

> The standard modular enterprise application framework for Go teams.

Governance will evolve as the project and community grow.
