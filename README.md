# Awesome Block Puzzle [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🎮 A curated list of Block Puzzle games, solvers, AI agents, and resources

Block Puzzle is a grid-based placement puzzle game (typically 8×8, 9×9, or 10×10) 
where players strategically place shapes to clear complete rows and columns.

**Not to be confused with Tetris** - Block Puzzle games feature static grids 
with free placement, while Tetris involves falling blocks.

Contributions welcome! Check out the [contributing guidelines](CONTRIBUTING.md).

## Contents
- [What is Block Puzzle?](#what-is-block-puzzle)
- [Online Games](#online-games)
- [Open Source Implementations](#open-source-implementations)
- [AI & Solvers](#ai--solvers)
- [Tools & Libraries](#tools--libraries)
- [Learning Resources](#learning-resources)
- [Research Papers](#research-papers)
- [Community](#community)

---

## What is Block Puzzle?

Block Puzzle is a family of grid-based puzzle games where:
- ✅ Players place shapes on a fixed grid (8×8, 9×9, or 10×10)
- ✅ Complete **rows OR columns** are cleared (unlike Tetris which only clears rows)
- ✅ Turn-based gameplay with no time pressure
- ✅ Strategy over reflexes

**Popular variants:**
- **Block Blast** (8×8) - Mobile game with combo system
- **1010!** (10×10) - Classic variant with color scoring
- **Woodoku/Blockudoku** (9×9) - Combines Sudoku 3×3 region rules

**Key differences from Tetris:**

| Feature | Block Puzzle | Tetris |
|---------|--------------|--------|
| Gameplay | Free placement | Falling blocks |
| Grid | Static | Dynamic |
| Clear rule | Rows **OR** columns | Rows only |
| Timing | Turn-based | Real-time |

---

## Online Games

Websites to play Block Puzzle games online.

| Website | Variant | AI opponent | Solver | Offline mode |
|---------|---------|-------------|--------|--------------|
| [Block Blast Training](https://block-blast01.netlify.app/) | Block Blast (8×8) | ✅ | ✅ | ✅ |
| ... | ... | ... | ... | ... |

---

## Open Source Implementations

### Block Blast Variants (8×8)

- ⭐ **[Block Blast Intelligent Training](https://github.com/dffge552/block-blast)** - Revolutionary training platform with 100% solvable puzzle generation. Features:
  - 🛡️ Four intelligent algorithms ensure every round is solvable
  - 🤖 AI analysis with game replay
  - 📸 Perspective transform OCR (99.5% accuracy)
  - 🎓 Educational design with strategy guides
  - 🏆 Multiple training modes

### 1010! Variants (10×10)

- [shanko/1010](https://github.com/shanko/1010) - Ruby/Gosu implementation with color-based scoring.
- [christinewang319/not1010](https://github.com/christinewang319/not1010) - JavaScript/HTML5 Canvas version.
- [JosePedroDias/tenbyten](https://github.com/JosePedroDias/tenbyten) - Vanilla JS with server validation.
- [LonamiWebs/Klooni1010](https://github.com/LonamiWebs/Klooni1010) - Open source Android game using libGDX.

### Woodoku/Blockudoku Variants (9×9)

- [gary-z/blokie](https://github.com/gary-z/blokie) - Game engine with AI battle mode. [Try it online](https://gary-z.github.io/blokie/).
- [Rustydoku](link-when-found) - Rust implementation playable in browser.

---

## AI & Solvers

### Reinforcement Learning Agents

- [awshaw/1010-rl](https://github.com/awshaw/1010-rl) - Deep RL for 1010! game.
- [RisticDjordje/BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent) - Multiple algorithms: DQN, PPO, Action Masking.
- [tommyothen/BlockBlastML](https://github.com/tommyothen/BlockBlastML) - PyTorch-based ML solver.

### Genetic Algorithms

- [hashempour/GaBlockSudoku](https://github.com/hashempour/GaBlockSudoku) - Genetic algorithm solver for Block Sudoku. [Online demo](https://hashempour.github.io/GaBlockSudoku/).

### Online Solver Services

- [gary-z/blokie AI](https://gary-z.github.io/blokie/) - Woodoku AI opponent.

---

## Tools & Libraries

### OCR & Recognition

- **[Block Blast OCR](https://github.com/dffge552/block-blast)** - Perspective transform OCR with 99.5% accuracy.
  - No machine learning required
  - Adapts to any screenshot angle
  - User calibration with reference points

### Puzzle Generation Algorithms

Resources on generating solvable puzzles:

- **Smart Generation Algorithms** (from Block Blast Training):
  1. Intelligent random generation
  2. Heuristic path search
  3. Reverse construction
  4. Path-dependency puzzles
  5. Hybrid with decoy traps

---

## Learning Resources

### Strategy Guides

- [Block Blast Training Docs](https://github.com/dffge552/block-blast) - Comprehensive algorithm analysis and educational guide.

### Video Tutorials

- (To be added - contributions welcome!)

### Articles

- (To be added - contributions welcome!)

---

## Research Papers

- (To be added - contributions welcome!)

Academic research on:
- Puzzle generation algorithms
- AI solving strategies
- Computational complexity analysis

---

## Community

### Discord Servers

- (To be added - contributions welcome!)

### Subreddits

- (To be added - contributions welcome!)

### Forums

- (To be added - contributions welcome!)

---

## Related Lists

- [awesome-xiangqi](https://github.com/ProgramFOX/awesome-xiangqi) - Chinese chess resources.
- (Not awesome-tetris - Tetris is a different game category)

---

## Contributing

Contributions welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
