# LSAS Specification

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)

**LSAS (Layered Safety and Accuracy System)** — Technical specification and whitepaper for governed Generative AI outputs in regulated healthcare and medtech environments.

## Overview

This repository contains the formal specification, schemas, examples, and technical whitepaper for LSAS, a framework designed to ensure safety, accuracy, and compliance for AI-generated content in regulated industries.

## Repository Structure

```
lsas-spec/
├── paper/          # Technical whitepaper and related documents
├── schemas/        # JSON schemas and specification files
├── examples/       # Example implementations and use cases
├── CITATION.cff    # Citation metadata for academic use
├── CHANGELOG.md    # Version history and release notes
├── CONTRIBUTING.md # Contribution guidelines
├── CODE_OF_CONDUCT.md # Community code of conduct
└── LICENSE         # Apache 2.0 License
```

## Getting Started

### For Implementers

1. Review the technical specification in the `/paper` directory
2. Examine the schemas in `/schemas` to understand data structures
3. Check `/examples` for reference implementations
4. Follow the implementation guidelines in the specification

### For Contributors

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## Versioning

We use [Semantic Versioning](https://semver.org/) for this specification. For available versions, see the [releases page](https://github.com/reactlabs-dev/lsas-spec/releases).

## Citation

If you use this specification in your research or implementation, please cite it using the metadata in [CITATION.cff](CITATION.cff).

## Minting a DOI via Zenodo

This repository is configured to automatically generate a DOI (Digital Object Identifier) for each release via Zenodo:

### Setup (One-time)

1. Go to [Zenodo GitHub integration](https://zenodo.org/account/settings/github/)
2. Log in with your GitHub account
3. Find `reactlabs-dev/lsas-spec` in the repository list
4. Toggle the switch to enable Zenodo integration

### Creating a Release with DOI

1. Ensure all changes are committed and the repository is ready for release
2. Update `CHANGELOG.md` with release notes
3. Update version numbers in `CITATION.cff` and any schema files
4. Create a new release on GitHub:
   - Go to the [releases page](https://github.com/reactlabs-dev/lsas-spec/releases)
   - Click "Draft a new release"
   - Create a new tag (e.g., `v1.0.0`)
   - Add release title and description
   - Publish the release
5. Zenodo will automatically:
   - Detect the new release
   - Archive the repository snapshot
   - Generate a unique DOI
   - Create a DOI badge
6. Update the DOI badge in this README with the newly generated DOI

### After DOI Generation

1. Copy the DOI from Zenodo
2. Update the badge at the top of this README
3. Update `CITATION.cff` with the DOI
4. Commit these changes to the `main` branch

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Contact

For questions, issues, or contributions, please use the GitHub issue tracker or refer to [CONTRIBUTING.md](CONTRIBUTING.md).

## Acknowledgments

LSAS was developed to address the critical need for governed AI systems in regulated healthcare and medtech environments.
