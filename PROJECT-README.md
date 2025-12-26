# Chronicles of Destiny - Project Guide

**Genre:** Fantasy Light Novel
**Style:** Epic warfare meets political intrigue (Game of Thrones style)
**Audience:** Mature (20+)
**Format:** Multi-book series

## Project Status

| Book | Title | Chapters | Status |
|------|-------|----------|--------|
| 1 | Dance of Life and Death | 15 | ✅ Complete & Revised |
| 2 | Birth of Fallen Hero | - | 📝 Planned |
| 3 | Darkest Light | - | 📝 Planned |
| 4 | TBD | - | 📝 Planned |

## Repository Structure

```
Chronicles-of-Destiny/
│
├── Book-1-Dance-of-Life-and-Death/    # BOOK 1 (COMPLETE)
│   ├── 01-Planning/                   # Plot outlines and blueprints
│   ├── 02-Chapters/                   # 15 completed chapters
│   ├── 03-Reference/                  # Summaries, critiques, character tracking
│   └── World Setting/                 # World state AT END of Book 1
│       ├── Characters/                # By role: Main, Supporting, Antagonists, Minor
│       ├── Locations/                 # Geography and places
│       └── Items/                     # Artifacts and weapons
│
├── Book-2-Birth-of-Fallen-Hero/       # BOOK 2 (PLANNED)
│   ├── 01-Planning/                   # Plot outline ready
│   ├── 02-Chapters/                   # (Empty - not yet written)
│   ├── 03-Reference/                  # (Create after writing)
│   └── World Setting/                 # (Create when writing - inherits from Book 1)
│
├── Book-3-Darkest-Light/              # BOOK 3 (PLANNED)
├── Book-4-TBD/                        # BOOK 4 (PLANNED)
│
├── Plot Setting/                      # Cross-book plot documentation
│
├── CLAUDE.md                          # AI writing assistant instructions
├── PROJECT-README.md                  # This file
├── README.md                          # Project summary
└── requirement.txt                    # Chapter generation requirements
```

## Key Organizational Principle

### Per-Book World Setting

Each book has its OWN `World Setting/` folder tracking the world state at that point:

- **Book 1 World Setting**: Characters, locations, items as of Book 1 END
- **Book 2 World Setting**: Inherits from Book 1, tracks new changes
- **Book 3 World Setting**: Inherits from Books 1-2

This allows proper tracking of:
- Character deaths (Elfiria dies Ch14, Aric dies Ch8)
- Status changes (Xylos captured Ch11)
- New locations (Deephollow established)
- World events (Holy Dome activation)

## Quick Start Guide

### For Reading
Navigate to `Book-1-Dance-of-Life-and-Death/02-Chapters/` and start with Chapter 1.

### For Writing New Chapters

1. **Choose Your Book** - Navigate to the book folder
2. **Check Planning** - Read `01-Planning/` files
3. **Reference World State** - Check PREVIOUS book's `World Setting/`
4. **Check Continuity** - Read previous book's `03-Reference/`
5. **Write Chapter** - Follow `requirement.txt` (5000+ words, light novel style)
6. **Save Chapter** - Place in book's `02-Chapters/` folder
7. **After Book Completion** - Create/update that book's `World Setting/`

## Key Files

| File | Purpose |
|------|---------|
| **CLAUDE.md** | AI writing assistant instructions |
| **requirement.txt** | Chapter generation requirements and style guide |
| **Book-X/01-Planning/** | Plot and chapter outlines |
| **Book-X/02-Chapters/** | Written chapters |
| **Book-X/03-Reference/** | Character status, summaries, critiques |
| **Book-X/World Setting/** | World state at end of that book |

## World of Mythosia

### Magic Systems
1. **Aether/Celestial** - Divine magic (Aasimar, priests)
2. **Elemental** - Nature-based magic (mages, various races)
3. **Shadow/Void** - Dark magic (demons, corrupted beings)

### Major Factions (End of Book 1)

| Faction | Status | Territory |
|---------|--------|-----------|
| Alliance of Light | 4 kingdoms protected | Within Holy Dome |
| The Exiled | ~1,500 fighters | Outer lands (Deephollow) |
| Demon Army | Demon King + Generals | All outer lands |

### Key Locations
- **Protected (Holy Dome)**: Aetheria, Eldoria, Sylvanaria, Drakoria
- **Fallen**: Kharaz'Mar, Luminara, Aridia
- **Resistance Base**: Deephollow

## Character Quick Reference (End of Book 1)

### Protagonists (The Trinity)
| Character | Status | Role |
|-----------|--------|------|
| Kaelen | ALIVE | Commander of The Exiled |
| Lyra | ALIVE | Second-in-Command |
| Drakon | ALIVE | Key Commander |

### Deceased Main Characters
- **Elfiria** - Died Chapter 14 (overuse of Holy Dome)
- **Aric** - Died Chapter 8 (fighting 5 Demon Generals)

### Demon Generals
| General | Title | Status |
|---------|-------|--------|
| Malakor | Herald of Despair | ACTIVE |
| Dravos | Herald of War | ACTIVE |
| Xylos | Herald of Pain | CAPTURED |
| Vex | Herald of Plague | WOUNDED |
| Noxia | Herald of Shadows | DECEASED |

## Writing Style

- **Format:** Light novel (5000+ words per chapter)
- **Tone:** Balanced action, politics, character development
- **Content:** Mature themes - combat, romance, moral dilemmas
- **Humor:** Witty dialogue and character banter
- **POV:** Multiple perspectives when appropriate
- **Setting:** Real-world fantasy (NO game mechanics/VR elements)

## Core Themes

- Sacrifice and moral complexity
- Love and relationships in war
- Found family and brotherhood
- Heroism vs. pragmatism
- Power and corruption
- Hope in darkness

---

*Private Novel Project - December 2024*
