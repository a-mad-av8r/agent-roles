# agent-roles

Role-based steering for AI agent teams.

Agent roles are not personalities. They are operating boundaries: ownership,
exclusions, verification, and escalation. This repo gives those boundaries a
small file format and local checks.

## Quick Start

```bash
git clone https://github.com/a-mad-av8r/agent-roles
cd agent-roles
./scripts/role-list
./scripts/role-show designer
./scripts/role-check designer --path docs/posts/personal/cortex-series/cs004-role-based-steering.md --action edit
./scripts/role-check designer --path src/payments/service.py --action edit
```

The first check should pass. The second should fail because payment service code
is outside the designer role boundary.

## What Is Included

- Five example role profiles in `roles/`.
- `schemas/role-profile.schema.json` for a structured profile shape.
- `scripts/role-list`, `scripts/role-show`, `scripts/role-check`, and
  `scripts/role-diagnose`.
- Example Codex and Gemini adapter notes.
- Docs on boundaries and escalation.

## What Is Deliberately Out

- Platform-grade permission enforcement.
- Customer tenancy controls.
- Billing or deployment approval gates.
- Full impact-gate integration.

## Series Map

| Part | Repo | Focus |
| --- | --- | --- |
| 1 | [agent-cortex](https://github.com/a-mad-av8r/agent-cortex) | Operating memory core |
| 2 | [agent-telepathy](https://github.com/a-mad-av8r/agent-telepathy) | Event awareness |
| 3 | [agent-handoffs](https://github.com/a-mad-av8r/agent-handoffs) | Structured transfer |
| 4 | [agent-roles](https://github.com/a-mad-av8r/agent-roles) | Role boundaries |
| 5 | [agent-retention](https://github.com/a-mad-av8r/agent-retention) | Memory lifecycle |
| 6 | [agent-multimodel](https://github.com/a-mad-av8r/agent-multimodel) | Shared protocol across tools |

## Author

Amad Malik - Founder and CEO/CTO of Adaptech AI Ltd, building EnGenAI
([engenai.app](https://engenai.app)).

[LinkedIn](https://www.linkedin.com/in/amadmalik/) | [GitHub](https://github.com/a-mad-av8r)
