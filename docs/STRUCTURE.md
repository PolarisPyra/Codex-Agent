# Codex Home Structure

This document maps the durable files under `/home/polaris/.codex`.

## Instruction Surfaces

- `AGENTS.md`: active home-level routing instructions. Keep it short and focused on load order, boundaries, and when to use other files.
- `SOUL.md`: stable collaboration principles and safety defaults.
- `roles/*/SKILL.md`: local role descriptions for specialist/fleet workflows. These are reference docs unless the user explicitly asks for role delegation or role-doc edits.

## Skills

- `skills/*/SKILL.md`: callable local user/community skills.
- `skills/.skill-lock.json`: install metadata for migrated user/community skills.
- `skills/.system/`: system-provided skills. Treat this as generated and do not edit or track it as user policy.

The old `~/.agents/skills` root has been folded into `~/.codex/skills`.
Do not recreate `.agents` for normal skill work.

## Memory

- `memories/MEMORY.md`: generated searchable memory registry.
- `memories/memory_summary.md`: generated compact summary used for fast context.
- `memories/rollout_summaries/`: append-only summaries of prior rollouts.
- `memories/extensions/ad_hoc/notes/`: the only place to add explicit memory-update notes by hand.

Do not manually edit generated memory registry files. Add a new note under
`memories/extensions/ad_hoc/notes/` only when the user explicitly asks to update memory.

## Design Prompt

- `design-system-prompt/codex/system-prompt.md`: optional design reference.
- Load it only for explicit design/UI/UX/prototype/visual-polish tasks.
- Do not load it for ordinary coding, review, cleanup, filesystem, or reconnaissance work.

## Runtime And Generated Data

- `sessions/`, `archived_sessions/`, `shell_snapshots/`, `log`, `cache`, sqlite files, auth files, and global state JSON files are runtime/tool state.
- `vendor_imports/` and `.tmp/` are cached or imported tool data.
- `rules/` is intentionally ignored by Git here.
