# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Chronicles-of-Destiny is a fantasy novel series writing project that blends virtual reality elements (Sword Art Online style) with political intrigue (Game of Thrones style). The project consists of detailed world-building documentation and structured novel content organized for AI-assisted writing.

## Repository Structure

```
Chronicles-of-Destiny/
├── World Setting/          # Core world-building documentation
│   ├── Characters/        # Character profiles and relationships
│   ├── Locations/         # Geographic and location details
│   ├── Magic.md          # Magic systems and factions
│   ├── Races.md          # Race descriptions and traits
│   ├── jobs.md           # Class/job system with progression paths
│   └── book 1 - World State.md  # Current state of the world
├── Plot Setting/          # Book-level plot outlines
│   ├── Book 1: The Dance of Life and Death.md
│   ├── Book 2: The Birth of a Fallen Hero.md
│   ├── Book 3: The Darkest Light.md
│   └── Book 4 : xx.md
├── Book/                  # Generated novel chapters (output directory)
└── requirement.txt        # AI prompt instructions for novel generation
```

## Key Concepts

### Writing Workflow

The primary workflow is defined in `requirement.txt`, which contains detailed instructions for generating novel chapters. When the user requests "write novel chapter [X] book [Y]", follow this framework:

1. **Blueprint Implementation**: Execute chapter content based on plot outlines in `Plot Setting/`
2. **World-Building Consistency**: Reference all documentation in `World Setting/` to maintain consistency
3. **Data Management**: Strictly follow chronological progression (Book 1 can only reference Book 1 data; Book 2 can reference Books 1-2, etc.)
4. **Chapter Length**: Minimum 5000 words per chapter in light novel style
5. **Content**: Balance action, political intrigue, character development, humor, and mature romantic elements

### World-Building System

The world of Mythosia is governed by interconnected systems:

- **Magic Systems**: Three primary types (Aether/Celestial, Elemental, Shadow/Void) with distinct sources and users
- **Job Progression**: 18+ job paths with 4-tier progression (Base → 2nd Job → 3rd Job → Hidden Legendary)
- **Races**: 9 distinct races including Humans, Elves, Aasimar, Dragons, etc.
- **Factions**: Alliance of Light (5 kingdoms), Shadow Forces, Demon Army (7 Generals)
- **Key Artifact**: The Holy Dome protecting Aetheria, Eldoria, Kharaz'Mar, and Sylvanaria

### Character Relationships

Track character dynamics as defined in `World Setting/Characters/Main.md`:
- **Kaelen** (Protagonist): Swordsman → Blademaster → Sword Saint path
- **Elfiria** (Main Heroine): High Priestess, holds the Holy Dome artifact
- **Lyra** (Support/Romance): Sniper, exiled elf
- **Drakon** (Rival/Friend): Dragon Knight from Drakoria

Relationships evolve through defined arcs (Strangers → Protector/Protectee → Lovers)

## Documentation Management

### When Creating/Editing World-Building Files

1. **Maintain Consistency**: Cross-reference existing files before adding new lore
2. **Update Character Profiles**: Track relationship progression in `World Setting/Characters/`
3. **Location Details**: Add new locations to `World Setting/Locations/` with proper structure
4. **Chronological Data**: Ensure Book N content doesn't reference future books

### When Generating Novel Content

1. Reference `requirement.txt` for complete generation instructions
2. Verify all details against `World Setting/` documentation
3. Follow the blueprint in corresponding `Plot Setting/Book X` file
4. Save generated chapters to `Book/` directory with clear naming (e.g., `Book 1 Chapter 1.md`)

## Git Workflow

The repository tracks deleted files from a previous `Setting/` and `saga/` structure. The current active structure uses `World Setting/`, `Plot Setting/`, and `Book/` directories.

When committing:
- Chapter content goes in `Book/`
- World-building updates go in `World Setting/`
- Plot modifications go in `Plot Setting/`
- Include the chapter/modification scope in commit messages

## Important Notes

- **No code execution needed**: This is a documentation-based writing project
- **Consistency is critical**: The world-building must remain internally consistent across all files
- **Markdown format**: All content is in Markdown for easy editing and version control
- **Blueprint-driven**: Never write content beyond what the blueprint specifies for a chapter
- **Data isolation**: When writing Book 1, ignore Book 2+ data to prevent anachronisms
