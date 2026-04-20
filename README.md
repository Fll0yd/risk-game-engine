# AI Risk (Python Strategy Game)

## Overview
A Python-based implementation of the classic board game **Risk**, featuring turn-based gameplay, territory control, combat mechanics, and basic AI decision-making.

This project models the core systems of Risk, including:
- Territory ownership and troop management
- Adjacency-based movement and combat
- Reinforcement and continent bonuses
- Card trading system
- Basic AI player behavior

Built as a deep-dive into game logic, state management, and rule-based systems.

---

## Features

- Full world map with territories and adjacency graph
- Turn-based gameplay loop
- Troop placement and reinforcement system
- Attack phase with dice mechanics
- Fortification phase with path validation
- Card system with trade-in bonuses
- Basic AI turn logic
- Win condition detection

---

## Tech Stack

- **Python**
- Standard libraries (`random`, `time`)
- Object-oriented design

---

## How to Run

```bash
python AIRISK.py
```

Game runs in the terminal with interactive prompts.

## Project Purpose

This project was built to explore:

Complex rule-based systems
Game state modeling
Graph structures (territory adjacency)
Turn-based game loops
Basic AI decision-making
Managing large interconnected data structures

## Current Status

⚠️ Work in Progress / Incomplete

The core systems are partially implemented, but the game is not fully stable or compliant with official Risk rules.

Known issues include:

Inconsistent data structures (players used as both list and dict)
Some function signature mismatches
Incomplete or buggy game flow logic
Missing validation and edge-case handling
AI behavior is simplistic and not strategic


## ⚠️ Important Note on Game Rules

This implementation focuses on core classic Risk mechanics only.

Features such as:

Alliances
Truces
Draw proposals
Peace treaties
Ceasefires

are NOT part of official Risk rules and are not currently implemented.

These could be added later as optional “house rules” or advanced gameplay features.


## Future Improvements
focus on these in order:

### 1. Fix Core Architecture
Standardize players data structure (use dict consistently)
Separate game state, logic, and UI (even if CLI-based)
Break large methods into smaller, testable functions

### 2. Stabilize Game Loop
Clean up turn flow:
Reinforcement
Attack
Fortify
Ensure players can:
Skip phases
End turn cleanly
Fix infinite loops and edge cases

### 3. Fix Combat System
Align attack logic with official rules:
Max 3 dice attacker / 2 defender
Proper dice comparisons
Fix function signature mismatch in attack()

### 4. Validate Map Integrity
Ensure all territories exist and match adjacency map
Fix missing references (e.g. Afghanistan inconsistencies)
Consider moving map data to external JSON file

### 5. Improve AI
Replace random behavior with:
Threat evaluation
Territory prioritization
Strategic reinforcement
Add difficulty levels

### 6. Add CLI UX Improvements
Clearer prompts and feedback
Display current game state (territories, troop counts)
Show player summaries each turn

### 7. Add Save/Load System
Serialize game state to file
Allow resume of long matches

### 8. Optional Advanced Features
(ONLY after core game is stable)
House rules (alliances, diplomacy)
Multiplayer support
GUI (Tkinter or Pygame)
Web version (Flask / FastAPI)


## Strategic Note
This project demonstrates:
Complex system design
State management across many entities
Rule-based logic implementation


Author

Kenneth Lloyd Boller
