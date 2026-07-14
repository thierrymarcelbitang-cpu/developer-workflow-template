# AGENTS.md

## Purpose

This repository uses AI coding agents as assistants. Agents must work carefully, preserve project stability, and follow the rules below.

## General Rules

1. Read `PROJECT.md` before making decisions.
2. Inspect the repository before modifying files.
3. Do not assume the framework, package manager, architecture, or deployment platform.
4. Make the smallest change necessary to complete the task.
5. Do not modify unrelated files.
6. Do not delete files unless the task explicitly requires it.
7. Do not expose, print, commit, or copy secrets.
8. Never commit `.env`, credentials, API keys, tokens, certificates, or private configuration files.
9. Preserve the existing coding style and project structure.
10. Explain important assumptions clearly.
11. Run relevant checks after modifications.
12. Report commands executed, files changed, checks performed, and remaining risks.

## Before Editing

1. Run `pwd`.
2. Run `git status`.
3. Identify the current branch.
4. Inspect the relevant files.
5. Confirm that the requested change is within scope.
6. Create a short plan for work involving multiple files.

## Validation

Use only commands supported by the repository.

JavaScript or TypeScript examples:

- `npm run lint`
- `npm run typecheck`
- `npm test`
- `npm run build`

Python examples:

- `ruff check .`
- `pytest`
- `mypy .`

Do not invent scripts that are not defined in the project.

## Git Safety

1. Do not work directly on `main` unless explicitly authorized.
2. Do not run destructive Git commands without explicit permission.
3. Do not use `git reset --hard`, `git clean -fd`, force push, or history rewriting unless explicitly requested.
4. Do not commit or push unless explicitly requested.
5. Review `git diff` before reporting completion.

## Agent Coordination

Only one coding agent should modify a branch at a time.

Recommended roles:

- Claude Code: implementation, architecture, refactoring, and multi-file work.
- OpenHands: repository analysis, audits, debugging, and controlled implementation.
- Codex: code review, testing, focused fixes, and implementation support.
- Human owner: approves architecture, security-sensitive changes, commits, pushes, merges, and deployment.

## Completion Report

At the end of a task, report:

- Summary
- Files changed
- Commands run
- Validation results
- Known limitations
- Recommended next step
