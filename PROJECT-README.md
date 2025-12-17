# Chronicles of Destiny

**Genre:** Fantasy Light Novel
**Style:** Sword Art Online (VR elements) meets Game of Thrones (political intrigue)
**Audience:** Mature (20+)
**Format:** Multi-book series

## Project Status

- ✅ **Book 1:** The Dance of Life and Death (15 chapters, COMPLETE)
- 📝 **Book 2:** The Birth of a Fallen Hero (Planned)
- 📝 **Book 3:** The Darkest Light (Planned)
- 📝 **Book 4:** [Title TBD] (Planned)

## Repository Structure

```
Chronicles-of-Destiny/
│
├── 00-Series/                          # Series-wide resources
│   ├── World-Building/                 # Universal world lore
│   │   ├── Characters/                # Character profiles (organized by role)
│   │   ├── Locations/                 # Geography and places
│   │   ├── Magic.md                   # Magic systems
│   │   ├── Races.md                   # Races of Mythosia
│   │   ├── Jobs.md                    # Job/class progression
│   │   ├── Items/                     # Important artifacts
│   │   └── Pre-War-Country.md         # Historical kingdoms
│   └── README.md                       # Series overview guide
│
├── Book-1-Dance-of-Life-and-Death/    # Book 1 (COMPLETE)
│   ├── 01-Planning/                   # Plot outlines and blueprints
│   ├── 02-Chapters/                   # 15 completed chapters
│   ├── 03-Reference/                  # Summaries and completion docs
│   └── README.md                       # Book 1 guide
│
├── Book-2-Birth-of-Fallen-Hero/       # Book 2 (PLANNED)
│   ├── 01-Planning/                   # Plot outline (ready)
│   ├── 02-Chapters/                   # (Empty - not yet written)
│   ├── 03-Reference/                  # (Empty - create after writing)
│   └── README.md                       # Book 2 guide
│
├── Book-3-Darkest-Light/              # Book 3 (PLANNED)
│   └── [Same structure as Book 2]
│
├── Book-4-TBD/                        # Book 4 (PLANNED)
│   └── [Same structure as Book 2]
│
├── CLAUDE.md                          # AI writing assistant instructions
├── requirement.txt                    # Chapter generation requirements
└── PROJECT-README.md                  # This file
```

## Quick Start Guide

### For Writing New Chapters

1. **Choose Your Book** - Navigate to the book folder (e.g., `Book-2-Birth-of-Fallen-Hero/`)
2. **Check Planning** - Read `01-Planning/` files (plot outline, chapter outline, world state)
3. **Reference World-Building** - Check `00-Series/World-Building/` for:
   - Character profiles and status
   - Location details
   - Magic system rules
   - Race and job information
4. **Write Chapter** - Follow `requirement.txt` guidelines (5000+ words, light novel style)
5. **Save Chapter** - Place in book's `02-Chapters/` folder
6. **Update References** - After book completion, update `03-Reference/` materials

### For Referencing Previous Books

When writing Book N, you can reference:
- ✅ All events from Books 1 through N-1
- ✅ World-building from `00-Series/World-Building/`
- ✅ Character status from previous books' `03-Reference/` folders
- ❌ Future books (maintains chronological integrity)

## Key Files

| File | Purpose |
|------|---------|
| **CLAUDE.md** | Instructions for AI writing assistant |
| **requirement.txt** | Chapter generation requirements and style guide |
| **00-Series/World-Building/** | Universal lore (magic, races, jobs, etc.) |
| **00-Series/World-Building/Characters/** | All character profiles organized by role |
| **Book-X/01-Planning/** | Plot and chapter outlines for each book |
| **Book-X/02-Chapters/** | Actual written chapters |
| **Book-X/03-Reference/** | Book summaries and world state after completion |

## Writing Workflow

### Starting a New Book

1. Review previous book's `03-Reference/World-Changes.md`
2. Create `World-State-Book-X.md` in new book's `01-Planning/`
3. Expand plot outline into detailed chapter outline
4. Begin writing chapters based on chapter outline

### While Writing

1. Reference `requirement.txt` for style and content requirements
2. Check character profiles for consistency
3. Verify magic/race/job rules in world-building files
4. Maintain 5000+ word minimum per chapter
5. Balance action, politics, character development, humor, romance

### After Completing a Book

1. Create summary in `03-Reference/Book-Summary.md`
2. Document character status changes in `03-Reference/Character-Status.md`
3. Record world changes in `03-Reference/World-Changes.md`
4. Update character profiles in `00-Series/World-Building/Characters/` if needed

## World of Mythosia

### Magic Systems
1. **Aether/Celestial** - Divine magic
2. **Elemental** - Nature-based magic
3. **Shadow/Void** - Dark magic

### Major Factions (as of Book 1 end)
- **Alliance of Light** - Four kingdoms within Holy Dome
- **The Exiled** - Resistance in outer lands (led by Kaelen)
- **Demon Army** - Demon King and Generals controlling outer lands

### Key Locations
- **Inner Kingdoms** (Protected by Holy Dome): Aetheria, Eldoria, Sylvanaria, Drakoria
- **Fallen Outer Lands**: Kharaz'Mar, Luminara, Aridia
- **Deephollow** - The Exiled's base

## Character Organization

Characters are organized by role in `00-Series/World-Building/Characters/`:
- **Main/** - Protagonists and central characters
- **Supporting/** - Important allies and secondary characters
- **Antagonists/** - Villains and demon forces
- **Minor/** - Named but less significant characters

See `00-Series/World-Building/Characters/README.md` for character index.

## Core Themes

- Sacrifice and moral complexity
- Love and relationships in war
- Found family and brotherhood
- Heroism vs. pragmatism
- Power and corruption
- Hope in darkness

## Writing Style

- **Format:** Light novel (5000+ words per chapter)
- **Tone:** Balanced action, politics, character development
- **Content:** Mature themes including combat, romance, and moral dilemmas
- **Humor:** Witty dialogue and character banter
- **POV:** Multiple perspectives when appropriate

## Version Control Notes

Old folder structure (deprecated):
- `World Setting/` → Moved to `00-Series/World-Building/`
- `Plot Setting/` → Distributed to each book's `01-Planning/`
- `Book/` → Renamed to `Book-X-Title/` with better organization

All files have been reorganized for easier multi-book management.

## Contact & Contribution

This is a private novel project. For questions or collaboration, contact the repository owner.
