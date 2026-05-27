# PROJECT GENESIS — ARCHITECTURE

# Engine

- Godot 4.6.2
- C#
- JSON-driven architecture

---

# Core Design Philosophy

Project Genesis uses:
- modular facility scenes
- centralized managers
- data-driven creatures
- dynamic UI routing

---

# Autoload Systems

## CreatureManager
Runtime creature registry.

## TraitLibrary
Trait definition system.

## BreedingManager
Inheritance and offspring generation.

## SimulationAdapter
UI ? simulation bridge.

## GodotEventStore
Runtime event messaging/logging.

---

# SanctuarySite04.tscn

Primary game shell.

Hierarchy:

SanctuarySite04
+-- DataLoader
+-- GameBootstrap
+-- MarginContainer
¦
+-- VBoxContainer
    +-- TopBar
    +-- MainSection
    ¦   +-- LeftFacilityMenu
    ¦   +-- MainContentPanel
    ¦
    +-- BottomEventLog

---

# MainContentPanel

Dynamic facility loading region.

Current implementation:
- PackedScene loading
- runtime instantiation
- cleanup before replacement

---

# Facility Scenes

Current:
- BreedingLabUI.tscn

Planned:
- CreatureRosterUI.tscn
- HabitatDomeUI.tscn
- ObservatoryUI.tscn

---

# Data Pipeline

Creature JSON
?
DataLoader
?
CreatureManager
?
BreedingManager
?
Runtime offspring population

---

# Initialization Order

Correct order:
1. DataLoader
2. GameBootstrap
3. Autoload systems
4. Facility scene loading

Incorrect order causes:
- empty breeding dropdowns
- missing creature population

---

# Current Technical Priorities

1. Complete facility integration
2. Add persistence
3. Build habitat simulation
4. Expand event system
5. Add simulation ticking
