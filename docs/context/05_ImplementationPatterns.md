# 05 Implementation Patterns

Purpose: compact implementation playbook based on verified patterns from Vanilla, PD, Giga, and current PI.

## Pattern 1: Tech-gated decision family

Use when:
- A feature should unlock in stages and then expose decisions.

Verified examples:
- PI: tech_pi_advanced_planetary_mega_engineering gates many decision_pi_* entries.
- PD: tech_pd_domed_colonies gates moon base decisions.
- Giga: giga_tech_asteroid_manufactory gates asteroid industry construction.

## Pattern 2: Decision adds persistent deposit payload

Use when:
- Planet effects should remain as a durable transformation.

Verified examples:
- Vanilla: decision_strip_mining -> d_prospectorium_strip_mine.
- PI: decision_pi_* -> pi_d_*.

## Pattern 3: Deposit delegates repetitive job logic to inline scripts

Use when:
- Many deposits share similar job injection logic.

Verified examples:
- PI deposits call jobs/pi_* inline scripts.
- PD system hub uses jobs/pd_* inline scripts.
- Giga asteroid buildings use inline_script blocks for job swap and scaling.

## Pattern 4: Multi-scope propagation (moon/system/planet)

Use when:
- Effects originate in one scope but should impact related scopes.

Verified example:
- PD domed chain uses moon modifiers plus a system-level hub deposit to project benefits.

## Pattern 5: Long-form progression with situations (optional for PI)

Use when:
- Feature should evolve over time with monthly progress and events.

Verified vanilla example:
- divination_visitors, divination_locus.

PI status:
- No current PI situation file; adopting this is an optional evolution path, not a migration requirement.

## Open Questions / Follow-up Searches
