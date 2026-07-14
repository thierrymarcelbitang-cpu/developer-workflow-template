# WORKFLOW.md

# Development Workflow

This document defines the standard development workflow for all projects.

---

# Project Lifecycle

Idea

↓

Create GitHub Repository

↓

Initialize from developer-workflow-template

↓

Complete PROJECT.md

↓

Complete README.md

↓

Create GitHub Issue

↓

Create Feature Branch

↓

Implementation

↓

Validation

↓

Pull Request

↓

Human Review

↓

Merge

↓

Deployment

---

# Branch Workflow

Never work directly on main.

Always create a branch.

Examples:

feature/login

feature/dashboard

bugfix/navbar

hotfix/payment

---

# Development Process

## Step 1

Understand the task.

Read:

- README.md
- PROJECT.md
- AGENTS.md

Inspect the repository.

---

## Step 2

Create a short implementation plan.

---

## Step 3

Implement only the requested task.

Avoid unrelated modifications.

---

## Step 4

Run validation.

Examples:

npm run lint

npm test

npm run build

Only use commands supported by the repository.

---

## Step 5

Review changes.

Check:

- git diff
- changed files
- formatting
- tests

---

## Step 6

Open a Pull Request.

Do not merge without approval.

---

# AI Responsibilities

## Claude Code

Responsible for:

- implementation
- architecture
- refactoring
- documentation
- multi-file work

---

## OpenHands

Responsible for:

- repository analysis
- debugging
- dependency review
- architecture validation
- implementation verification

---

## Codex

Responsible for:

- code review
- focused fixes
- testing
- validation
- improvement suggestions

---

# Human Responsibilities

The project owner decides:

- priorities
- architecture approval
- security approval
- commits
- pushes
- merges
- production deployment

---

# Definition of Done

A task is complete only if:

- implementation finished
- validation passed
- documentation updated
- git diff reviewed
- no secrets exposed
- human approval received
