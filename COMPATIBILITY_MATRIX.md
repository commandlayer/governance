# Compatibility Matrix Policy

## Purpose

Define the required structure and governance controls for compatibility declarations across CommandLayer repositories.

## Matrix Dimensions

Each compatibility record MUST include these dimensions:
1. protocol/interface baseline identifier,
2. runtime-core compatibility state,
3. runtime compatibility state,
4. agent-sdk compatibility state,
5. verifyagent compatibility state,
6. mcp-server compatibility state,
7. governance policy baseline reference,
8. effective date and release record reference.

## State Semantics

Allowed state values:
- `compatible`: validated for coordinated use,
- `conditionally-compatible`: compatible with documented constraints,
- `incompatible`: not validated or known to violate requirements.

## Evidence Requirements

Compatibility state changes MUST reference:
- verification evidence source,
- release coordination artifact,
- approving authority.

## Maintenance Rules

1. No repository may self-declare `compatible` without required evidence.
2. Conditional compatibility MUST include explicit operational constraints.
3. Matrix updates MUST be synchronized with relevant release records.
