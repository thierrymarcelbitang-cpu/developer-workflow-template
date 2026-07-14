# RELEASE_PROCESS.md

# Release Process

This document defines how releases are versioned, documented, and published.

---

# Versioning

This project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (SemVer).

Format:

MAJOR.MINOR.PATCH

Rules:

- MAJOR: incompatible or breaking changes.
- MINOR: new functionality, backward compatible.
- PATCH: backward-compatible bug fixes.

Examples:

1.0.0 → 1.1.0 (new feature)

1.1.0 → 1.1.1 (bug fix)

1.1.1 → 2.0.0 (breaking change)

---

# Changelog

All notable changes must be recorded in `CHANGELOG.md` following [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

Rules:

- Add entries to the `[Unreleased]` section during development.
- Group entries under: Added, Changed, Deprecated, Removed, Fixed, Security.
- Move `[Unreleased]` entries under a new version heading when releasing.
- Never rewrite or delete published release entries.

---

# Release Steps

## Step 1

Confirm `main` is stable and all validation passes.

## Step 2

Review `CHANGELOG.md`.

Move relevant `[Unreleased]` entries under a new version section:

## [X.Y.Z] - YYYY-MM-DD

## Step 3

Update the version reference where applicable (for example `package.json`, if present).

## Step 4

Commit the release preparation using Conventional Commits format:

chore(release): prepare vX.Y.Z

See `docs/COMMIT_CONVENTIONS.md`.

## Step 5

Create an annotated Git tag:

git tag -a vX.Y.Z -m "vX.Y.Z"

## Step 6

Push the tag:

git push origin vX.Y.Z

## Step 7

Create a GitHub Release from the tag.

Use the corresponding `CHANGELOG.md` section as the release description.

---

# Hotfix Releases

Used for critical production fixes.

Process:

1. Branch from `main` using `hotfix/*`.
2. Implement the minimal fix.
3. Validate.
4. Merge into `main`.
5. Release a new PATCH version following the standard release steps.

See `docs/BRANCHING.md` for branch naming.

---

# Pre-releases

Optional pre-release identifiers may be used before a stable release:

1.0.0-alpha.1

1.0.0-beta.1

1.0.0-rc.1

Pre-releases are marked as such in the GitHub Release.

---

# AI Agent Rules

Claude Code

- prepares changelog updates
- updates documentation
- drafts release notes from the changelog

OpenHands

- validates release readiness
- inspects the repository before release

Codex

- reviews the diff before release
- verifies validation results

AI agents must not create tags, push tags, or publish GitHub Releases.

---

# Human Approval

Only the project owner:

- approves the version number
- creates and pushes release tags
- publishes the GitHub Release
- approves hotfix releases
