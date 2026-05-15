# Release Sequencing Policy

## Purpose

Define the mandatory sequencing and gate model for coordinated CommandLayer stack releases.

## Release Classes

1. **Protocol Governance Release**: policy-level changes affecting protocol semantics, interoperability constraints, or stack-wide release behavior.
2. **Implementation Coordination Release**: synchronized release event across runtime, SDK, agent, or integration repositories.
3. **Security Response Release**: out-of-band coordinated release triggered by a security event.

## Normative Release Sequence

For coordinated releases, repositories MUST be processed in this order unless a documented security override applies:
1. governance policy and decision artifacts,
2. protocol or interface-defining repositories,
3. runtime-core and runtime repositories,
4. agent-sdk and verification repositories,
5. MCP server and organization integration repositories.

## Gate Criteria

A release coordination record in `RELEASES/` MUST include:
- release scope statement,
- impacted repositories,
- compatibility matrix deltas,
- security impact assessment,
- required approvals and sign-off evidence,
- rollback or reversion procedure reference.

No coordinated release is considered complete until all required artifacts are recorded.

## Security Override

Security response releases MAY alter sequence to minimize exposure window, but MUST:
- record deviation reason,
- identify temporary compatibility impact,
- schedule post-incident normalization update.
