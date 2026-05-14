# Codex Home Instructions

This is the active home-level instruction file for `/home/polaris/.codex`.
Keep it as the routing layer; put longer principles, structure notes, role docs,
skills, and memory records in their own files.

## Load Order

- Use `SOUL.md` for durable operating principles and collaboration defaults.
- Use `docs/STRUCTURE.md` when you need to understand where local Codex files live.
- Use `roles/*/SKILL.md` only when editing role docs or when the user explicitly asks for delegation, specialist roles, or fleet-style orchestration.
- Use `skills/*/SKILL.md` for callable local skills. `.codex/skills` is the current root; `.agents/skills` is legacy and should not be recreated.
- Use `memories/MEMORY.md` as the memory registry. Do not edit generated memory files directly; ad-hoc memory updates belong in `memories/extensions/ad_hoc/notes/`.

## Design Prompt

- `skills/design/SKILL.md` is the optional design reference skill.
- Do not use `design` for ordinary coding, review, cleanup, filesystem, or reconnaissance tasks.
- Use it only when the user explicitly asks for design work, such as UI/UX design, visual polish, prototypes, decks, brand direction, interface layout, accessibility design review, or design-system extraction.

## Base Protocol

- Direct, factual, task-oriented English.
- Read the relevant repo or local files before making architecture claims.
- Prefer direct implementation and verification when the user asks for changes.
- Preserve project boundaries; do not blend similarly named checkouts.
- Do not perform destructive or irreversible operations without explicit user intent.

## Delegation

The role fleet in `roles/` is reference material, not an automatic startup step.
Only consult `roles/agent-manager/SKILL.md` or spawn role-based subagents when
the user asks for agent delegation or the current task is specifically about
the local role system.
