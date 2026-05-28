# PROJECT GENESIS — ACTIVE TASKS

# Highest Priority

- Build CreatureCard.tscn as the reusable biological specimen UI unit
- Integrate CreatureCard into Creature Roster
- Improve registry readability and information density
- Add mutation/rarity visual indicators
- Add color-coded trait visualization
- Improve parent slot visual presentation
- Improve offspring prediction display with ranges and risk labels

---

# In Progress

## SanctuarySite04 Migration

Completed:
- SanctuarySite04 shell
- facility navigation
- dynamic MainContentPanel scene loading
- BreedingLabUI integration
- predictive breeding / offspring projection panel
- mutation variance display

Pending:
- Creature Roster full integration
- Habitat Dome integration
- Observatory integration

---

# Current Design Priority

The project is now moving from:

simple breeding prototype

toward:

scientific creature stewardship and genetics management simulation

The immediate bottleneck is no longer missing breeding functionality. The bottleneck is data readability and registry UX.

---

# Pending Integration

## CreatureCard System

Needed:
- reusable CreatureCard.tscn
- CreatureCardUI.cs
- use in roster rows
- use in parent slots
- use in future lineage viewer
- use in future habitat assignment

---

## CreatureRosterUI

Needed:
- scene modularization if not already completed
- dynamic loading support in SanctuarySite04
- creature detail display
- specimen card list
- search/filter/sort support

---

## HabitatDomeUI

Needed after roster/card work:
- environmental stats
- creature assignment
- compatibility calculations
- habitat population display

---

## Save System

Needed:
- runtime creature serialization
- JSON save format
- save/load manager
- persistent progression

---

# Known Blockers

- No save/load system
- Placeholder creature visuals
- Registry is still too text-row oriented
- Simulation complexity is beginning to outpace UI readability
- Habitat compatibility not implemented yet

---

# Recommended Next Steps

1. Build CreatureCard.tscn
2. Integrate CreatureCard into CreatureRosterUI
3. Add trait color coding
4. Add mutation/stability indicators
5. Add lineage viewer
6. Build HabitatDomeUI
7. Add compatibility scoring
8. Implement SaveGameManager
9. Expand event logging
10. Improve visual polish
