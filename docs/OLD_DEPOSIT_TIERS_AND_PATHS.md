# Deposit Tiers and Unlock Paths

This file visualizes how PI deposits are reached through technology and planetary decisions.

## Core Progression Path

```mermaid
flowchart TD
    A[tech_pi_rudimentary_planetary_mega_engineering]

    A --> B[tech_pi_intermediate_economic_planetary_mega_engineering]
    A --> C[tech_pi_intermediate_governmental_planetary_mega_engineering]
    A --> D[tech_pi_intermediate_industrial_planetary_mega_engineering]
    A --> E[tech_pi_intermediate_defensive_planetary_mega_engineering]

    C --> F[tech_pi_advanced_planetary_mega_engineering]

    F --> G[tech_pi_specialized_planetary_mega_engineering]
    F --> H[tech_pi_ascendant_planetary_mega_engineering]

    A --> A1[Rudimentary deposits via decisions\n15 total]
    B --> B1[Economic intermediate deposits\n4 total]
    C --> C1[Governmental intermediate deposits\n6 total]
    D --> D1[Industrial intermediate deposits\n7 total]
    E --> E1[Defensive intermediate deposits\n3 total]
    F --> F1[Advanced deposits\n18 total]
    G --> G1[Specialized deposits\n2 total]
    H --> H1[Ascendant deposits\n5 total]
```

## Path Type

```mermaid
flowchart LR
    T[Tech prerequisite met] --> U[Planet meets decision potential/allow checks]
    U --> V[Player or AI enacts decision]
    V --> W[add_deposit effect runs]
```

## Full Tier Catalog (Every Decision Path)

### Rudimentary
Prerequisite: `tech_pi_rudimentary_planetary_mega_engineering` (15 total)

### Base Variant
- `decision_pi_worldwide_maglev` -> `pi_d_worldwide_maglev`
- `decision_pi_polar_resource_silos` -> `pi_d_polar_resource_silos`
- `decision_pi_mining_construction` -> `pi_d_mining_construction`
- `decision_pi_planetary_irrigation_water` -> `pi_d_planetary_irrigation_water`
- `decision_pi_planetary_fusion_grid` -> `pi_d_planetary_fusion_grid`

##### Machine Variant
- `decision_pi_machine_worldwide_maglev` -> `pi_d_machine_worldwide_maglev`
- `decision_pi_machine_polar_resource_silos` -> `pi_d_machine_polar_resource_silos`
- `decision_pi_machine_system_extraction` -> `pi_d_machine_system_extraction`
- `decision_pi_machine_planetary_water_processing` -> `pi_d_machine_planetary_water_processing`
- `decision_pi_machine_planetary_fusion_grid` -> `pi_d_machine_planetary_fusion_grid`

##### Hive Variant
- `decision_pi_hive_worldwide_maglev` -> `pi_d_hive_worldwide_maglev`
- `decision_pi_hive_polar_resource_silos` -> `pi_d_hive_polar_resource_silos`
- `decision_pi_hive_mineral_extraction_warrens` -> `pi_d_hive_mineral_extraction_warrens`
- `decision_pi_hive_nutrient_processing_megaplant` -> `pi_d_hive_nutrient_processing_megaplant`
- `decision_pi_hive_planetary_fusion_grid` -> `pi_d_hive_planetary_fusion_grid`

### Intermediate Economic
Prerequisite: `tech_pi_intermediate_economic_planetary_mega_engineering` (4 total)

### Base Variant
- `decision_pi_space_elevator` -> `pi_d_space_elevator`
- `decision_pi_corporate_megacampus` -> `pi_d_corporate_megacampus`

##### Machine Variant
- `decision_pi_machine_space_elevator` -> `pi_d_machine_space_elevator`

##### Hive Variant
- `decision_pi_hive_space_elevator` -> `pi_d_hive_space_elevator`

## Intermediate Governmental
Prerequisite: `tech_pi_intermediate_governmental_planetary_mega_engineering` (6 total)

### Base Variant
- `decision_pi_supermax_prison_rehab` -> `pi_d_supermax_prison_rehab`
- `decision_pi_interstellar_hospital` -> `pi_d_interstellar_hospital`

##### Machine Variant
- `decision_pi_machine_drone_reprogramming_center` -> `pi_d_machine_drone_reprogramming_center`
- `decision_pi_machine_auxiliary_assembly_centers` -> `pi_d_machine_auxiliary_assembly_centers`

##### Hive Variant
- `decision_pi_hive_neural_regulation_nexus` -> `pi_d_hive_neural_regulation_nexus`
- `decision_pi_hive_supplemental_breeding_pools` -> `pi_d_hive_supplemental_breeding_pools`

## Intermediate Industrial
Prerequisite: `tech_pi_intermediate_industrial_planetary_mega_engineering` (7 total)

