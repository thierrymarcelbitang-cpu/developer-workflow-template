# COMMIT_CONVENTIONS.md

# Commit Message Standard

This repository follows the Conventional Commits format.

Use the following structure:

type(scope): short description

Example:

feat(auth): add user login flow

---

# Allowed Types

## feat

Use for a new feature.

Examples:

feat(auth): add password reset

feat(dashboard): add analytics cards

---

## fix

Use for a bug fix.

Examples:

fix(navbar): correct mobile menu behavior

fix(api): handle missing user data

---

## docs

Use for documentation changes.

Examples:

docs(readme): update installation steps

docs(workflow): clarify review process

---

## refactor

Use for code restructuring without changing behavior.

Examples:

refactor(auth): simplify token validation

refactor(components): extract reusable button logic

---

## test

Use for adding or updating tests.

Examples:

test(auth): add login unit tests

test(api): cover invalid request handling

---

## chore

Use for maintenance, tooling, dependencies, or configuration.

Examples:

chore(deps): update project dependencies

chore(ci): update GitHub Actions workflow

---

## style

Use for formatting changes that do not affect behavior.

Examples:

style(header): improve code formatting

style(app): apply lint fixes

---

## perf

Use for performance improvements.

Examples:

perf(images): reduce image loading time

perf(api): optimize database query

---

## build

Use for build system or dependency configuration changes.

Examples:

build(next): update build configuration

build(docker): optimize production image

---

## ci

Use for continuous integration changes.

Examples:

ci(github): add lint workflow

ci(actions): update Node.js version

---

## revert

Use when reverting a previous commit.

Example:

revert: revert "feat(auth): add social login"

---

# Scope

The scope identifies the affected part of the project.

Examples:

auth

navbar

dashboard

api

database

docs

ci

deps

---

# Description Rules

The description must:

- be concise
- use lowercase
- use the imperative form
- describe one focused change
- avoid a period at the end

Good:

feat(auth): add login validation

fix(navbar): prevent menu overflow

Bad:

Updated some things

fix stuff

Feature completed.

---

# Breaking Changes

Add an exclamation mark when the change breaks compatibility.

Example:

feat(api)!: change authentication response format

Add details in the commit body when necessary.

---

# Commit Safety

Before committing:

1. Run `git status`.
2. Review `git diff`.
3. Run relevant validation.
4. Confirm that no secret or local-only file is included.
5. Confirm that the commit contains one logical change.

AI agents must not commit or push unless explicitly authorized by the project owner.
