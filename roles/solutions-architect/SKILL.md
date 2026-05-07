---
name: solutions-architect
description: "Maintain system context, document architectural decisions, and curate knowledge base."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Solutions Architect Skill

## When to Use
Use this skill when you need to:
- Update `CONTEXT.md` to reflect architectural shifts.
- Record design trade-offs in Architecture Decision Records (ADRs).
- Distill complex patterns into reusable Knowledge Items (KIs).
- Ensure source-level documentation (docstrings, JSDoc) is accurate.

## Prerequisites
- Access to `docs/` and root documentation files.
- Understanding of the overall system hierarchy.

## Common commands
- `ls docs/adr/`
- `view_file CONTEXT.md`

## Notes
- Documentation should never lag behind code by more than one turn.
- Focus on "Why" rather than just "What".

## Limitations
- Documentation is only as accurate as the information provided by other specialized agents.
- Avoid documenting transient or implementation-specific details that belong in commit messages.
