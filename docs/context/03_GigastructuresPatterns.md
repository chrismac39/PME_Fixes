# 03 Gigastructures Patterns

Purpose: document the giga asteroid-industry and orbital-arcology references used for PI planning.

## Core Giga files (verified)

- Gigastructures/common/technology/giga_02_society.txt
- Gigastructures/common/technology/giga_03_engineering.txt
- Gigastructures/common/decisions/giga_decisions.txt
- Gigastructures/common/megastructures/zz_c_asteroid_manufactory.txt
- Gigastructures/common/inline_scripts/megastructures/asteroid_industry/asteroid_industry_construction.txt
- Gigastructures/common/buildings/giga_asteroid_industry_buildings.txt
- Gigastructures/common/static_modifiers/giga_asteroid_industry_modifiers.txt

## Key IDs and hooks (verified)

Tech and decision gates:
- giga_tech_asteroid_manufactory
- giga_tech_orbital_arcologies
- decision_giga_build_orbital_arcology

Asteroid-manufactory megastructure IDs:
- asteroid_manufactory_0
- asteroid_manufactory_alloys
- asteroid_manufactory_consumer_goods
- asteroid_manufactory_energy
- asteroid_manufactory_food
- asteroid_manufactory_supertensiles

Building links:
- building_giga_asteroid_factory_alloys
- building_giga_asteroid_factory_consumer_goods
- building_giga_asteroid_factory_energy

Candidate modifiers:
- giga_asteroid_industry_candidate_alloys
- giga_asteroid_industry_candidate_marked

## Architectural pattern

1. Tech unlock gates construction eligibility.
2. Inline script centralizes placement rules, caps, and queue/cancel lifecycle.
3. Megastructure variants map to specialized downstream building modifiers.
4. Planet candidate modifiers mark valid targets and can be removed on completion.

## Reusable lessons for PI

- Split large features into: tech gate, placement/eligibility script, and effect payload.
- Keep cap logic in one script path rather than duplicating checks in every definition.
- Use candidate markers when target validation is non-trivial.

## Open Questions / Follow-up Searches
