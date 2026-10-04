# Ledger Status

**Project:** `L_OPTUNA`  
**Tier:** TIER_5_WORLD_NEURO_EMBODIED  
**Identity:** Upstream `optuna/optuna` @ `0684fbd74793` (MIT)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `optuna/optuna` |
| Commit | `0684fbd74793f71a01d713ba97bba8966be7a979` |
| Upstream licence | MIT |
| Licence class | permissive |
| Clone size | 3.95 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1000.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
