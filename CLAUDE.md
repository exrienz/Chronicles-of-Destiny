# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Chronicles-of-Destiny is a High Fantasy novel series writing project set in a real-world fantasy setting (not VR/game-based) that blends epic fantasy warfare with political intrigue (Game of Thrones style). The world of Mythosia is a living, breathing fantasy realm with magic, diverse races, and an existential demon threat. The project is organized for multi-book series management with clear separation between universal world-building and book-specific content.

**Important**: This is a "Real World" High Fantasy setting. Avoid all game mechanics terminology (classes, levels, stats, UI elements, etc.). Use in-world equivalents instead.

**Current Status:** Book 1 complete (15 chapters), Books 2-4 planned

## Repository Structure

```
Chronicles-of-Destiny/
│
├── 00-Series/                          # SERIES-WIDE RESOURCES
│   ├── World-Building/                 # Universal world lore (consistent across all books)
│   │   ├── Characters/                 # Character profiles organized by role
│   │   │   ├── README.md              # Character index and quick reference
│   │   │   ├── Main/                  # Protagonists (Kaelen, Elfiria, Lyra, Drakon, Aric)
│   │   │   ├── Supporting/            # Allies (Grimm, Gorim, Aldric, Selene, etc.)
│   │   │   ├── Antagonists/           # Villains (Demon King, Generals)
│   │   │   └── Minor/                 # Named minor characters
│   │   ├── Locations/                 # Geography (World.md, Arcanis.md, etc.)
│   │   ├── Magic.md                   # Magic systems (Aether, Elemental, Shadow/Void)
│   │   ├── Races.md                   # Race descriptions and traits
│   │   ├── Jobs.md                    # Job/class progression paths
│   │   ├── Items/                     # Important artifacts
│   │   └── Pre-War-Country.md         # Historical kingdom info
│   └── README.md                       # Series overview guide
│
├── Book-1-Dance-of-Life-and-Death/    # BOOK 1 (✅ COMPLETE)
│   ├── 01-Planning/                   # Blueprint for Book 1
│   │   ├── Plot-Outline.md            # Overall book plot
│   │   ├── Chapter-Outline.md         # 15-chapter detailed breakdown
│   │   └── World-State-Book-1.md      # World state at book start
│   ├── 02-Chapters/                   # 15 completed chapters
│   │   ├── Chapter 1 - Ashes and Echoes.md
│   │   ├── Chapter 2 - The Domino Falls.md
│   │   └── ... (Chapters 3-15)
│   ├── 03-Reference/                  # Book completion materials
│   │   ├── Book-Summary.md            # Complete book summary
│   │   └── BOOK 1 - FULLY COMPLETE.md
│   └── README.md                       # Book 1 guide
│
├── Book-2-Birth-of-Fallen-Hero/       # BOOK 2 (📝 PLANNED)
│   ├── 01-Planning/
│   │   └── Plot-Outline.md            # Book 2 plot (ready)
│   ├── 02-Chapters/                   # (Empty - write chapters here)
│   ├── 03-Reference/                  # (Create after completion)
│   └── README.md
│
├── Book-3-Darkest-Light/              # BOOK 3 (📝 PLANNED)
│   └── [Same structure as Book 2]
│
├── Book-4-TBD/                        # BOOK 4 (📝 PLANNED)
│   └── [Same structure as Book 2]
│
├── CLAUDE.md                          # This file - AI instructions
├── requirement.txt                    # Chapter generation requirements
└── PROJECT-README.md                  # Comprehensive project guide
```

### Old Structure (Deprecated)
- `World Setting/` → Moved to `00-Series/World-Building/`
- `Plot Setting/` → Distributed to each book's `01-Planning/`
- `Book/` → Reorganized to `Book-X-Title/` with Planning/Chapters/Reference folders

## Key Concepts

### Writing Workflow

The primary workflow is defined in `requirement.txt`, which contains detailed instructions for generating novel chapters. When the user requests "write novel chapter [X] book [Y]", follow this framework:

1. **Navigate to Book Folder**: Go to `Book-[Y]-[Title]/`
   - Example: `Book-2-Birth-of-Fallen-Hero/` for Book 2

