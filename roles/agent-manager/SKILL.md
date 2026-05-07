---
name: agent-manager
description: "Manage multiple local CLI agents via tmux sessions (start/stop/monitor/assign) with cron-friendly scheduling."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Agent Manager Skill

## When to Use
Use this skill when you need to:
- Run multiple local CLI agents in parallel (separate tmux sessions).
- Start/stop agents and tail their logs.
- Assign tasks to agents and monitor output.
- Schedule recurring agent work (cron).

## Prerequisites
- Install `agent-manager-skill` in your workspace.
- Requires `tmux` and `python3`.

## Common commands
- `python3 agent-manager/scripts/main.py doctor`
- `python3 agent-manager/scripts/main.py list`
- `python3 agent-manager/scripts/main.py start [AGENT_ID]`
- `python3 agent-manager/scripts/main.py monitor [AGENT_ID] --follow`
- `python3 agent-manager/scripts/main.py assign [AGENT_ID] <<'EOF' ... EOF`

## Notes
- Agents are configured under an `agents/` directory.

## Limitations
- Use this skill only when the task clearly matches the scope described above.
- Do not treat the output as a substitute for environment-specific validation, testing, or expert review.
- Stop and ask for clarification if required inputs, permissions, safety boundaries, or success criteria are missing.
