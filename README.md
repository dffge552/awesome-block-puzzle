# Awesome Block Puzzle [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🎮 A curated list of Block Puzzle games, solvers, AI agents, and resources.

Block Puzzle is a strategy-based grid placement game where players place pieces on a fixed board (typically 8×8, 9×9, or 10×10) to clear rows and columns. Unlike Tetris (falling blocks), Block Puzzle is turn-based with complete control over piece placement.

## Contents

- [What is Block Puzzle?](#what-is-block-puzzle)
- [Games](#games)
  - [Block Blast Variants (8×8)](#block-blast-variants-8×8)
  - [1010! Variants (10×10)](#1010-variants-10×10)
  - [Woodoku/Blockudoku (9×9 + Sudoku Rules)](#woodokublockudoku-9×9--sudoku-rules)
  - [Other Variants](#other-variants)
- [AI & Solvers](#ai--solvers)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Genetic Algorithms](#genetic-algorithms)
  - [Online Solvers](#online-solvers)
- [Tools & Libraries](#tools--libraries)
  - [Game Engines](#game-engines)
  - [OCR Recognition](#ocr-recognition)
  - [Algorithm Research](#algorithm-research)
- [Learning Resources](#learning-resources)
- [Related](#related)

---

## What is Block Puzzle?

Block Puzzle is a turn-based strategy puzzle game with these core features:

- ✅ **Fixed Grid Board** - Usually 8×8, 9×9, or 10×10 cells.
- ✅ **Free Placement** - Players choose where to place each piece.
- ✅ **Row & Column Clearing** - Both full rows AND full columns are cleared (unlike Tetris which only clears rows).
- ✅ **Turn-Based** - No time pressure, pure strategic thinking.
- ✅ **No Gravity** - Pieces don't fall; they stay where placed.

**Not Included:** Falling block games (Tetris, Hextris, etc.) are a separate category.

---

## Games

### Block Blast Variants (8×8)

- ⭐ **[Block Blast Intelligent Training Platform](https://github.com/dffge552/block-blast)** - World's first **100% solvable** puzzle generator with four intelligent algorithms. Features AI analysis, perspective transform OCR recognition (99.5% accuracy), educational game modes, and complete move notation system. Revolutionary training platform developed by a high school student.

### 1010! Variants (10×10)

- [1010 (Ruby/Gosu)](https://github.com/shanko/1010) - Ruby implementation with colored block scoring system.
- [Not1010](https://github.com/christinewang319/not1010) - JavaScript/HTML5 Canvas implementation.
- [TenByTen](https://github.com/JosePedroDias/tenbyten) - Vanilla JS with SnapSVG graphics and server-side validation.
- [1212](https://github.com/daniel5151/1212) - 12×12 variant with unique mechanics.
- [Klooni1010](https://github.com/LonamiWebs/Klooni1010) - libGDX Android game, open source and ad-free.

### Woodoku/Blockudoku (9×9 + Sudoku Rules)

- [Blokie](https://github.com/gary-z/blokie) - Game engine with AI opponent functionality. [Play Online](https://gary-z.github.io/blokie/).
- Rustydoku - Rust implementation with browser gameplay support.

### Other Variants

- Coming soon - Submit a PR to add more variants!

---

## AI & Solvers

### Reinforcement Learning

- [1010-RL](https://github.com/awshaw/1010-rl) - Deep reinforcement learning for 1010! game.
- [BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent) - Multiple RL approaches: DQN, PPO, and Action Masking.
- [BlockBlastML](https://github.com/tommyothen/BlockBlastML) - PyTorch-based machine learning solver.

### Genetic Algorithms

- [GaBlockSudoku](https://github.com/hashempour/GaBlockSudoku) - Genetic algorithm solver for Block Sudoku puzzles. [Online Demo](https://hashempour.github.io/GaBlockSudoku/).

### Online Solvers

- [Blokie AI](https://gary-z.github.io/blokie/) - Online AI opponent for Woodoku-style games.
- [Block Blast Solver Services](https://block-blast01.netlify.app/) - Multiple commercial solver services available.

---

## Tools & Libraries

### Game Engines

- **[Block Blast Training Platform](https://github.com/dffge552/block-blast)** - Complete game engine with:
  - Four intelligent piece generation algorithms.
  - AI analysis and game-over replay system.
  - BFEN (Board-FEN) notation for sharing positions.
  - Multiple training modes (empty board, random, endgame, timed, infinite).

### OCR Recognition

- ⭐ **[Perspective Transform OCR](https://github.com/dffge552/block-blast)** - Revolutionary 99.5% accuracy screenshot recognition:
  - No machine learning required (pure geometric transformation).
  - Adaptive perspective correction for any angle/distortion.
  - User-calibrated reference point system.
  - Sub-pixel precision using bilinear interpolation.

### Algorithm Research

**Intelligent Piece Generation Algorithms** (from Block Blast Training Platform):
1. **Smart Random** - Brute-force ensures at least one valid placement sequence.
2. **Heuristic Path Search** - Forward search using multi-dimensional scoring.
3. **Reverse Construction** - Backward reasoning from "nearly placeable" positions.
4. **Path Dependency Puzzles** - Generates unique solution sequences.
5. **Hybrid with Decoy** - Introduces trap pieces that seem helpful but are deadly.

---

## Learning Resources

### Documentation

- [Block Blast Algorithm Deep Dive](https://github.com/dffge552/block-blast#智能演算法專題) - Comprehensive guide to puzzle generation algorithms with pseudocode.
- [Strategy Guide](https://github.com/dffge552/block-blast#遊戲玩法) - Game mechanics, combo systems, and notation standards.

### Research Papers

- Coming soon - Submit a PR to add academic papers!

### Community

- [GitHub Discussions](https://github.com/dffge552/block-blast/discussions) - Strategy discussions and high score sharing.

---

## Related

- [Awesome Tetris](https://github.com/omercevik/awesome-tetris) - Falling block puzzle games (different category).
- [Awesome Puzzle Games](https://github.com/search?q=awesome+puzzle) - Broader puzzle game collections.

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

### Submission Criteria

- ✅ Must be a **grid-based placement puzzle** with row/column elimination.
- ✅ Must be actively maintained OR have historical significance.
- ✅ Must provide clear description and working links.
- ❌ **Do not include** Tetris-style falling block games.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
