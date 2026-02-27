# Keel Versioning Policy

Keel follows **Semantic Versioning (SemVer)**:

MAJOR.MINOR.PATCH

Example:
1.4.2

---

## MAJOR

Incremented when:

- Breaking API changes are introduced
- Module system behavior changes
- Dependency Injection behavior changes
- Core lifecycle changes

Upgrading between major versions may require code changes.

---

## MINOR

Incremented when:

- New features are added
- New modules or capabilities are introduced
- Addons gain new functionality
- Enhancements that are backward compatible

No breaking changes allowed.

---

## PATCH

Incremented when:

- Bugs are fixed
- Internal refactors do not change behavior
- Documentation improvements
- Performance optimizations without API impact

---

## Addon Alignment

Official `ss-keel-addon-*` addons should:

- Follow the same versioning philosophy
- Maintain compatibility with supported core versions
- Clearly document compatibility if version mismatch exists

---

## Breaking Changes Policy

Breaking changes:

- Must increment MAJOR
- Must be clearly documented
- Must be listed in the CHANGELOG
- Should include migration guidance

---

## Stability Commitment

Keel does not currently provide Long-Term Support (LTS) versions.

Instead:

- Stability is ensured through strict semantic versioning
- Automated testing
- Clear release notes
- Transparent roadmap

---

Keel prioritizes predictable evolution over rapid, unstable change.
