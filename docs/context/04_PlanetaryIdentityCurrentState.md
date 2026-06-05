# 04 PlanetaryIdentity Current State

Purpose: snapshot the current PI gameplay code state and immediate constraints.

## Active gameplay files (verified)

- PlanetaryIdentity/common/decisions/pi_decisions.txt
- PlanetaryIdentity/common/deposits/pi_deposits.txt
- PlanetaryIdentity/common/deposits/pi_blocker_deposits.txt
- PlanetaryIdentity/common/technology/pi_deposit_techs.txt
- PlanetaryIdentity/common/scripted_triggers/pi_screipted_triggers.txt
- PlanetaryIdentity/common/scripted_variables/pi_scripted_variables.txt

## Current namespace state (verified)

- Current active gameplay IDs are PI-style (pi_ prefix) in the main files above.
- This branch reflects substantial PME -> PI migration work already applied.
- Legacy PME context may still exist in historical docs/content, but active core gameplay script surface is PI-prefixed.

## Confirmed PI structure

Decision layer:
- decision_pi_* entries in pi_decisions.txt generally add one matching pi_d_* deposit.

Deposit layer:
- pi_d_* deposits hold most effect payloads (planet modifiers, inline job scripts, country modifiers).

Tech layer:
- tech_pi_* progression in pi_deposit_techs.txt
- cost/weight values sourced from pi_scripted_variables.txt (@pi_tech_cost_* and @pi_tech_weight_*)

Trigger layer:
- pi_is_gaia_planet
- pi_is_ecumenopolis
- pi_is_machine_planet
- pi_is_hive_planet

## Known quality notes (verified from file comments/names)

- In pi_deposits.txt, pi_d_mini_ecumenopolis includes an inline note: job_politician_add marked as not working correctly.
- Scripted trigger filename is spelled pi_screipted_triggers.txt (typo in filename, but valid as a path).
- No PI common/situations file currently found.

## Open Questions / Follow-up Searches
