# Ledger Status

**Project:** `L_BLACKBIRD`  
**Tier:** TIER_6_SECURITY_EVAL  
**Identity:** Upstream `p1ngul1n0/Blackbird` @ `b45505080ef5` (GPL-3.0)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `p1ngul1n0/Blackbird` |
| Commit | `b45505080ef51bb3ef52dc29879ee6bef31e5b94` |
| Upstream licence | GPL-3.0 |
| Licence class | copyleft |
| Clone size | 2.27 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1500.0 IIU |
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