### Base Variant
- `decision_pi_subsurface_megaforges` -> `pi_d_subsurface_megaforges`
- `decision_pi_orbital_superfactory` -> `pi_d_orbital_superfactory`
- `decision_pi_chemical_hazardous_goods` -> `pi_d_chemical_hazardous_goods`

##### Machine Variant
- `decision_pi_machine_subsurface_megaforges` -> `pi_d_machine_subsurface_megaforges`
- `decision_pi_machine_chemical_hazardous_goods` -> `pi_d_machine_chemical_hazardous_goods`

##### Hive Variant
- `decision_pi_hive_subsurface_megaforges` -> `pi_d_hive_subsurface_megaforges`
- `decision_pi_hive_chemical_hazardous_goods` -> `pi_d_hive_chemical_hazardous_goods`

## Intermediate Defensive
Prerequisite: `tech_pi_intermediate_defensive_planetary_mega_engineering` (3 total)

### Base Variant
- `decision_pi_orbital_defense_grid` -> `pi_d_orbital_defense_grid`

##### Machine Variant
- `decision_pi_machine_orbital_defense_grid` -> `pi_d_machine_orbital_defense_grid`

##### Hive Variant
- `decision_pi_hive_orbital_defense_grid` -> `pi_d_hive_orbital_defense_grid`

## Advanced
Prerequisite: `tech_pi_advanced_planetary_mega_engineering` (18 total)

### Base Variant
- `decision_pi_mini_ecumenopolis` -> `pi_d_mini_ecumenopolis`
- `decision_pi_orbital_colonies` -> `pi_d_orbital_colonies`
- `decision_pi_fleet_academy` -> `pi_d_fleet_academy`
- `decision_pi_university_cityscape` -> `pi_d_university_cityscape`
- `decision_pi_resort_archipelago` -> `pi_d_resort_archipelago`
- `decision_pi_deep_mantle_exotic_hyperforge` -> `pi_d_deep_mantle_exotic_hyperforge`

##### Machine Variant
- `decision_pi_machine_global_management_nexus` -> `pi_d_machine_global_management_nexus`
- `decision_pi_machine_orbital_colonies` -> `pi_d_machine_orbital_colonies`
- `decision_pi_machine_fleet_coordination_systems` -> `pi_d_machine_fleet_coordination_systems`
- `decision_pi_machine_continental_computing_system` -> `pi_d_machine_continental_computing_system`
- `decision_pi_machine_planetwide_software_standardization_network` -> `pi_d_machine_planetwide_software_standardization_network`
- `decision_pi_machine_deep_mantle_exotic_hyperforge` -> `pi_d_machine_deep_mantle_exotic_hyperforge`

##### Hive Variant
- `decision_pi_hive_planetary_coordination_nodes` -> `pi_d_hive_planetary_coordination_nodes`
- `decision_pi_hive_orbital_colonies` -> `pi_d_hive_orbital_colonies`
- `decision_pi_hive_fleet_coordination_nexus` -> `pi_d_hive_fleet_coordination_nexus`
- `decision_pi_hive_collective_computing_consciousness` -> `pi_d_hive_collective_computing_consciousness`
- `decision_pi_hive_consciousness_synchronization_lattice` -> `pi_d_hive_consciousness_synchronization_lattice`
- `decision_pi_hive_deep_mantle_exotic_hyperforge` -> `pi_d_hive_deep_mantle_exotic_hyperforge`

## Specialized
Prerequisite: `tech_pi_specialized_planetary_mega_engineering` (2 total)

### Base Variant
- `decision_pi_gaia_biosphere_preservation_webbing` -> `pi_d_gaia_biosphere_preservation_webbing`

##### Hive Variant
- `decision_pi_hive_gaia_biosphere_preservation_webbing` -> `pi_d_hive_gaia_biosphere_preservation_webbing`

## Ascendant
Prerequisite: `tech_pi_ascendant_planetary_mega_engineering` (5 total)

### Base Variant
- `decision_pi_psionic_shroud_emitter` -> `pi_d_psionic_shroud_emitter`
- `decision_pi_gene_preservation_vaults` -> `pi_d_gene_preservation_vaults`
- `decision_pi_orbital_robotics_assembly_labs` -> `pi_d_orbital_robotics_assembly_labs`

##### Machine Variant
- `decision_pi_machine_orbital_robotics_assembly_labs` -> `pi_d_machine_orbital_robotics_assembly_labs`

##### Special Gate Variant
- `decision_pi_cybernetics_uplink_facility` -> `pi_d_cybernetics_uplink_facility`

## Authority and Tradition Gates

- Many deposits have three authority paths: regular, machine, and hive variants.
- Cybernetics Uplink Facility additionally requires the cybernetics tradition finisher in decision potential.

## Notes

- This is a decision-driven unlock structure: deposits are not randomly dropped from tier tech unlock alone.
- Late FTL origin/startup injection path has been removed in this fork.
