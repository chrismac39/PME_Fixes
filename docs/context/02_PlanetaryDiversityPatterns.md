# 02 Planetary Diversity Patterns

Purpose: extract the PD domed-colony chain used as a reference architecture.

## Core PD files (verified)

- Planetary Diversity/common/technology/pd_technology.txt
- Planetary Diversity/common/decisions/pd_domed_base_decisions.txt
- Planetary Diversity/common/deposits/pd_domed_habitat_deposits.txt
- Planetary Diversity/common/deposits/pd_domed_colony_deposits.txt
- Planetary Diversity/common/static_modifiers/pd_domed_colonies_modifiers.txt
- Planetary Diversity/events/pd_dome_bases_events.txt

## Key IDs and hooks (verified)

Technology gate:
- tech_pd_domed_colonies

Decision/event chain:
- decision_build_pd_moon_base
- decision_build_pd_moon_base_moon_colony
- pddomebases.50
- pddomebases.100
- pd_create_outpost_visual_effect

System hub deposit:
- d_pd_solar_system_network_hub

Moon/outpost modifiers:
- pd_moon_base_trade
- pd_moon_base_military
- pd_moon_base_factory
- pd_moon_base_foundry
- pd_moon_base_admin
- pd_moon_base_priest

## Architectural pattern

1. A tech unlock enables the decision family.
2. Decisions add a system-level deposit anchor (network hub).
3. Event IDs assign one of several moon-base specializations.
4. Triggered modifiers and inline job scripts read moon modifiers and project effects to planets in system scope.

## Reusable lessons for PI

- PD shows strong multi-scope design: moon modifiers -> system hub deposit -> planet effects.
- The event-driven assignment step avoids hardcoding one static result per decision.
- Inline job scripts keep repetitive job math centralized.

## Open Questions / Follow-up Searches
