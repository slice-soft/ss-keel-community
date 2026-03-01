# Versioning Policy — SliceSoft

All SliceSoft projects follow **Semantic Versioning (SemVer)**:

```
MAJOR.MINOR.PATCH
```

Example: `1.4.2`

---

## MAJOR

Incremented when:

- Breaking API changes are introduced
- System behavior changes in an incompatible way
- Code changes are required in the consumer to upgrade

Upgrading between major versions may require changes to existing code.

---

## MINOR

Incremented when:

- New features are added
- New capabilities or modules are introduced
- Enhancements are backward compatible

No breaking changes allowed in minor versions.

---

## PATCH

Incremented when:

- Bugs are fixed
- Internal refactors do not change behavior
- Documentation is improved
- Performance is optimized without API impact

---

## Breaking Changes Policy

Breaking changes:

- Must increment MAJOR
- Must be clearly documented in the CHANGELOG
- Should include migration guidance where possible

---

## Automation

Releases are managed with `release-please` across all repos:

- `feat:` commits increment MINOR
- `fix:` commits increment PATCH
- `feat!:` or `BREAKING CHANGE:` footer increments MAJOR

The CI/CD system in `ss-pipeline` provides reusable workflows for the release process.

---

## Stability Commitment

SliceSoft does not currently provide Long-Term Support (LTS) versions.

Instead:

- Stability is ensured through strict semantic versioning
- Automated testing on every PR
- Clear release notes
- Transparent roadmap

SliceSoft prioritizes predictable evolution over rapid, unstable change.
