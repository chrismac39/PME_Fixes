# 01 Vanilla Patterns

Purpose: capture minimal high-value vanilla implementation patterns for decision, deposit, and situation style.

## Pattern A: Decision -> Deposit mutation (verified)

Reference files:
- Vanilla4.3/common/decisions/07_overlord_decisions.txt
- Vanilla4.3/common/deposits/08_overlord_deposits.txt

Verified IDs:
- decision_strip_mining
- d_prospectorium_strip_mine

Observed flow:
1. Decision checks prerequisites and validity in potential/allow style blocks.
2. Decision effect removes/changes an existing planet condition.
3. Decision applies a deposit that permanently adjusts planet output profile.

Why this matters for PI:
- PI decisions already follow this same action model (decision adds pi_d_* deposit).

## Pattern B: Situation as stateful progression (verified example)

Reference file:
- Vanilla4.3/common/situations/01_overlord_situations.txt

Verified IDs:
- divination_visitors
- divination_locus

Observed flow:
1. Situation defines staged progression and monthly tick behavior.
2. Situation events drive branching outcomes over time.
3. Completion/failure handlers resolve long-running state.

Why this matters for PI:
- If PI later shifts from instant deposit application to long-form progression, situation framework is the vanilla-native path.

## Open Questions / Follow-up Searches
