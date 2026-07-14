# PROJECT.md

# Project Overview

Describe the project here.

Example:

This repository contains the source code for a web application.
The objective is to build a maintainable, production-ready application using modern development practices.

---

# Goals

Primary goals:

- Maintain clean architecture.
- Keep the codebase easy to understand.
- Minimize technical debt.
- Prefer maintainability over clever code.
- Keep commits small and focused.

---

# Tech Stack

Replace these values for each project.

Frontend:

- React
- Next.js
- TypeScript

Backend:

- Node.js

Styling:

- Tailwind CSS

Database:

- PostgreSQL

Package manager:

- npm

Deployment:

- Vercel

---

# Repository Structure

Describe the important folders.

Example:

app/
components/
lib/
hooks/
public/
styles/

---

# Development Workflow

Preferred workflow:

1. Understand the task.
2. Inspect the repository.
3. Create a plan.
4. Implement only the requested changes.
5. Validate.
6. Review the diff.
7. Wait for approval before committing.

---

# Coding Standards

General rules:

- Prefer readability.
- Prefer explicit code.
- Avoid unnecessary abstraction.
- Avoid duplicated logic.
- Keep functions small.
- Use descriptive names.
- Preserve the existing style.

---

# Testing Strategy

Run only the tests supported by the repository.

Examples:

npm run lint

npm run build

npm test

Do not invent commands.

---

# Git Workflow

Branch strategy:

main
develop
feature/*
bugfix/*
hotfix/*

Never commit directly to production branches without approval.

---

# Security

Never expose:

- API keys
- passwords
- secrets
- tokens
- certificates
- private configuration

Never commit:

.env
.env.local
credentials
private keys

---

# Deployment

Document the deployment platform here.

Examples:

- Vercel
- AWS
- Docker
- Railway

---

# AI Agent Instructions

All coding agents must:

- read AGENTS.md first
- inspect the repository
- avoid unnecessary modifications
- preserve project architecture
- avoid destructive Git commands
- never commit without approval
- provide a completion report
