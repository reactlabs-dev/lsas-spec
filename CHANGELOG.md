# Changelog

All notable changes to the LSAS Specification will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned for v1.0.0

This section tracks the release checklist for version 1.0.0.

#### Pre-Release Checklist

- [ ] Complete technical whitepaper in `/paper`
- [ ] Finalize all JSON schemas in `/schemas`
- [ ] Add comprehensive examples in `/examples`
- [ ] Review and validate all schemas against examples
- [ ] Complete API documentation
- [ ] Add implementation guidelines
- [ ] Review all documentation for clarity and completeness
- [ ] Ensure all links in documentation are valid
- [ ] Add security considerations section
- [ ] Add compliance guidelines section

#### Code and Schema Quality

- [ ] Run schema validation tests
- [ ] Verify all examples are valid against schemas
- [ ] Check for schema versioning consistency
- [ ] Validate JSON syntax in all schema files
- [ ] Review schema documentation completeness

#### Documentation Review

- [ ] Technical accuracy review by domain experts
- [ ] Grammar and spelling check
- [ ] Consistency check across all documents
- [ ] Update README with latest information
- [ ] Ensure CONTRIBUTING.md is up to date
- [ ] Verify CODE_OF_CONDUCT.md is appropriate

#### Legal and Compliance

- [ ] Verify LICENSE file is correct (Apache 2.0)
- [ ] Ensure all contributions are properly attributed
- [ ] Review for any proprietary or sensitive information
- [ ] Confirm compliance with healthcare regulations (HIPAA, GDPR, etc.)

#### Release Preparation

- [ ] Update version number in CITATION.cff to 1.0.0
- [ ] Update version in all schema files
- [ ] Update date-released in CITATION.cff
- [ ] Write comprehensive release notes
- [ ] Tag release in git: `git tag -a v1.0.0 -m "Release v1.0.0"`
- [ ] Create GitHub release with detailed notes
- [ ] Verify Zenodo DOI generation
- [ ] Update README badge with new DOI
- [ ] Announce release to stakeholders

#### Post-Release

- [ ] Monitor for issues reported after release
- [ ] Update documentation based on feedback
- [ ] Plan for v1.1.0 features and improvements

---

## [0.1.0] - 2026-01-28

### Added
- Initial repository structure
- README with comprehensive documentation
- CITATION.cff for academic citations
- CONTRIBUTING.md with contribution guidelines
- CODE_OF_CONDUCT.md for community standards
- GitHub issue templates
- Folder structure: `/paper`, `/schemas`, `/examples`
- Placeholder schema and example files
- Zenodo DOI minting instructions
- Apache 2.0 LICENSE

### Documentation
- Created comprehensive README with:
  - Project overview
  - Repository structure
  - Getting started guide
  - Zenodo integration instructions
  - Citation guidelines

---

## Release Notes Format

When adding new versions, use the following format:

```markdown
## [X.Y.Z] - YYYY-MM-DD

### Added
- New features or files

### Changed
- Changes to existing functionality

### Deprecated
- Features that will be removed in future versions

### Removed
- Features that have been removed

### Fixed
- Bug fixes

### Security
- Security fixes and improvements
```

[Unreleased]: https://github.com/reactlabs-dev/lsas-spec/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/reactlabs-dev/lsas-spec/releases/tag/v0.1.0
