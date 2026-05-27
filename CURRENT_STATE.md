# PROJECT GENESIS — CURRENT STATE

## Project Overview

Project Genesis is a single-player, data-driven creature breeding and genetics simulation built in Godot 4.6.2 using C#.

The game is set within Sanctuary Site-04, a post-collapse scientific facility where the player breeds, mutates, manages, and studies synthetic organisms using a Dominant/Recessive/Mutation (D/R/M) inheritance system.

The project is currently transitioning from isolated prototype scenes into a modular multi-scene management simulation architecture.

---

# Current Gameplay Loop

1. Open Sanctuary Site-04
2. Enter Breeding Lab
3. Select Parent A
4. Select Parent B
5. Breed offspring
6. View breeding results
7. Repeat breeding loop

---

# Working Systems

## Core Systems

### DataLoader.cs
Loads:
- foundation_creatures.json
- core_traits.json

### TraitLibrary.cs
Handles:
- trait definitions
- categories
- inheritance support

### CreatureManager.cs
Central creature registry and runtime population tracking.

### BreedingManager.cs
Handles:
- breeding execution
- offspring generation
- mutation handling
- generation tracking

### SimulationAdapter.cs
Bridge layer between gameplay and simulation systems.

### GodotEventStore.cs
Runtime event/logging system.

---

# Current Scene Structure

## SanctuarySite04.tscn

Primary gameplay shell.

Contains:
- TopBar
- LeftFacilityMenu
- MainContentPanel
- BottomEventLog

Facilities:
- Breeding Lab
- Creature Roster (placeholder)
- Habitat Dome A (placeholder)
- Observatory (placeholder)

---

## TestScene.tscn

Legacy prototype/testing scene.

Currently still used for:
- debugging
- isolated system testing
- rapid UI iteration

---

# Active UI Systems

## BreedingLabUI.tscn

Integrated into SanctuarySite04.

Features:
- Parent selection dropdowns
- Trait preview labels
- Placeholder creature icons
- Breed button
- Reset button
- Result output

---

# Current Limitations

- No save/load system
- No habitat simulation
- No ecosystem simulation
- No final creature visuals
- Simplified genetics implementation
- Creature roster integration incomplete

---

# Immediate Next Steps

1. Integrate CreatureRosterUI
2. Build HabitatDomeUI
3. Implement save/load
4. Add habitat compatibility scoring
5. Expand event system
6. Add simulation ticking
