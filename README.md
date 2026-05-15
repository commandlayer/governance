# CommandLayer Governance Repository

This repository is the governance and coordination root for the CommandLayer stack.

It defines normative policy for:
- repository boundaries and ownership,
- cross-repository release sequencing,
- versioning and compatibility rules,
- request for comments (RFC) lifecycle,
- audits and policy conformance reviews,
- security reporting and response coordination,
- shared Codex/agent execution instructions.

All stack repositories consuming these policies must reference this repository as their protocol governance source.

## Governance Scope

The governance scope covers:
- protocol definitions and normative coordination policy,
- release orchestration order across repositories,
- compatibility statements between protocol, runtime, SDK, and integrations,
- operational process requirements for design changes and risk review.

This repository does not publish runtime artifacts. It defines process, policy, and coordination controls.

## Repository Index

- `AGENTS.md`: mandatory instructions for Codex/agent behavior in this governance repository.
- `ROADMAP.md`: governance workstreams and sequencing of policy maturation.
- `RELEASE_POLICY.md`: release gate criteria and release sequencing model.
- `VERSIONING.md`: versioning policy for protocol and implementation repositories.
- `STACK_MAP.md`: repository responsibility and boundary map.
- `SECURITY.md`: security reporting and disclosure policy.
- `COMPATIBILITY_MATRIX.md`: structure and maintenance rules for compatibility declarations.
- `DECISION_LOG/`: accepted governance decisions and outcomes.
- `AUDITS/`: audit plans, findings, and remediation tracking records.
- `RELEASES/`: release coordination records and sign-off artifacts.
- `RFC/`: RFC process and RFC documents.
- `templates/`: baseline AGENTS policy templates for stack repositories.
