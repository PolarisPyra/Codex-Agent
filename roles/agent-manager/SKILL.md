---
name: agent-manager
description: "Orchestrate specialized agents (employees) by matching tasks to their SKILL.md profiles."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Agent Manager Skill

## When to Use
Use this skill when you need to:
- Select the correct specialist (agent) for a specific task.
- Coordinate multi-agent workflows where different skills are needed in sequence.
- Manage the "Fleet" of available roles and understand their specific capabilities.

## Agent Fleet (The Employees)

| Agent ID | Role | Deployment Scenario |
|----------|------|---------------------|
| `project-manager` | Project Manager | Planning, TODO management, Triage, Milestones. |
| `security-engineer` | Security Engineer | Secret scanning, vulnerability audits, permission checks. |
| `code-reviewer` | Code Reviewer | TDD, logic verification, standards compliance. |
| `solutions-architect` | Solutions Architect | CONTEXT.md updates, ADRs, technical strategy. |
| `performance-engineer` | Performance Engineer | Profiling, bottlenecks, algorithmic optimization. |
| `product-designer` | Product Designer | Obsidian Void aesthetic, UI tokens, CSS/Tailwind. |
| `python-engineer` | Python Engineer | `uv`, `ruff`, `mypy`, `pytest`, idiomatic Python logic. |
| `javascript-engineer` | JavaScript Engineer | Frontend/Backend JS/TS, Web APIs, Vite/Next.js. |

## Dispatching Logic
1. **Analyze**: Determine the domain of the request (e.g., UI, Security, Backend).
2. **Select**: Match the domain to the `Agent ID` in the Fleet.
3. **Invoke**: Refer to the respective `SKILL.md` in `.codex/roles/[Agent-ID]/` for execution details.

## Notes
- `agent-manager` is the bridge between a raw user request and a specialized execution.
- Always check if a task requires multiple agents (e.g., `python-engineer` + `code-reviewer`).

## Limitations
- Do not perform the work of a specialist; only delegate and coordinate.
- If no agent matches the task, escalate to the Orchestrator for clarification.
