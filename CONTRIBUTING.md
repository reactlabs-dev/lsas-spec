# Contributing to LSAS Specification

Thank you for your interest in contributing to the LSAS (Layered Safety and Accuracy System) Specification! This document provides guidelines for contributing to this project.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Process](#development-process)
- [Style Guidelines](#style-guidelines)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)

## Code of Conduct

This project adheres to a Code of Conduct that all contributors are expected to follow. Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) before contributing.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title and description**
- **Steps to reproduce** the issue
- **Expected behavior** vs. actual behavior
- **Version information** (specification version, schema version)
- **Additional context** (screenshots, error messages, etc.)

Use the bug report template when creating issues.

### Suggesting Enhancements

Enhancement suggestions are welcome! When suggesting enhancements:

- **Use a clear title** describing the enhancement
- **Provide a detailed description** of the proposed functionality
- **Explain why this enhancement would be useful** to most users
- **List any alternatives** you've considered

Use the feature request template when creating issues.

### Contributing to Schemas

Schema contributions should:

- Follow JSON Schema specification standards
- Include comprehensive documentation
- Provide example use cases
- Be validated against test data
- Maintain backward compatibility when possible

### Contributing to Documentation

Documentation improvements are always welcome:

- Fix typos and grammatical errors
- Improve clarity and readability
- Add examples and use cases
- Update outdated information
- Expand on technical details

## Development Process

1. **Fork the repository** to your GitHub account
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/lsas-spec.git
   cd lsas-spec
   ```
3. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. **Make your changes** following the style guidelines
5. **Test your changes** thoroughly
6. **Commit your changes** following commit guidelines
7. **Push to your fork**:
   ```bash
   git push origin feature/your-feature-name
   ```
8. **Create a Pull Request** from your fork to the main repository

## Style Guidelines

### JSON Schema Guidelines

- Use consistent indentation (2 spaces)
- Include `$schema` and `$id` fields
- Provide `title` and `description` for all schemas
- Use descriptive property names
- Include examples in schema documentation
- Validate all schemas before committing

Example schema structure:
```json
{
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "$id": "https://github.com/reactlabs-dev/lsas-spec/schemas/example.schema.json",
  "title": "Example Schema",
  "description": "A detailed description of what this schema represents",
  "type": "object",
  "properties": {
    "propertyName": {
      "type": "string",
      "description": "Description of this property"
    }
  },
  "required": ["propertyName"]
}
```

### Documentation Guidelines

- Use clear, concise language
- Follow Markdown best practices
- Include code examples where appropriate
- Use proper heading hierarchy
- Add links to related sections
- Keep line length reasonable (80-100 characters when possible)

### File Naming Conventions

- Schema files: `lowercase-with-hyphens.schema.json`
- Example files: `lowercase-with-hyphens.example.json`
- Documentation: `UPPERCASE.md` for root-level docs, `lowercase-with-hyphens.md` for others

## Commit Guidelines

Follow these commit message conventions:

### Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Formatting changes (no code changes)
- **refactor**: Code refactoring
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```
feat(schemas): add validation schema for safety layers

Add new JSON schema for validating safety layer configurations
including audit trails and compliance checkpoints.

Closes #123
```

```
docs(readme): update Zenodo integration instructions

Clarify the steps for setting up Zenodo integration and
provide troubleshooting tips for common issues.
```

## Pull Request Process

1. **Update documentation** to reflect any changes
2. **Add or update tests** if applicable
3. **Ensure all tests pass** and schemas validate
4. **Update CHANGELOG.md** with your changes
5. **Reference related issues** in the PR description
6. **Request review** from maintainers
7. **Address review feedback** promptly
8. **Squash commits** if requested before merging

### Pull Request Template

When creating a PR, include:

- **Description**: What changes does this PR introduce?
- **Motivation**: Why is this change needed?
- **Related Issues**: Link to related issues
- **Testing**: How was this tested?
- **Checklist**: Complete the PR checklist
- **Breaking Changes**: Note any breaking changes

### Review Process

- All PRs require at least one approval from a maintainer
- Address all review comments or explain why changes aren't needed
- Keep PRs focused on a single concern
- Be responsive to feedback
- Be patient - reviews may take time depending on maintainer availability

## Questions?

If you have questions about contributing, please:

1. Check existing documentation
2. Search for related issues
3. Create a new issue with the "question" label
4. Reach out to maintainers via GitHub Discussions

Thank you for contributing to LSAS! Your efforts help improve AI safety in healthcare and regulated environments.
