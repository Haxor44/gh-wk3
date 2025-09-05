# Emat - Go Backend Application

A simple Go backend application with automated build and linting using GitHub Actions and Super Linter.

## Development Setup

### Prerequisites
- Go 1.24.4 (or latest stable version)
- Git

### Installation
1. Clone the repository:
```bash
git clone https://github.com/Haxor44/gh-wk3
cd emat
```

2. Install dependencies:
```bash
go mod download
```

## Automated Quality Checks

This project uses GitHub Super Linter for code quality checks, which automatically runs on every commit via GitHub Actions.

The Super Linter performs:
- Go linting and static analysis
- Code quality checks
- Syntax validation

## GitHub Actions

The repository includes automated workflows:
1. **Build** - Compiles the application on push to main branch
2. **Lint** - Runs Super Linter analysis on every commit

Workflows are located in `.github/workflows/` and automatically execute on:
- Push events to any branch
- Pull requests to main branch

## Experiment

A deliberate linting error has been introduced in the codebase to demonstrate:
- How Super Linter detects violations across multiple languages
- How GitHub Actions workflow fails when linting errors exist
- The importance of maintaining code quality standards

Check the Actions tab in GitHub to see the failed workflow runs when the error is present.
