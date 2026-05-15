# Versioning Policy

## Scope

This policy defines versioning behavior for CommandLayer protocol and implementation repository classes.

## Versioning Model

1. Protocol-facing repositories MUST use semantic versioning semantics for declared external interfaces.
2. Non-protocol governance documents MAY use revision identifiers or dated records but MUST preserve traceability.
3. Repository-specific tag format MAY vary, but change class interpretation MUST remain consistent with this policy.

## Change Classification

- **Major**: incompatible interface or protocol behavior change.
- **Minor**: backward-compatible feature expansion.
- **Patch**: backward-compatible correction with no interface expansion.

## Cross-Repository Coordination Rules

1. If a protocol-level major change is accepted, dependent repositories MUST declare compatibility intent before coordinated release closure.
2. A minor or patch change in one repository MUST NOT claim stack-wide compatibility without matrix evidence.
3. Version claims in release records MUST reference compatibility entries in `COMPATIBILITY_MATRIX.md`.

## Prohibited Claims

- No repository MAY claim stack compatibility without explicit matrix registration.
- No governance document MAY assign concrete version numbers in advance of release records.
