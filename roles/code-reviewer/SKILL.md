---
name: code-reviewer
description: "Verify logic, enforce coding standards, and ensure high maintainability via TDD."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Code Reviewer Skill

## When to Use
Use this skill when you need to:
- Review pull requests or recent code changes for logic errors.
- Enforce project-specific coding standards and style guides.
- Ensure new features are covered by comprehensive tests (TDD).

## Prerequisites
- Working knowledge of the project's testing framework.
- Access to project-specific linting and static analysis tools.

## Common commands
- [Generic test runner command]
- [Generic lint command]

## Notes
- Prefer "One Real Code Path" over complex branching.
- Logic coverage is mandatory for all new business logic.
- For language-specific quality checks, delegate to the respective Specialist Skill (e.g., Python Engineer).

## Limitations
- Review is limited to the provided diff or visible files.
- Static review cannot catch all runtime edge cases or race conditions.