2. **Blueprint Implementation**: Execute chapter content based on planning documents
   - Read `Book-[Y]/01-Planning/Chapter-Outline.md` for detailed chapter specifications
   - Read `Book-[Y]/01-Planning/Plot-Outline.md` for overall book arc
   - The chapter itself should BE the blueprint implementation, not continue beyond it
   - Modifications to improve quality are allowed but document them

3. **World-Building Consistency**: Reference `00-Series/World-Building/` for universal lore
   - **Characters**: `00-Series/World-Building/Characters/` (organized by role)
     - See `Characters/README.md` for quick reference and status
     - Main protagonists in `Characters/Main/` (The Trinity, Elfiria, Aric)
     - Supporting cast in `Characters/Supporting/` (Grimm, Gorim, Aldric, etc.)
     - Antagonists in `Characters/Antagonists/` (Demon King, Generals)
   - **Magic**: `00-Series/World-Building/Magic.md` (Aether/Celestial, Elemental, Shadow/Void)
   - **Jobs**: `00-Series/World-Building/Jobs.md` (18+ paths, 4-tier progression)
   - **Locations**: `00-Series/World-Building/Locations/` (World.md for geography)
   - **Races**: `00-Series/World-Building/Races.md`

4. **Previous Books Reference**: Check earlier books for established continuity
   - For Book 2: Can reference all `Book-1-Dance-of-Life-and-Death/` content
   - For Book 3: Can reference Books 1-2
   - Check `Book-[X]/03-Reference/` folders for summaries and world changes
   - **Never** reference future books (maintains chronological integrity)

5. **Chapter Writing**:
   - Minimum 5000 words per chapter in light novel style
   - Balance: action, political intrigue, character development, humor, mature romance (20+ audience)
   - Save to `Book-[Y]/02-Chapters/Chapter [X] - [Title].md`

6. **After Completion**: Update reference materials in `Book-[Y]/03-Reference/` when book is done

### World-Building System

The world of Mythosia is governed by interconnected systems:

- **Magic Systems**: Three primary types (Aether/Celestial, Elemental, Shadow/Void) with distinct sources and users
- **Job Progression**: 18+ job paths with 4-tier progression (Base → 2nd Job → 3rd Job → Hidden Legendary)
- **Races**: 9 distinct races including Humans, Elves, Aasimar, Dragons, etc.
- **Factions**: Alliance of Light (5 kingdoms), Shadow Forces, Demon Army (7 Generals)
- **Key Artifact**: The Holy Dome protecting Aetheria, Eldoria, Kharaz'Mar, and Sylvanaria

### Character Relationships

Character profiles are comprehensively documented in `World Setting/Characters/`:
- **The Trinity** (Legendary Fighting Unit): Kaelen, Lyra, Drakon - unbreakable bonds
- **Kaelen** (Protagonist in `Main/Kaelen.md`): Dual-wielder awakening Sword Saint abilities
- **Elfiria** (Main Heroine in `Main/Elfiria.md`): High Priestess, Holy Dome vessel (DECEASED Book 1 Ch14)
- **Lyra** (Support in `Main/Lyra.md`): Sniper, exiled elf, The Exiled second-in-command
- **Drakon** (Best Friend in `Main/Drakon.md`): Dragon Knight from Drakoria
- **Aric** (Mentor in `Main/Aric.md`): Sword Saint mentor (DECEASED Book 1 Ch8)

See `Characters/README.md` for complete relationship maps and status tracking

## Documentation Management

### When Creating/Editing World-Building Files

1. **Maintain Consistency**: Cross-reference existing files in `00-Series/World-Building/` before adding new lore
2. **Update Character Profiles**: Track character changes in `00-Series/World-Building/Characters/`
   - Main characters go in `Characters/Main/`
   - Supporting characters in `Characters/Supporting/`
   - Antagonists in `Characters/Antagonists/`
   - Minor characters in `Characters/Minor/`
   - Update `Characters/README.md` when adding new characters
3. **Location Details**: Add new locations to `00-Series/World-Building/Locations/` with proper structure
4. **Chronological Data**: Ensure Book N content doesn't reference Books N+1 and beyond

### When Generating Novel Content

