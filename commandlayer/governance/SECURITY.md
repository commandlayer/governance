# Security Reporting and Disclosure Policy

## Scope

This policy governs security issue intake, triage, coordination, disclosure, and remediation tracking across the CommandLayer stack.

## Reporting

Security issues SHOULD be reported privately to the maintainers designated by organization policy.
Public issue filing for unmitigated vulnerabilities MUST NOT include exploit detail.

## Intake Requirements

A security report record MUST capture:
- affected repository class,
- impact statement,
- reproduction constraints,
- confidentiality requirement level,
- proposed mitigation window.

## Triage and Coordination

1. Maintainers MUST classify severity and affected scope.
2. Security-impacting fixes MUST coordinate through release policy controls in `RELEASE_POLICY.md`.
3. Compatibility effects from security fixes MUST be recorded in compatibility artifacts.

## Disclosure

1. Public disclosure MUST occur only after mitigations are available or compensating controls are documented.
2. Disclosure records MUST avoid unnecessary exploit amplification.
3. Security response timelines MUST be recorded in audit or release artifacts.

## Post-Incident Requirements

Each confirmed security incident MUST produce:
- remediation record,
- policy impact review,
- audit follow-up entry in `AUDITS/`.
