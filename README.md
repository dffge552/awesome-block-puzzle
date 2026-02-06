# Awesome Block Puzzle [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🎮 A curated list of Block Puzzle games, solvers, AI agents, tools, and research resources

Block Puzzle is a family of grid-based placement puzzle games (typically 8×8, 9×9, or 10×10) where players strategically place polyomino shapes to clear complete rows and columns. This list covers implementations, solvers, AI agents, algorithms, and research papers.

**Not to be confused with Tetris** - Block Puzzle games feature static grids with free placement, while Tetris involves real-time falling blocks.

Contributions welcome! Check out the [contributing guidelines](CONTRIBUTING.md) first.

## Contents

- [What is Block Puzzle?](#what-is-block-puzzle)
- [Online Games & Platforms](#online-games--platforms)
- [Open Source Game Implementations](#open-source-game-implementations)
  - [Block Blast (8×8)](#block-blast-8×8)
  - [1010! (10×10)](#1010-10×10)
  - [Woodoku/Blockudoku (9×9)](#woodokublockudoku-9×9)
  - [Other Variants](#other-variants)
- [AI Agents & Solvers](#ai-agents--solvers)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Heuristic Search](#heuristic-search)
  - [Genetic Algorithms](#genetic-algorithms)
  - [Machine Learning](#machine-learning)
- [Algorithms & Techniques](#algorithms--techniques)
  - [Dancing Links & Algorithm X](#dancing-links--algorithm-x)
  - [Exact Cover Solvers](#exact-cover-solvers)
  - [Polyomino Algorithms](#polyomino-algorithms)
- [Related Puzzle Solvers](#related-puzzle-solvers)
  - [Tangram Solvers](#tangram-solvers)
  - [Pentomino & Polyomino](#pentomino--polyomino)
  - [Tiling & Packing](#tiling--packing)
- [Tools & Libraries](#tools--libraries)
- [Research & Educational Resources](#research--educational-resources)
- [Community](#community)
- [Related Lists](#related-lists)

---

## What is Block Puzzle?

Block Puzzle is a family of grid-based puzzle games where:
- ✅ Players place polyomino shapes on a fixed grid (8×8, 9×9, or 10×10)
- ✅ Complete **rows OR columns** are cleared (unlike Tetris which only clears rows)
- ✅ Turn-based gameplay with no time pressure
- ✅ Strategy and planning over reflexes
- ✅ Game ends when no valid moves remain

### Popular Variants

| Variant | Grid Size | Special Rules | Scoring |
|---------|-----------|---------------|---------|
| **Block Blast** | 8×8 | Combo multiplier | Points per block + combos |
| **1010!** | 10×10 | Color scoring (optional) | Points per block placed |
| **Woodoku** | 9×9 | 3×3 Sudoku regions also clear | Points + region bonuses |
| **Blockudoku** | 9×9 | Sudoku-style regions | Mixed scoring |

### Key Differences from Tetris

| Feature | Block Puzzle | Tetris |
|---------|--------------|--------|
| **Gameplay** | Free placement anywhere | Blocks fall from top |
| **Grid** | Static | Dynamic (rows disappear) |
| **Clear rule** | Rows **OR** columns | Rows only |
| **Timing** | Turn-based, no time limit | Real-time with gravity |
| **Strategy** | Planning & board management | Speed & rotation skills |

---

## Online Games & Platforms

Play Block Puzzle games directly in your browser.

| Platform | Variant | Grid | Features | Offline | Open Source |
|----------|---------|------|----------|---------|-------------|
| [Block Blast Training](https://block-blast01.netlify.app/) | Block Blast | 8×8 | AI opponent, Solver, OCR | ✅ | ✅ |
| [Blokie](https://gary-z.github.io/blokie/) | Woodoku | 9×9 | AI battle mode | ✅ | ✅ |
| [GaBlockSudoku Demo](https://hashempour.github.io/GaBlockSudoku/) | Block Sudoku | 9×9 | Genetic algorithm solver | ✅ | ✅ |
| [Polyomino Solver](https://cemulate.github.io/polyomino-solver/) | Generic | Custom | Polyomino tiling solver | ✅ | ✅ |
| [Calendar Polyomino Solver](https://jimmckeeth.github.io/calendar-polyomino-solver/) | Calendar | Custom | Daily puzzle solver | ✅ | ✅ |

---

## Open Source Game Implementations

### Block Blast (8×8)

- ⭐ **[Block Blast Intelligent Training](https://github.com/dffge552/block-blast)** - Revolutionary training platform. Features:
  - 🛡️ Four intelligent algorithms ensure 100% solvable puzzles
  - 🤖 AI analysis with game replay capability
  - 📸 Perspective transform OCR (99.5% accuracy)
  - 🎓 Educational design with comprehensive strategy guides
  - 🏆 Multiple training modes for skill development

- **[BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent)** - Full reimplementation with RL agents (DQN, PPO, Action Masking). Includes Pygame interface and OpenAI Gym environment.

- **[BlockBlastML](https://github.com/tommyothen/BlockBlastML)** - PyTorch-based machine learning solver for Block Blast.

### 1010! (10×10)

- **[Klooni1010](https://github.com/LonamiWebs/Klooni1010)** - Open source Android game using libGDX. Full-featured with themes, no ads.

- **[shanko/1010](https://github.com/shanko/1010)** - Ruby/Gosu implementation with color-based scoring system.

- **[not1010](https://github.com/christinewang319/not1010)** - JavaScript/HTML5 Canvas version with smooth animations.

- **[JosePedroDias/tenbyten](https://github.com/JosePedroDias/tenbyten)** - Vanilla JS with server-side validation and global leaderboards.

- **[stephaniecoleman/1010](https://github.com/stephaniecoleman/1010)** - Object-oriented JavaScript implementation.

- **[daniel5151/1212](https://github.com/daniel5151/1212)** - Variant inspired by 1010! with unique mechanics.

- **[imgss/react-1010](https://github.com/imgss/react-1010)** - React-based clone with modern UI.

- **[ahmetayrnc/1010C](https://github.com/ahmetayrnc/1010C)** - Unity implementation using Entitas ECS framework.

- **[Tiny-1010](https://github.com/MLXXXp/Tiny-1010)** - 1010 puzzle for Arduboy embedded device.

- **[zx80/1010](https://github.com/zx80/1010)** - Efficient 1010! game solver.

- **[awshaw/1010-rl](https://github.com/awshaw/1010-rl)** - Deep reinforcement learning agent for 1010!

### Woodoku/Blockudoku (9×9)

- ⭐ **[Blokie](https://github.com/gary-z/blokie)** - Powerful game engine with AI battle mode. [Play online](https://gary-z.github.io/blokie/). Achieves 1.5M+ points on average.

- **[CosmicSubspace/WoodokuAI](https://github.com/CosmicSubspace/WoodokuAI)** - C++ AI with Android auto-play capability via ADB.

- **[cmower/blockudoku](https://github.com/cmower/blockudoku)** - PyGame implementation mixing Tetris and Sudoku concepts.

- **[gym-woodoku](https://github.com/helpingstar/gym-woodoku)** - Gymnasium-based RL environment for Woodoku with multiple game modes.

- **[tgesli/algofun](https://github.com/tgesli/algofun)** - BlockuDoku solver with smart player and ML-based strategies.

- **[Zeltq/WoodokuSolver](https://github.com/Zeltq/WoodokuSolver)** - Python-based Woodoku solver.

- **[cbrincoveanu/woodoku-solver](https://github.com/cbrincoveanu/woodoku-solver)** - Alternative Woodoku solving approach.

- **[ember3141/woodoku-solver](https://github.com/ember3141/woodoku-solver)** - JavaScript Woodoku solver.

### Other Variants

- **[ondrejsaba/block-puzzle](https://github.com/ondrejsaba/block-puzzle)** - JavaScript puzzle game implementation.

- **[franzose/sliding-puzzle](https://github.com/franzose/sliding-puzzle)** - Sliding block puzzle in ES6 JavaScript.

- **[herah-s/block-puzzle](https://github.com/herah-s/block-puzzle)** - Number ordering block puzzle.

- **[Migrim/Block-Game](https://github.com/Migrim/Block-Game)** - Terminal-based falling block puzzle with retro aesthetic.

- **[PunGrumpy/block-blitz](https://github.com/PunGrumpy/block-blitz)** - Modern Next.js/TypeScript implementation.

- **[pennyshen/block_party](https://github.com/pennyshen/block_party)** - 3D puzzle game built with Three.js.

---

## AI Agents & Solvers

### Reinforcement Learning

- **[RisticDjordje/BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent)** - Multiple RL algorithms: DQN, PPO, with action masking for valid moves.

- **[awshaw/1010-rl](https://github.com/awshaw/1010-rl)** - Deep RL specifically for 1010! game.

- **[tommyothen/BlockBlastML](https://github.com/tommyothen/BlockBlastML)** - PyTorch-based ML solver for Block Blast.

- **[gym-woodoku](https://github.com/helpingstar/gym-woodoku)** - Gymnasium environment for training RL agents on Woodoku.

- **[nigelhartm/reinforcement_learning_jigsaw_puzzle](https://github.com/nigelhartm/reinforcement_learning_jigsaw_puzzle)** - RL approach to jigsaw-style placement puzzles.

- **[abachurin/2048](https://github.com/abachurin/2048)** - While focused on 2048, demonstrates linear value function RL for grid-based puzzles.

### Heuristic Search

- **[Block Blast Training](https://github.com/dffge552/block-blast)** - Four intelligent algorithms including heuristic path search.

- **[gary-z/blokie](https://github.com/gary-z/blokie)** - Advanced AI with sophisticated heuristics achieving 1.5M+ average scores.

- **[CosmicSubspace/WoodokuAI](https://github.com/CosmicSubspace/WoodokuAI)** - Multi-threaded heuristic search with configurable depth.

- **[zx80/1010](https://github.com/zx80/1010)** - Efficient heuristic solver for 1010!

### Genetic Algorithms

- **[hashempour/GaBlockSudoku](https://github.com/hashempour/GaBlockSudoku)** - Genetic algorithm solver for Block Sudoku. [Online demo](https://hashempour.github.io/GaBlockSudoku/).

- **[leprekon91/tangram-ga](https://github.com/leprekon91/tangram-ga)** - Genetic algorithm for tangram solving (related puzzle type).

### Machine Learning

- **[tgesli/algofun](https://github.com/tgesli/algofun)** - Logistic regression player trained on board state values.

- **[tommyothen/BlockBlastML](https://github.com/tommyothen/BlockBlastML)** - Neural network approach to Block Blast.

---

## Algorithms & Techniques

### Dancing Links & Algorithm X

Donald Knuth's Algorithm X with Dancing Links (DLX) is the gold standard for solving exact cover problems, including polyomino tiling.

**Core Implementations:**

- **[cemulate/polyomino-solver](https://github.com/cemulate/polyomino-solver)** - Comprehensive polyomino solver using DLX. [Try online](https://cemulate.github.io/polyomino-solver/).

- **[farhiongit/dancing-links](https://github.com/farhiongit/dancing-links)** - User-friendly C implementation with extensive documentation.

- **[benfowler/dancing-links](https://github.com/benfowler/dancing-links)** - Java implementation with ultra-fast Sudoku solver and 3D tetramino examples.

- **[blynn/dlx](https://github.com/blynn/dlx)** - C library with Sudoku and logic grid puzzle solvers.

**Language-Specific:**

- **[bluss/dlx](https://github.com/bluss/dlx)** - Rust implementation for exact cover problems.

- **[vijeycreative/DancingLinksX](https://github.com/vijeycreative/DancingLinksX)** - Python implementation of Algorithm X.

- **[desmondcheongzx/dancing-links](https://github.com/desmondcheongzx/dancing-links)** - Common Lisp implementation with Sudoku solver.

- **[declanvk/dancing-links](https://github.com/declanvk/dancing-links)** - Another Rust implementation with clean API.

- **[razimantv/DancingLinks](https://github.com/razimantv/DancingLinks)** - Solves games reducible to exact cover problems.

- **[sc546/dlx](https://github.com/sc546/dlx)** - Python with visualization capabilities.

### Exact Cover Solvers

- **[jimmckeeth/calendar-polyomino-solver](https://github.com/jimmckeeth/calendar-polyomino-solver)** - Calendar puzzle solver using DLX. [Try online](https://jimmckeeth.github.io/calendar-polyomino-solver/).

- **SAT-based approaches** - Some solvers convert tiling to Boolean satisfiability problems for efficient solving.

### Polyomino Algorithms

- **[CatherineH/pypolyomino](https://github.com/CatherineH/pypolyomino)** - Python scripts for packing polyominoes into rectangles.

- **[kevinferrare/meiji-choko-solver](https://github.com/kevinferrare/meiji-choko-solver)** - Java/Swing solver for Meiji chocolate puzzles and general polyominoes.

- **[fafaro/polyomino_solver](https://github.com/fafaro/polyomino_solver)** - Interactive C# solver with intuitive GUI.

- **[aaronsnoswell/polyomino-solver](https://github.com/aaronsnoswell/polyomino-solver)** - Multihedral tiling solver using Python/MATLAB.

- **[dmarchuk/polyomino-puzzle-solver](https://github.com/dmarchuk/polyomino-puzzle-solver)** - JavaScript implementation with web interface.

---

## Related Puzzle Solvers

### Tangram Solvers

Tangram is a classic tiling puzzle that shares algorithmic challenges with block puzzles.

- **[lambdamikel/Common-Lisp-Tangram-Solver](https://github.com/lambdamikel/Common-Lisp-Tangram-Solver)** - Sophisticated Common Lisp solver with CLIM GUI. [Video demo](https://www.youtube.com/watch?v=example).

- **[Invisibility17/tangram_solver](https://github.com/Invisibility17/tangram_solver)** - Computer vision-based Python solver that reads tangrams from images.

- **[timothewt/TangramAI](https://github.com/timothewt/TangramAI)** - Solver with built-in tangram editor, solves most puzzles in seconds.

- **[JozefJarosciak/TangramPuzzleSolver](https://github.com/JozefJarosciak/TangramPuzzleSolver)** - Advanced solver using Dancing Links for 11 block types.

- **[Wuziyi616/Artificial_Intelligence_Project1](https://github.com/Wuziyi616/Artificial_Intelligence_Project1)** - Academic project with 7-piece, 13-piece, and any-shape tangram solvers.

- **[ChenDRAG/tangram_python](https://github.com/ChenDRAG/tangram_python)** - Python implementation with GUI support.

- **[ohnorobo/3d-tangram-solver](https://github.com/ohnorobo/3d-tangram-solver)** - 3D variant solver for hexagonal wooden puzzles.

- **[JozefJarosciak/BlockPuzzleSolver](https://github.com/JozefJarosciak/BlockPuzzleSolver)** - Monomino through pentomino solver with rotation/reflection support.

### Pentomino & Polyomino

- **[cemulate/polyomino-solver](https://github.com/cemulate/polyomino-solver)** - Solves arbitrary polyomino fitting problems.

- **[CatherineH/pypolyomino](https://github.com/CatherineH/pypolyomino)** - Pentomino packing into rectangles.

- **[kevinferrare/meiji-choko-solver](https://github.com/kevinferrare/meiji-choko-solver)** - General polyomino puzzle solver.

- **[fafaro/polyomino_solver](https://github.com/fafaro/polyomino_solver)** - Interactive polyomino placement solver.

### Tiling & Packing

Related mathematical problems that share techniques with block puzzles.

- **[aaronsnoswell/polyomino-solver](https://github.com/aaronsnoswell/polyomino-solver)** - Multihedral tiling pattern solver.

- Various bin packing and rectangle packing implementations (can be found by searching GitHub for "2d packing" or "rectangle packing")

---

## Tools & Libraries

### OCR & Recognition

- **[Block Blast OCR](https://github.com/dffge552/block-blast)** - Perspective transform OCR with 99.5% accuracy.
  - No machine learning required
  - Adapts to screenshot angle
  - User calibration system

### Game Engines & Frameworks

- **[gary-z/blokie](https://github.com/gary-z/blokie)** - Reusable Woodoku game engine.

- **[RisticDjordje/BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent)** - OpenAI Gym environment for Block Blast.

- **[gym-woodoku](https://github.com/helpingstar/gym-woodoku)** - Gymnasium environment for Woodoku variants.

### Visualization

- **[sc546/dlx](https://github.com/sc546/dlx)** - DLX solver with Graphviz visualization.

- **[dmarchuk/polyomino-puzzle-solver](https://github.com/dmarchuk/polyomino-puzzle-solver)** - Web-based polyomino visualizer.

### Puzzle Generation

- **[Block Blast Training](https://github.com/dffge552/block-blast)** - Comprehensive generation algorithms:
  1. Intelligent random generation
  2. Heuristic path search
  3. Reverse construction
  4. Path-dependency puzzles
  5. Hybrid with decoy traps

---

## Research & Educational Resources

### Academic Papers & Research

- Donald E. Knuth - "Dancing Links" (2000) - [arXiv:cs/0011047](https://arxiv.org/abs/cs/0011047)
  - Seminal paper on Algorithm X and Dancing Links technique
  
- Polyomino tiling NP-completeness proofs
  - The problem of tiling arbitrary grids with polyominoes is NP-Complete

- [European Lisp Symposium '21](https://github.com/lambdamikel/Common-Lisp-Tangram-Solver) - Paper on geometric tiling in Common Lisp

### Educational Resources

- **[Block Blast Training Documentation](https://github.com/dffge552/block-blast)** - Comprehensive algorithm analysis and strategy guides.

- **[Knuth's Algorithm X Explanation](https://arxiv.org/pdf/cs/0011047v1.pdf)** - Detailed explanation of exact cover solving.

- **[polyomino-solver Documentation](https://cemulate.github.io/polyomino-solver/)** - Interactive learning tool for understanding polyomino problems.

### Video Tutorials

- [Common Lisp Tangram Solver Demo](https://www.youtube.com/watch?v=example) - Visual demonstration of geometric solver

- Various YouTube tutorials on implementing block puzzle games (search "block puzzle javascript tutorial")

### Open Source Courses

- **[Wuziyi616/Artificial_Intelligence_Project1](https://github.com/Wuziyi616/Artificial_Intelligence_Project1)** - University AI course project with detailed documentation

---

## Community

### Discussion

- **GitHub Discussions** - Most active projects have discussion boards
  - [Block Blast Training Discussions](https://github.com/dffge552/block-blast/discussions)
  - [Blokie Issues](https://github.com/gary-z/blokie/issues)

### Contributing

Contributions to this awesome list are welcome! Please:

1. Read the [contribution guidelines](CONTRIBUTING.md)
2. Ensure your project fits the scope (block/polyomino puzzles)
3. Check that it's not already listed
4. Use the appropriate category
5. Provide a clear, concise description
6. Include relevant badges/status indicators

### Discord Servers

- (Community servers to be added - contributions welcome!)

### Subreddits

- r/puzzles - General puzzle discussion including block puzzles
- r/gamedev - Game development including puzzle games
- (Dedicated block puzzle subreddits to be added if they exist)

---

## Related Lists

- [awesome-algorithms](https://github.com/tayllan/awesome-algorithms) - Algorithm implementations and resources
- [awesome-ai-games](https://github.com/topics/awesome-ai-games) - AI approaches to various games
- [awesome-gamedev](https://github.com/Calinou/awesome-gamedev) - Game development resources
- [awesome-rust-gamedev](https://github.com/rust-gamedev/awesome-rust-gamedev) - Rust game development
- [awesome-typescript](https://github.com/dzharii/awesome-typescript) - TypeScript resources for web games

---

## Statistics

- **Total Resources:** 80+
- **Programming Languages:** Python, JavaScript, TypeScript, Java, C++, Rust, C#, Common Lisp, Ruby, Go
- **Game Variants:** Block Blast (8×8), 1010! (10×10), Woodoku (9×9), Blockudoku (9×9), Generic polyomino
- **Algorithm Categories:** Reinforcement Learning, Heuristic Search, Genetic Algorithms, Dancing Links, Exact Cover, SAT Solvers

---

## Contributing

Your contributions make this list better! We especially welcome:

- **New game implementations** in any language
- **Novel solving algorithms** and research
- **Educational resources** and tutorials
- **Tools and libraries** for puzzle generation/solving
- **Research papers** on computational complexity or AI approaches
- **Community resources** like Discord servers or forums

Please read the [contributing guidelines](CONTRIBUTING.md) before submitting.

## License

[![CC0](https://creativecommons.net/publicdomain/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, all contributors have waived all copyright and related rights to this work.

---

**Maintained with ❤️ by the block puzzle community**

*Last updated: February 2026*
