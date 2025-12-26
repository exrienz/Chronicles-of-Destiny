# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Chronicles-of-Destiny is a High Fantasy novel series writing project set in a real-world fantasy setting (not VR/game-based) that blends epic fantasy warfare with political intrigue (Game of Thrones style). The world of Mythosia is a living, breathing fantasy realm with magic, diverse races, and an existential demon threat.

**Important**: This is a "Real World" High Fantasy setting. Avoid all game mechanics terminology (classes, levels, stats, UI elements, etc.). Use in-world equivalents instead.

**Current Status:** Book 1 complete (15 chapters, fully revised), Books 2-4 planned

## Repository Structure

```
Chronicles-of-Destiny/
│
├── Book-1-Dance-of-Life-and-Death/    # BOOK 1 (✅ COMPLETE)
│   ├── 01-Planning/                   # Blueprint for Book 1
│   │   ├── Plot-Outline.md            # Overall book plot
│   │   ├── Chapter-Outline.md         # 15-chapter breakdown
│   │   └── World-State-Book-1.md      # World state at book start
│   ├── 02-Chapters/                   # 15 completed chapters
│   │   └── Chapter [N] - [Title].md   # Individual chapters (5000+ words each)
│   ├── 03-Reference/                  # Book-specific reference materials
│   │   ├── Character-Master.md        # Complete character list from Book 1
│   │   ├── Character-Status.md        # Character status at end of Book 1
│   │   ├── Demon-General-Status.md    # Demon General tracking
│   │   ├── Chapter_[N]_Critique.txt   # Editorial critiques
│   │   └── BOOK 1 - FULLY COMPLETE.md # Completion summary
│   └── World Setting/                 # BOOK 1 WORLD STATE
│       ├── Characters/                # Characters as of Book 1
│       │   ├── Main/                  # Kaelen, Elfiria, Lyra, Drakon, Aric
│       │   ├── Supporting/            # Gorim, Grimm, Aldric, Selene, Theron
│       │   ├── Antagonists/           # Demon King, Generals
│       │   └── Minor/                 # Named minor characters
│       ├── Locations/                 # Geography as of Book 1
│       │   ├── World.md               # Comprehensive location reference
│       │   ├── Arcanis.md             # Capital city details
│       │   ├── Deephollow.md          # Exiled base
│       │   └── Neutral-Spire.md       # Diplomatic tower
│       └── Items/                     # Artifacts and weapons
│           └── Items.md               # Comprehensive item reference
│
├── Book-2-Birth-of-Fallen-Hero/       # BOOK 2 (📝 PLANNED)
│   ├── 01-Planning/                   # Plot outline (ready)
│   ├── 02-Chapters/                   # (Empty - write chapters here)
│   ├── 03-Reference/                  # (Create after completion)
│   └── World Setting/                 # BOOK 2 WORLD STATE (create when writing)
│
├── Book-3-Darkest-Light/              # BOOK 3 (📝 PLANNED)
│   └── [Same structure]
│
├── Book-4-TBD/                        # BOOK 4 (📝 PLANNED)
│   └── [Same structure]
│
├── Plot Setting/                      # Cross-book plot documentation
│
├── CLAUDE.md                          # This file - AI instructions
├── README.md                          # Project summary
├── PROJECT-README.md                  # Comprehensive project guide
└── requirement.txt                    # Chapter generation requirements
```

## Key Organizational Principle: Per-Book World Setting

Each book has its OWN `World Setting/` folder that tracks the state of the world AT THAT POINT in the story:

- **Book 1 World Setting**: Characters, locations, and items as they exist at the END of Book 1
- **Book 2 World Setting**: Will inherit from Book 1 but track new changes independently
- **Book 3 World Setting**: Will inherit from Books 1-2 state

This allows tracking character deaths, new abilities, location changes, and world events per book.

## Key Concepts

### Writing Workflow

The primary workflow is defined in `requirement.txt`, which contains detailed instructions for generating novel chapters. When the user requests "write novel chapter [X] book [Y]", follow this framework:

1. **Navigate to Book Folder**: Go to `Book-[Y]-[Title]/`

2. **Blueprint Implementation**: Execute chapter content based on planning documents
   - Read `Book-[Y]/01-Planning/Chapter-Outline.md` for detailed chapter specifications
   - Read `Book-[Y]/01-Planning/Plot-Outline.md` for overall book arc
   - The chapter itself should BE the blueprint implementation, not continue beyond it

