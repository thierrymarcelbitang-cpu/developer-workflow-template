# PROJECT_STRUCTURE.md

# Project Structure

This document describes the layout of the `developer-workflow-template` repository itself.

Projects created from this template should replace this file with a description of their own structure once the codebase exists.

---

# Root Files

## README.md

Project overview, features, tech stack, and getting started instructions.

## PROJECT.md

Project-specific goals, tech stack, architecture, and standards. Filled in per project.

## AGENTS.md

Rules and responsibilities for AI coding agents working in this repository.

## CLAUDE.md

Claude Code specific instructions and responsibilities.

## CONTRIBUTING.md

Contribution process: branching, validation, commits, and Pull Requests.

## CHANGELOG.md

Version history, following Keep a Changelog and Semantic Versioning. See `docs/RELEASE_PROCESS.md`.

## .gitignore

Files and folders excluded from version control.

---

# .github/

## .github/workflows/ci.yml

Continuous integration workflow.

## .github/ISSUE_TEMPLATE/

Templates for bug reports and feature requests.

## .github/pull_request_template.md

Default template applied to new Pull Requests.

---

# docs/

## docs/WORKFLOW.md

End-to-end development workflow, from idea to deployment.

## docs/BRANCHING.md

Branch strategy and naming rules.

## docs/COMMIT_CONVENTIONS.md

Conventional Commits standard used across the project.

## docs/RELEASE_PROCESS.md

Versioning and release steps.

## docs/PROJECT_STRUCTURE.md

This file.

---

# Adding Project Code

When a project is implemented from this template, application code is added alongside these files.

Typical additions (adapt to the actual stack; do not assume any of these apply):

src/ or app/

components/

lib/ or utils/

tests/

public/

Update `PROJECT.md` and this file to describe the real structure once it exists. Do not leave placeholder structure documentation once actual source code is added.

---

# AI Agent Rules

Claude Code

- keeps this file synchronized with the actual repository structure
- updates this file when top-level folders are added or removed

OpenHands

- verifies this file matches the real repository layout

Codex

- flags documentation drift during review

---

# Human Approval

Structural changes to the repository (new top-level folders, renamed core files) should be reviewed and approved by the project owner before merge.
