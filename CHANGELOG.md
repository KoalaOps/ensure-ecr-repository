# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

No unreleased changes.

## [1.0.0] - 2025-01-27

### Added
- Initial release of ensure-ecr-repository action
- Idempotent ECR repository creation
- Comprehensive error handling for different AWS scenarios
- Action outputs for repository URI and existence status
- Support for all AWS regions
- Zero GitHub Actions UI errors with proper error handling

### Features
- ✅ Creates ECR repository if it doesn't exist
- ✅ Skips creation if repository already exists (idempotent)
- ✅ Handles AWS permission errors gracefully
- ✅ Provides repository URI as output for downstream steps
- ✅ Validates inputs and provides clear error messages
- ✅ Works with both access keys and OIDC authentication

### Requirements
- AWS credentials configured (via aws-actions/configure-aws-credentials or similar)
- Required AWS permissions: `ecr:DescribeRepositories`, `ecr:CreateRepository`

---

## Release Notes Template

When creating releases, use this template:

### [X.Y.Z] - YYYY-MM-DD

#### Added
- New features

#### Changed
- Changes in existing functionality

#### Deprecated
- Soon-to-be removed features

#### Removed
- Now removed features

#### Fixed
- Bug fixes

#### Security
- Vulnerability fixes 