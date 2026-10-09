# GLOW Audio Story Host — Repository Governance

**Persistent branch count:** `3`

## Branch roles

### `main`
Accepted Host source authority after governed promotion. No routine experimentation.

### `sandbox`
Only routine integration/security/runtime/deployment test surface.

### `backup`
Predecessor preservation, recovery and forensic lineage. No routine development.

```text
PERSISTENT_BRANCH_COUNT = 3
main
backup
sandbox
```

No persistent `feature/*`, `candidate/*`, `repair/*`, `rnd/*`, `integration/*` or version branches without explicit governance exception.

## Promotion law

```text
SANDBOX CANDIDATE
-> EXACT IDENTITY FREEZE
-> BUILD / TEST
-> NORMAL / FAILURE / ADVERSARIAL / RECOVERY
-> SECURITY / CLAIM AUDIT
-> AUTHORIZED PROMOTION
-> PRESERVE PREDECESSOR
-> MAIN UPDATE
-> READ-BACK VERIFY
```

Material failure => `NO MAIN MUTATION`.

## Factory boundary

The Host exposes or transports only explicitly approved interfaces/results.

It may not own or silently redefine Factory semantics, Capability System semantics, Canon, qualification state or release authority.

`HOST CONTRACT != FACTORY CONTROL`.

## Secrets and private data

Secrets belong in deployment/runtime secret stores, never committed source.

Private Factory internals, proprietary intelligence, protected corpus/DNA, private evidence and consent/identity data are excluded unless a future explicit security design authorizes a bounded representation.

## Current claim ceiling

`HOST_REPOSITORY_BOOTSTRAP_ONLY`.

No runtime, provider, deployment, qualification, reproduction or field claim is established.
