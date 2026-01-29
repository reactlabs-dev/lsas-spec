# Changelog

All notable changes to the LSAS Specification will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned
- Worked scenarios expansion (e.g., telehealth workflow, EHR tool firewall, IDE codegen)
- Operational model deepening (policy pack lifecycle, release gates, HITL workflows)
- Schema hardening (stricter typing, enums, required fields, versioning strategy)
- Diagram source standardization (Mermaid sources + optional exports)

> Release checklist note: keep operational checklists in a separate file (e.g., `/RELEASE_CHECKLIST.md`)
> rather than inside the changelog.

---

## [1.0.1] - 2026-01-28

### Added
- `NOTICE` — attribution notice for LSAS and project origin
- `TRADEMARK.md` — naming guidance for “LSAS / LSAS Framework” (nominative use vs branding)

### Changed
- `README.md` — improved citation/attribution guidance and repository structure documentation
- Documentation polish across examples/diagrams references (no specification behavior changes)

### Notes
- Documentation/attribution patch release only. No changes to LSAS schemas or core specification behavior.

---

## [1.0.0] - 2026-01-28

### Added
- LSAS Technical Whitepaper / Specification v1.0.0 in `/paper`
- Initial JSON Schemas in `/schemas`:
  - `lsas-safety-report.schema.json`
  - `claim-to-citation-map.schema.json`
- Examples in `/examples`:
  - Safety Report example(s)
  - Claim-to-citation map example(s)
  - Risk classification example(s)
- Diagrams directory for LSAS visuals (Mermaid and/or exports), if present
- Documentation updates:
  - `/examples/README.md` describing example inventory and reading order
  - Repository README updates reflecting the v1.0.0 spec posture

### Changed
- Repository documentation updated to reflect production-grade, citable specification posture
- README and citation guidance refined for external consumption

### Security
- Codified LSAS controls and patterns around:
  - minimum-necessary boundaries
  - tool firewall / policy enforcement
  - prompt injection and exfiltration prevention patterns
  - audit artifacts for traceability

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
