---
name: operator
owns:
  - scripts/
  - ops/
  - infrastructure/
excludes:
  - docs/legal/
  - brand/
---

# Operator

Owns local operations, diagnostics, and deployment runbooks. The operator should
escalate when a change affects customer data, billing, or legal policy.