3. **World-Building Consistency**: Reference the PREVIOUS book's `World Setting/` for world state
   - For Book 2: Check `Book-1-Dance-of-Life-and-Death/World Setting/`
   - For Book 3: Check `Book-2-Birth-of-Fallen-Hero/World Setting/`
   - Characters: `World Setting/Characters/` (Main, Supporting, Antagonists, Minor)
   - Locations: `World Setting/Locations/`
   - Items: `World Setting/Items/`

4. **Previous Books Reference**: Check earlier books for established continuity
   - `Book-[X-1]/03-Reference/` for character status, world changes
   - **Never** reference future books (maintains chronological integrity)

5. **Chapter Writing**:
   - Minimum 5000 words per chapter in light novel style
   - Balance: action, political intrigue, character development, humor, mature romance (20+ audience)
   - Save to `Book-[Y]/02-Chapters/Chapter [X] - [Title].md`

6. **After Completion**: Create/update `World Setting/` for the current book when done

### World-Building System

The world of Mythosia is governed by interconnected systems:

- **Magic Systems**: Three primary types (Aether/Celestial, Elemental, Shadow/Void)
- **Races**: 9 distinct races including Humans, Elves, Aasimar, Dragons, etc.
- **Factions**: Alliance of Light (within Holy Dome), The Exiled, Demon Army
- **Key Artifact**: The Holy Dome protecting four kingdoms

### Character Status (End of Book 1)

Quick reference from `Book-1-Dance-of-Life-and-Death/World Setting/Characters/`:

| Character | Status | Role |
|-----------|--------|------|
| **Kaelen** | ALIVE | Commander of The Exiled |
| **Lyra** | ALIVE | Second-in-Command |
| **Drakon** | ALIVE | Key Commander |
| **Elfiria** | DECEASED (Ch14) | Was High Priestess |
| **Aric** | DECEASED (Ch8) | Was Sword Saint mentor |

Demon Generals: Malakor (active), Dravos (active), Xylos (CAPTURED), Vex (wounded), Noxia (DECEASED)

## Documentation Management

### When Creating/Editing World-Building Files

1. **Per-Book Updates**: Update the relevant book's `World Setting/` folder
2. **Character Profiles**: Track character changes in that book's `World Setting/Characters/`
3. **Location Details**: Add new locations to that book's `World Setting/Locations/`
4. **Chronological Data**: Ensure Book N content doesn't reference Books N+1 and beyond

### When Generating Novel Content

1. Reference `requirement.txt` for complete generation instructions
2. Navigate to appropriate book folder: `Book-[X]-[Title]/`
3. Check planning documents in `01-Planning/`
4. Verify details against PREVIOUS book's `World Setting/`
5. Check previous books' `03-Reference/` for continuity
6. Follow the blueprint specifications exactly (POV, key events, tone)
7. Save chapters to `Book-[X]/02-Chapters/`
8. After book completion, create `World Setting/` for that book

## Quick Reference Commands

### When asked to "write novel chapter [X] book [Y]":

1. **Navigate**: Go to `Book-[Y]-[Title]/` folder
2. **Read Planning**: `01-Planning/Chapter-Outline.md` and `Plot-Outline.md`
3. **Check World State**: Read `Book-[Y-1]/World Setting/` for world state entering Book Y
4. **Check Previous Books**: Read `Book-[Y-1]/03-Reference/` for continuity
5. **Generate**: Write 5000+ word chapter following blueprint
6. **Save**: To `Book-[Y]/02-Chapters/Chapter [X] - [Title].md`

### File Locations Quick Map

| What | Where |
|------|-------|
| **Character Profiles** | `Book-[X]/World Setting/Characters/[Role]/[Name].md` |
| **Locations** | `Book-[X]/World Setting/Locations/` |
| **Items** | `Book-[X]/World Setting/Items/` |
| **Book Plot** | `Book-[X]/01-Planning/Plot-Outline.md` |
| **Chapter Outline** | `Book-[X]/01-Planning/Chapter-Outline.md` |
| **Completed Chapters** | `Book-[X]/02-Chapters/` |
| **Book Reference** | `Book-[X]/03-Reference/` |
| **Writing Requirements** | `requirement.txt` (root) |

### Book Status

- **Book 1** (Dance of Life and Death): ✅ Complete (15 chapters, revised, world setting complete)
- **Book 2** (Birth of Fallen Hero): 📝 Planned
- **Book 3** (Darkest Light): 📝 Planned
- **Book 4** (TBD): 📝 Planned

## Important Notes

- **No code execution needed**: This is a documentation-based writing project
- **Consistency is critical**: The world-building must remain internally consistent
- **Per-book World Setting**: Each book tracks its own world state
- **Blueprint-driven**: Never write content beyond what the blueprint specifies
- **Data isolation**: When writing Book N, only reference Books 1 through N-1
