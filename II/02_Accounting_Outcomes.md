# Accounting Outcomes

**Project:** `L_BLACKBIRD`  
**Tier:** TIER_6_SECURITY_EVAL  
**Identity:** Upstream `p1ngul1n0/Blackbird` @ `b45505080ef5` (GPL-3.0)

## The eight outcomes

Every settled action is classified as exactly one of these. The set is
deliberately wider than pass/fail, because a system that reports only
'within budget' cannot distinguish good planning from a budget nobody
read.

| Outcome | Meaning | Compliant |
| --- | --- | --- |
| `ADHERED` | spent within the declared allocation | yes |
| `USED` | consumed granted-but-undeclared budget | yes |
| `TOUCHED` | budget read, ~zero consumption | yes |
| `IGNORED` | budget available, never consulted | **no** |
| `EFFICIENCY` | finished materially under allocation, as planned | yes |
| `OVERSPEND` | exceeded allocation without escalation | **no** |
| `UNDERSPEND` | far under allocation: possible underplanning | yes |
| `REFUSED` | declined to act; budget preserved | yes |

`UNDERSPEND` is not `EFFICIENCY`. Finishing well under a realistic
allocation is good planning; finishing far under one usually means the
estimate was wrong or the work was skipped. The two should not score
the same, so they are separate outcomes.

## This project's standing

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

Ledger blocks: **0**

Envelope `II-L_BLACKBIRD` caps spend at 1500.0 IIU, warning at
1200, escalating at
1425.

The cap is a policy allocation, not a measurement. Until an action
settles into the ledger there is no observed cost for this project,
and the standing is genuinely unknown rather than good.

