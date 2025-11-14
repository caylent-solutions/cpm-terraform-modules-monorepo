# Changelog

All notable changes to CPM Terraform Modules Monorepo Packages will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-11-14

### Added
- **Shared Make Targets** - Standardized automation for Terraform module subdirectories
- **Testing Framework** - Terratest integration for comprehensive module testing
- **Terraform Automation** - Plan, format, lint, security scanning, and documentation generation
- **Go Automation** - Linting and formatting for Go test files
- **Cleanup Targets** - Remove Terraform state, cache files, and Go cache
- **All-in-One Validation** - Single command to run all validation and tests
- **CPM Integration** - Automatic inclusion via glob pattern in root Makefile

### Testing Targets
- `install` - Install Go dependencies and tools
- `test` - Run all Terratest tests
- `test-common` - Run common tests only
- `tf-test` - Run tests with test.config environment

### Terraform Targets
- `tf-plan` - Run terraform plan for examples
- `tf-format` - Check Terraform formatting
- `tf-format-fix` - Fix Terraform formatting
- `tf-lint` - Lint Terraform files with tflint
- `tf-security` - Run security checks with tfsec
- `tf-docs` - Generate Terraform documentation
- `tf-docs-check` - Verify documentation is up-to-date

### Go Targets
- `go-lint` - Lint Go test files
- `go-format` - Format Go test files

### Cleanup Targets
- `clean` - Remove Terraform state and cache files
- `clean-all` - Clean everything including Go cache

### Features
- Eliminates code duplication across all Terraform modules
- Consistent automation for all module subdirectories
- Ephemeral package management via CPM
- Automatic discovery and inclusion via glob patterns
- Module-level operations separate from monorepo-level tasks

### Documentation
- Comprehensive README with usage instructions
- Available Make targets reference
- Repository structure documentation
- Monorepo context and relationship explanation

[1.0.0]: https://github.com/caylent-solutions/cpm-terraform-modules-monorepo/releases/tag/1.0.0
