# CommandLayer Stack Responsibility Map

## Purpose

Define repository classes, boundaries, and coordination responsibilities for the CommandLayer stack.

## Repository Classes

1. **governance root (`commandlayer/governance`)**
   - Owns policy, process, sequencing, and coordination controls.
   - Does not host runtime implementation artifacts.

2. **commandlayer-clas**
   - Owns protocol/interface specifications and normative contract definitions.
   - Provides interface source of truth consumed by runtime and SDK repositories.

3. **runtime-core**
   - Owns foundational runtime primitives and execution contracts required by higher runtime layers.

4. **runtime**
   - Owns assembled runtime behavior and integration of runtime-core capabilities.

5. **agent-sdk**
   - Owns agent-facing SDK interfaces and integration surfaces for stack consumers.

6. **verifyagent**
   - Owns validation, conformance, and verification workflows used to confirm stack behavior.

7. **mcp-server**
   - Owns MCP-facing integration endpoints and protocol bridge behavior.

8. **commandlayer-org**
   - Owns organization-level coordination assets, policies, and operational controls that are not repository-local implementation code.

## Boundary Rules

- Protocol ownership MUST remain isolated from runtime implementation ownership.
- Runtime repositories MUST consume protocol definitions rather than redefining them.
- Verification repositories MUST assess conformance against declared protocol and compatibility policy.
- Governance repository MUST remain the authoritative source for cross-repository process rules.
