# CONTRIBUTING.md

## Purpose

This document explains how to contribute to projects created from this template.

## Before Starting

1. Read `README.md`.
2. Read `PROJECT.md`.
3. Read `AGENTS.md`.
4. Check existing issues and Pull Requests.
5. Confirm that the task is not already being handled.

## Branches

Never work directly on `main`.

Create a dedicated branch:

```bash
git switch -c feature/short-description 

```

Other examples:

```bash
git switch -c bugfix/login-error
git switch -c hotfix/security-patch
git switch -c chore/update-dependencies
```

See `docs/BRANCHING.md` for the complete branch strategy.

## Development

Keep changes focused.

Preserve the current architecture and style.

Do not modify unrelated files.

Add or update tests when appropriate.

Update documentation when behavior changes.

Never include secrets or machine-specific configuration.

## Validation

Run only commands supported by the repository.

Typical examples:

```bash
npm run lint
npm run typecheck
npm test
npm run build
```

or

```bash
ruff check .
pytest
mypy .
```

## Commits

Follow `docs/COMMIT_CONVENTIONS.md`.

Example:

```text
feat(auth): add password reset flow
```

Before committing:

```bash
git status
git diff
```

AI agents must not commit or push unless the project owner explicitly authorizes it.

## Pull Requests

Every Pull Request should include:

- a clear summary
- the reason for the change
- files or areas affected
- validation performed
- screenshots when relevant
- known limitations
- related issue number

## Review

A Pull Request should not be merged until:

- the change has been reviewed
- validation has passed
- no secret is included
- documentation is current
- the project owner approves the merge

## Code of Conduct

Be respectful, clear, constructive, and focused on improving the project.
