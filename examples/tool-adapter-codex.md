# Codex Adapter

Codex should read `AGENTS.md`, identify its active role, and run `role-check`
before touching shared code or policy-sensitive files.

```bash
./scripts/role-check backend-engineer --path src/api/projects.py --action edit
```
