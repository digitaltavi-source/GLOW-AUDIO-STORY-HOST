# GLOW Audio Story Host

Runtime/integration boundary for GLOW Audio Story.

## Current state

`HOST_REPOSITORY_BOOTSTRAP_ONLY / NO_FACTORY_RUNTIME_BOUND / NO_PROVIDER_BOUND / NO_DEPLOYMENT_CLAIM`

This repository is intentionally empty of protected Factory internals at bootstrap.

## Repository branches

Exactly three persistent branches:

- `main` — accepted Host source authority after governed promotion.
- `sandbox` — only routine Host integration / security / runtime / deployment test surface.
- `backup` — predecessor preservation / recovery / forensic lineage.

`BRANCH ROLE != PRODUCT VERSION`.

## Security boundary

```text
HOST != FACTORY
HOST != CANON
HOST != CAPABILITY SYSTEM
HOST AVAILABILITY != FACTORY AUTHORITY
```

Do not commit:
- private Factory internals;
- protected corpus or raw private DNA sources;
- credentials / API keys / tokens;
- private evidence or consent/identity records;
- restricted Capability System implementation merely to simplify deployment.

Future runtime binding must use explicit contracts, exact component identities and fail-closed validation.

No provider, deployment target, MCP surface or live Factory assembly has been authorized by this bootstrap.

See `REPOSITORY_GOVERNANCE.md`.
