# AGENTS Policy for CommandLayer Governance

## Purpose

This file defines mandatory execution behavior for Codex or any autonomous agent operating in this repository.

## Operating Rules

1. Treat this repository as policy infrastructure, not product code.
2. Use normative language (`MUST`, `MUST NOT`, `SHOULD`, `MAY`) for process definition.
3. Keep statements verifiable and repository-scoped.
4. Do not assert publication state, release state, or version state without explicit release record evidence in `RELEASES/`.
5. Do not introduce speculative implementation requirements that are not governance concerns.

## Change Control Rules

1. Governance policy changes that alter release gates, versioning semantics, compatibility interpretation, or security handling MUST be proposed through `RFC/`.
2. Structural changes to stack responsibility boundaries MUST update `STACK_MAP.md` and cross-reference a decision entry in `DECISION_LOG/`.
3. Security-policy edits MUST preserve coordinated disclosure requirements in `SECURITY.md`.
4. Compatibility policy edits MUST preserve matrix dimensions defined in `COMPATIBILITY_MATRIX.md`.

## Documentation Rules

1. No placeholders, no unresolved markers, and no implicit TODO instructions.
2. Each document MUST define scope, authority, and required update triggers.
3. Cross-repository instructions MUST identify responsible repository classes and verification artifacts.

## Scope

This file applies to `commandlayer/governance/` and all nested paths.
