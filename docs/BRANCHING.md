# BRANCHING.md

# Branch Strategy

This repository follows a simple, feature-based branching strategy.

---

# Permanent Branches

## main

Purpose:

- Production-ready code
- Stable releases only

Rules:

- Never develop directly on main.
- Never force push.
- Merge only after review and validation.

---

# Working Branches

## feature/*

Used for:

- new features
- enhancements
- improvements

Examples:

feature/login

feature/dashboard

feature/payment

---

## bugfix/*

Used for:

- bug corrections
- unexpected behavior
- regression fixes

Examples:

bugfix/navbar

bugfix/auth

bugfix/footer

---

## hotfix/*

Used for:

- production emergencies
- security fixes
- critical outages

Examples:

hotfix/payment

hotfix/security

---

## chore/*

Used for:

- dependency updates
- tooling
- maintenance
- configuration

Examples:

chore/eslint

chore/github-actions

chore/dependencies

---

# Branch Lifecycle

Issue

↓

Create Branch

↓

Implementation

↓

Validation

↓

Pull Request

↓

Review

↓

Merge into main

↓

Delete merged branch

---

# Naming Rules

Use lowercase.

Use hyphens.

Good:

feature/user-profile

feature/admin-dashboard

bugfix/login-error

Bad:

Feature1

MyBranch

FixStuff

---

# AI Agent Rules

Claude Code

- implements features
- refactors
- updates documentation

OpenHands

- validates architecture
- inspects repository
- verifies implementation

Codex

- reviews code
- suggests improvements
- validates quality

---

# Human Approval

Only the project owner decides when a branch is merged into main.