1. Reference `requirement.txt` for complete generation instructions
2. Navigate to appropriate book folder: `Book-[X]-[Title]/`
3. Check planning documents:
   - `Book-[X]/01-Planning/Chapter-Outline.md` for detailed chapter blueprint
   - `Book-[X]/01-Planning/Plot-Outline.md` for overall book arc
   - `Book-[X]/01-Planning/World-State-Book-[X].md` for world state at book start
4. Verify all details against `00-Series/World-Building/`:
   - Character personalities, abilities, and relationships
   - Location descriptions and geography
   - Magic system rules and limitations
   - Job progression and abilities
5. Check previous books' reference materials:
   - `Book-[X-1]/03-Reference/Book-Summary.md` for what happened before
   - `Book-[X-1]/03-Reference/Character-Status.md` for character states
   - `Book-[X-1]/03-Reference/World-Changes.md` for world state changes
6. Follow the blueprint specifications exactly (POV, key events, tone)
7. Save generated chapters to `Book-[X]/02-Chapters/` directory with format: `Chapter [N] - [Title].md`
8. Update `00-Series/World-Building/` if new canonical information is established
9. After book completion, update `Book-[X]/03-Reference/` with summaries and changes

## Git Workflow

**Structure Migration Note**: The repository was reorganized in December 2024 from flat `World Setting/`, `Plot Setting/`, and `Book/` directories to the current book-centric structure.

### When Committing

- **Chapter content**: Goes in `Book-[X]-[Title]/02-Chapters/`
- **World-building updates**: Goes in `00-Series/World-Building/`
- **Plot modifications**: Goes in `Book-[X]-[Title]/01-Planning/`
- **Reference materials**: Goes in `Book-[X]-[Title]/03-Reference/`

### Commit Message Format
- "Add Book [X] Chapter [N]: [Chapter Title]"
- "Update character profile: [Character Name]"
- "Add Book [X] planning: [Description]"
- "Update world-building: [Area]"

### Old Structure (Deprecated)
The old folders (`World Setting/`, `Plot Setting/`, `Book/`) are kept for reference but the new structure should be used for all new work.

## Important Notes

- **No code execution needed**: This is a documentation-based writing project
- **Consistency is critical**: The world-building must remain internally consistent across all files
- **Markdown format**: All content is in Markdown for easy editing and version control
- **Blueprint-driven**: Never write content beyond what the blueprint specifies for a chapter
- **Data isolation**: When writing Book 1, ignore Book 2+ data to prevent anachronisms
- **Status**: Book 1 (15 chapters) is complete. Books 2-4 are outlined but not yet written.

## Quick Reference Commands

### When asked to "write novel chapter [X] book [Y]":

1. **Navigate**: Go to `Book-[Y]-[Title]/` folder
2. **Read Planning**:
   - `Book-[Y]/01-Planning/Chapter-Outline.md` for chapter blueprint
   - `Book-[Y]/01-Planning/Plot-Outline.md` for overall arc
3. **Check World-Building**: Read relevant `00-Series/World-Building/` files:
   - Characters, Locations, Magic, Races, Jobs
4. **Check Previous Books**: Read `Book-[Y-1]/03-Reference/` for continuity
5. **Generate**: Write 5000+ word chapter following blueprint
6. **Save**: To `Book-[Y]/02-Chapters/Chapter [X] - [Title].md`

### File Locations Quick Map

| What | Where |
|------|-------|
| **Character Profiles** | `00-Series/World-Building/Characters/[Role]/[Name].md` |
| **Magic System** | `00-Series/World-Building/Magic.md` |
| **Locations** | `00-Series/World-Building/Locations/` |
| **Book Plot** | `Book-[X]-[Title]/01-Planning/Plot-Outline.md` |
| **Chapter Outline** | `Book-[X]-[Title]/01-Planning/Chapter-Outline.md` |
| **Completed Chapters** | `Book-[X]-[Title]/02-Chapters/` |
| **Book Summary** | `Book-[X]-[Title]/03-Reference/Book-Summary.md` |
| **Writing Requirements** | `requirement.txt` (root) |

### Book Status

- **Book 1** (Dance of Life and Death): ✅ Complete (15 chapters)
- **Book 2** (Birth of Fallen Hero): 📝 Planned
- **Book 3** (Darkest Light): 📝 Planned
- **Book 4** (TBD): 📝 Planned
