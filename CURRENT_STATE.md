# PROJECT GENESIS — CURRENT STATE

## Project Overview

Project Genesis is a single-player, data-driven creature breeding and genetics simulation built in Godot 4.6.2 using C#.

The game is set within Sanctuary Site-04, a post-collapse scientific facility where the player breeds, mutates, manages, and studies synthetic organisms using a Dominant/Recessive/Mutation (D/R/M) inheritance system.

Project Genesis is transitioning from prototype breeding simulation toward a true management-style scientific genetics and creature stewardship simulator.

---

# Current Gameplay Loop

Current functional gameplay loop:

1. Open Sanctuary Site-04
2. Enter Breeding Lab
3. Select Parent A
4. Select Parent B
5. Review projected offspring estimates
6. Breed offspring
7. View breeding results
8. Repeat breeding loop

---

# Working Systems

## Core Systems

### DataLoader.cs
Loads:
- foundation_creatures.json
- core_traits.json

### TraitLibrary.cs
Manages:
- trait definitions
- trait categories
- inheritance support
- mutation references

### CreatureManager.cs
Central runtime registry for:
- all loaded creatures
- generated offspring
- runtime population tracking

### BreedingManager.cs
Handles:
- breeding execution
- offspring creation
- inheritance logic
- mutation generation
- generation tracking
- inbreeding calculations

### SimulationAdapter.cs
Bridge layer between simulation systems and UI systems.

### GodotEventStore.cs
Runtime event messaging and notification foundation.

---

## Predictive Breeding System

Breeding UI now includes projected offspring estimation including:
- projected stat tendencies
- mutation variance display
- lineage projection
- live parent pairing analysis

This transitions the breeding system from pure RNG breeding toward intentional genetics management gameplay.

---

# Current Scene Structure

## SanctuarySite04.tscn

Primary game shell.

Contains:
- top status bar
- facility sidebar
- dynamic gameplay panel
- event log terminal
- facility routing system

Current facilities:
- Breeding Lab
- Creature Roster
- Habitat Dome A placeholder
- Observatory placeholder

## TestScene.tscn

Legacy prototype/testing environment.

Still useful for:
- isolated debugging
- UI experiments
- breeding debugging
- rapid iteration

---

# Current UI Identity

The UI is converging toward a scientific breeding terminal.

Current strengths:
- live parent pairing
- projected offspring panel
- trait/stat preview
- mutation variance readability
- sanctuary event feed
- modular facility layout

Current weakness:
- registry/card readability still needs improvement

---

# Current Limitations

- No save/load system
- Habitat simulation not started
- Creature roster needs stronger card-based UX
- No visual lineage/family tree
- Advanced D/R/M dominance conflicts are still simplified
- Placeholder creature icons
- Event logging is minimal

---

# Immediate Next Steps

1. Build CreatureCard.tscn
2. Integrate CreatureCard into Creature Roster
3. Add trait color coding
4. Add mutation/stability indicators
5. Add lineage viewer
6. Build HabitatDomeUI
7. Add habitat compatibility scoring
8. Implement save/load persistence
