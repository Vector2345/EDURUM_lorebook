# EDRUM_lorebook
A SillyTavern WorldInfo lorebook for an original high fantasy RPG setting — **Ederum**.

## About
Ederum is a high fantasy world featuring two rival empires, complex morality, and a first-person narrative system. Built for immersive TTRPG-style play with real consequences.

Developed over iterative testing sessions with assistance from Claude (Anthropic).

## Features
- 36 WorldInfo entries with keyword triggers
- DO / SAY / STORY command system
- Faction-aware NPC knowledge system
- Legal system with consequences — arrest, trial, execution
- Three different prison systems per race
- Magical shackles system for three races
- Class determination through player behavior

## Requirements
- [SillyTavern](https://github.com/SillyTavern/SillyTavern)

## Recommended Model
**L3-8B-Stheno-v3.2-Q4_K_M**

Tested and optimized for this model. Other roleplay-focused models should work but are untested.

## Files

| File | Description |
|------|-------------|
| `edrum_worldinfo_v10.json` | Main WorldInfo lorebook |
| `edrum_system_prompt_v5.txt` | System prompt |
| `Game Master EDURUM.json` | Character card with built-in prompt and opening message |
| `Default.json` | Sampler settings — temperature, penalties, generation parameters |
| `ST-formatting-2026-03-01.json` | SillyTavern response format settings |

## Setup
1. Import `edrum_worldinfo_v10.json` into SillyTavern WorldInfo
2. Load `edrum_system_prompt_v5.txt` as system prompt
3. Import `Game Master EDURUM.json` as character card
4. Import `Default.json` into your sampler settings
5. Import `ST-formatting-2026-03-01.json` into SillyTavern formatting settings

## Commands
- `DO [action]` — physical action
- `SAY "[dialogue]"` — speak to NPC
- `STORY [reflection]` — inner narrative or time skip

## License
GNU General Public License v2.0
