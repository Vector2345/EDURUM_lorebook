# EDRUM_lorebook
A SillyTavern WorldInfo lorebook for an original high fantasy RPG setting — **Ederum**.

## About
Ederum is a high fantasy world featuring two rival empires, complex morality, and a first-person narrative system. Built for immersive TTRPG-style play with real consequences.

Developed over iterative testing sessions with assistance from Claude (Anthropic).

## Features
- 36 WorldInfo entries with keyword triggers
- DO / SAY / STORY command system
- d20 dice mechanics
- Faction-aware NPC knowledge system
- Legal system with consequences — arrest, trial, execution
- Three different prison systems per race
- Magical shackles system for three races
- Class determination through player behavior

## Requirements
- [SillyTavern](https://github.com/SillyTavern/SillyTavern)
- **D&D Dice** extension for SillyTavern — required for d20 mechanics

## Recommended Model
**L3-8B-Stheno-v3.2-Q4_K_M**

Tested and optimized for this model. Other roleplay-focused models should work but are untested.

## Files

| File | Description |
|------|-------------|
| `edrum_worldinfo_v9.json` | Main WorldInfo lorebook |
| `edrum_system_prompt_v5.txt` | System prompt |
| `Game Master EDURUM.json` | Character card with built-in prompt and opening message |
| `Default.json` | Sampler settings — temperature, penalties, generation parameters |
| `ST-formatting-2026-03-01.json` | SillyTavern response format settings |

## Setup
1. Install **D&D Dice** extension in SillyTavern
2. Import `edrum_worldinfo_v9.json` into SillyTavern WorldInfo
3. Load `edrum_system_prompt_v5.txt` as system prompt
4. Import `Game Master EDURUM.json` as character card
5. Import `Default.json` into your sampler settings
6. Import `ST-formatting-2026-03-01.json` into SillyTavern formatting settings

## How Dice Work

D&D Dice extension rolls automatically on every DO action. The GM describes the outcome based on the result shown at the end of each response.

**Write your action:**
```
DO attack the guard
```

**D&D Dice rolls, GM describes the outcome:**
```
[Roll: 7]
```

### Roll Results (d20)

| Roll | Result |
|------|--------|
| 1 | Critical fail — worst possible outcome, death is possible |
| 2–5 | Fail — action failed, real consequences |
| 6–10 | Partial fail — succeeded with complications |
| 11–15 | Success |
| 16–19 | Success with advantage |
| 20 | Critical success |

**The GM never saves your character on a low roll.** A roll of 1–5 in a dangerous situation means failure — no lucky escapes, no divine intervention.

## Commands
- `DO [action]` — physical action, dice roll automatic
- `SAY "[dialogue]"` — speak to NPC
- `STORY [reflection]` — inner narrative or time skip

## License
GNU General Public License v2.0
