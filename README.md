# Awesome Block Puzzle [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🎮 A curated list of Block Puzzle games, solvers, AI agents, tools, and research resources

## About

Block Puzzle represents a family of strategic grid-based placement games where players position polyomino shapes on fixed grids (8×8, 9×9, or 10×10) to clear complete rows and columns. Unlike real-time falling block games (Tetris), Block Puzzle emphasizes spatial planning, pattern recognition, and strategic thinking in a turn-based environment.

This list brings together the fragmented Block Puzzle ecosystem—spanning game implementations, AI solvers, algorithmic research, and development tools—into a single comprehensive resource. Whether you're building a game, researching algorithms, or training AI agents, you'll find high-quality resources organized by category.

**What makes this different from Tetris?** While Tetris features real-time falling blocks with row-only clearing, Block Puzzle games offer free placement anywhere on a static grid with both row AND column clearing. This fundamental difference creates unique algorithmic challenges and strategic depth.

**Contributions are welcome!** Help grow this collection by submitting PRs. See [contributing guidelines](CONTRIBUTING.md).

---

## Contents

- [About](#about)
- [Understanding Block Puzzle](#understanding-block-puzzle)
  - [Game Variants](#game-variants)
  - [Key Mechanics](#key-mechanics)
- [Online Platforms](#online-platforms)
- [Game Implementations](#game-implementations)
  - [Block Blast (8×8)](#block-blast-8×8)
  - [1010! (10×10)](#1010-10×10)
  - [Woodoku/Blockudoku (9×9)](#woodokublockudoku-9×9)
  - [Generic & Custom Variants](#generic--custom-variants)
- [AI & Solvers](#ai--solvers)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Heuristic Search](#heuristic-search)
  - [Genetic Algorithms](#genetic-algorithms)
  - [Machine Learning](#machine-learning)
- [Core Algorithms](#core-algorithms)
  - [Dancing Links & Algorithm X](#dancing-links--algorithm-x)
  - [Exact Cover Solvers](#exact-cover-solvers)
  - [Polyomino Packing](#polyomino-packing)
- [Related Puzzle Types](#related-puzzle-types)
  - [Tangram Solvers](#tangram-solvers)
  - [Pentomino & Polyomino](#pentomino--polyomino)
  - [3D Block Puzzles](#3d-block-puzzles)
- [Development Tools](#development-tools)
  - [Game Engines & Libraries](#game-engines--libraries)
  - [OCR & Computer Vision](#ocr--computer-vision)
  - [Puzzle Generators](#puzzle-generators)
  - [Visualization Tools](#visualization-tools)
- [Learning Resources](#learning-resources)
  - [Academic Papers](#academic-papers)
  - [Educational Projects](#educational-projects)
  - [Video Tutorials](#video-tutorials)
- [Community](#community)
- [Related Awesome Lists](#related-awesome-lists)

---

## Understanding Block Puzzle

### Game Variants

| Variant | Grid | Special Rules | Primary Challenge |
|---------|------|---------------|-------------------|
| **Block Blast** | 8×8 | Combo scoring multiplier | Maximizing consecutive clears |
| **1010!** | 10×10 | Color-based scoring (optional) | Efficient space utilization |
| **Woodoku** | 9×9 | 3×3 Sudoku regions also clear | Balancing rows/columns/regions |
| **Blockudoku** | 9×9 | Hybrid Sudoku mechanics | Multi-constraint optimization |

### Key Mechanics

**Core Gameplay:**
- 🎯 Place polyomino shapes anywhere on a fixed grid
- ✨ Complete rows OR columns are cleared (both count!)
- 🧠 Turn-based with no time pressure
- 🎮 Game ends when no valid placements remain

**Strategic Elements:**
- Planning multi-move sequences
- Corner and edge management
- Combo chain optimization
- Space efficiency vs. clearing opportunities

**Comparison with Tetris:**

| Feature | Block Puzzle | Tetris |
|---------|--------------|--------|
| **Placement** | Free positioning anywhere | Blocks fall from top only |
| **Grid** | Static board | Dynamic with row elimination |
| **Clearing** | Rows **OR** columns | Rows only |
| **Timing** | Turn-based, unlimited think time | Real-time with increasing speed |
| **Primary Skill** | Strategic planning & pattern recognition | Reflexes & rotation speed |

---

## Online Platforms

Play, train, or experiment with Block Puzzle games directly in your browser.

| Platform | Variant | Grid | Features | Offline | Source |
|----------|---------|------|----------|---------|--------|
| [Block Blast Training](https://block-blast01.netlify.app/) | Block Blast | 8×8 | AI opponent, Solver, OCR, Replay | ✅ | [GitHub](https://github.com/dffge552/block-blast) |
| [Blokie](https://gary-z.github.io/blokie/) | Woodoku | 9×9 | AI battle, 1.5M+ avg score | ✅ | [GitHub](https://github.com/gary-z/blokie) |
| [GaBlockSudoku](https://hashempour.github.io/GaBlockSudoku/) | Block Sudoku | 9×9 | Genetic algorithm demo | ✅ | [GitHub](https://github.com/hashempour/GaBlockSudoku) |
| [Polyomino Solver](https://cemulate.github.io/polyomino-solver/) | Generic | Custom | Universal polyomino tiling | ✅ | [GitHub](https://github.com/cemulate/polyomino-solver) |
| [Calendar Puzzle Solver](https://jimmckeeth.github.io/calendar-polyomino-solver/) | Calendar | Custom | Daily puzzle solver | ✅ | [GitHub](https://github.com/jimmckeeth/calendar-polyomino-solver) |

---

## Game Implementations

### Block Blast (8×8)

- ⭐ **[Block Blast Intelligent Training](https://github.com/dffge552/block-blast)** `Python` `JavaScript` - Revolutionary training platform featuring:
  - 🛡️ Four algorithms ensuring 100% solvable puzzles
  - 🤖 AI analysis with game replay
  - 📸 Perspective transform OCR (99.5% accuracy)
  - 🎓 Comprehensive strategy guides
  - 🏆 Multiple training modes

- **[BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent)** `Python` - Complete reimplementation with:
  - Deep Q-Network (DQN)
  - Proximal Policy Optimization (PPO)
  - Action masking for valid moves
  - Pygame interface
  - OpenAI Gym environment

- **[BlockBlastML](https://github.com/tommyothen/BlockBlastML)** `Python` - PyTorch-based ML solver with neural network approach.

### 1010! (10×10)

- **[Klooni1010](https://github.com/LonamiWebs/Klooni1010)** `Java` - Professional Android game using libGDX:
  - Multiple themes
  - No advertisements
  - Offline play
  - Open source

- **[1010-rl](https://github.com/awshaw/1010-rl)** `Python` - Deep reinforcement learning agent for 1010! with documented training process.

- **[shanko/1010](https://github.com/shanko/1010)** `Ruby` - Ruby/Gosu implementation with color-based scoring.

- **[not1010](https://github.com/christinewang319/not1010)** `JavaScript` - HTML5 Canvas version with smooth animations.

- **[tenbyten](https://github.com/JosePedroDias/tenbyten)** `JavaScript` - Vanilla JS with server validation and global leaderboards.

- **[stephaniecoleman/1010](https://github.com/stephaniecoleman/1010)** `JavaScript` - Object-oriented implementation demonstrating clean architecture.

- **[1212](https://github.com/daniel5151/1212)** `JavaScript` - Inspired by 1010! with unique mechanics variation.

- **[react-1010](https://github.com/imgss/react-1010)** `React` - Modern React-based clone with contemporary UI patterns.

- **[1010C](https://github.com/ahmetayrnc/1010C)** `C#` - Unity implementation using Entitas ECS framework for performance.

- **[Tiny-1010](https://github.com/MLXXXp/Tiny-1010)** `C++` - Embedded version for Arduboy handheld device.

- **[zx80/1010](https://github.com/zx80/1010)** `Python` - Efficient heuristic solver optimized for speed.

### Woodoku/Blockudoku (9×9)

- ⭐ **[Blokie](https://github.com/gary-z/blokie)** `JavaScript` - Advanced engine with AI achieving 1.5M+ average score. [Play online](https://gary-z.github.io/blokie/).

- **[WoodokuAI](https://github.com/CosmicSubspace/WoodokuAI)** `C++` - High-performance AI with:
  - Multi-threaded search
  - Android auto-play via ADB
  - Configurable search depth

- **[blockudoku](https://github.com/cmower/blockudoku)** `Python` - PyGame implementation mixing Tetris and Sudoku concepts.

- **[gym-woodoku](https://github.com/helpingstar/gym-woodoku)** `Python` - Gymnasium RL environment supporting:
  - Multiple game modes
  - Custom reward functions
  - Observation space variants

- **[algofun](https://github.com/tgesli/algofun)** `Python` - BlockuDoku solver with ML-based strategies and logistic regression player.

- **[WoodokuSolver](https://github.com/Zeltq/WoodokuSolver)** `Python` - Clean Python solver implementation.

- **[woodoku-solver](https://github.com/cbrincoveanu/woodoku-solver)** `Python` - Alternative solving approach with detailed documentation.

- **[ember3141/woodoku-solver](https://github.com/ember3141/woodoku-solver)** `JavaScript` - Browser-based solver with interactive interface.

### Generic & Custom Variants

- **[block-puzzle-solver](https://github.com/samabcde/block-puzzle-solver)** `Java` - Generic solver supporting arbitrary grid sizes and block shapes with optimization focus.

- **[block-puzzle-solver](https://github.com/stevenlanders/block-puzzle-solver)** `Java` - RESTful API for puzzle generation and solving with web interface.

- **[block-puzzle](https://github.com/ondrejsaba/block-puzzle)** `JavaScript` - Customizable JavaScript implementation.

- **[sliding-puzzle](https://github.com/franzose/sliding-puzzle)** `JavaScript` - ES6 sliding block puzzle with modern syntax.

- **[block-puzzle](https://github.com/herah-s/block-puzzle)** `JavaScript` - Number ordering variant.

- **[Block-Game](https://github.com/Migrim/Block-Game)** `Python` - Terminal-based falling block puzzle with retro ASCII aesthetic.

- **[block-blitz](https://github.com/PunGrumpy/block-blitz)** `TypeScript` - Modern Next.js implementation with TypeScript.

- **[block_party](https://github.com/pennyshen/block_party)** `JavaScript` - 3D puzzle game built with Three.js.

---

## AI & Solvers

### Reinforcement Learning

- **[BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent)** `Python` - Multiple RL algorithms (DQN, PPO) with action masking.

- **[1010-rl](https://github.com/awshaw/1010-rl)** `Python` - Deep RL specifically for 1010! game optimization.

- **[BlockBlastML](https://github.com/tommyothen/BlockBlastML)** `Python` - PyTorch neural network approach.

- **[gym-woodoku](https://github.com/helpingstar/gym-woodoku)** `Python` - Gymnasium environment enabling RL research on Woodoku.

- **[reinforcement_learning_jigsaw_puzzle](https://github.com/nigelhartm/reinforcement_learning_jigsaw_puzzle)** `Python` - RL approach to jigsaw-style placement puzzles.

### Heuristic Search

- **[Block Blast Training](https://github.com/dffge552/block-blast)** `Python` - Four intelligent algorithms including heuristic path search.

- **[Blokie](https://github.com/gary-z/blokie)** `JavaScript` - Sophisticated heuristics achieving professional-level scores.

- **[WoodokuAI](https://github.com/CosmicSubspace/WoodokuAI)** `C++` - Multi-threaded search with configurable depth.

- **[zx80/1010](https://github.com/zx80/1010)** `Python` - Optimized heuristic solver for 1010!

### Genetic Algorithms

- **[GaBlockSudoku](https://github.com/hashempour/GaBlockSudoku)** `JavaScript` - Genetic algorithm for Block Sudoku with [live demo](https://hashempour.github.io/GaBlockSudoku/).

- **[tangram-ga](https://github.com/leprekon91/tangram-ga)** `Python` - Genetic algorithm for tangram (related puzzle category).

### Machine Learning

- **[algofun](https://github.com/tgesli/algofun)** `Python` - Logistic regression player trained on board state evaluations.

- **[BlockBlastML](https://github.com/tommyothen/BlockBlastML)** `Python` - Neural network approach with training pipeline.

---

## Core Algorithms

### Dancing Links & Algorithm X

Donald Knuth's Algorithm X with Dancing Links (DLX) represents the gold standard for exact cover problems, including polyomino tiling.

**Foundational Implementations:**

- ⭐ **[cemulate/polyomino-solver](https://github.com/cemulate/polyomino-solver)** `JavaScript` - Comprehensive solver with [interactive web interface](https://cemulate.github.io/polyomino-solver/).

- **[farhiongit/dancing-links](https://github.com/farhiongit/dancing-links)** `C` - User-friendly C implementation with extensive documentation and examples.

- **[benfowler/dancing-links](https://github.com/benfowler/dancing-links)** `Java` - High-performance Java version with:
  - Ultra-fast Sudoku solver
  - 3D tetramino examples
  - Benchmarking suite

- **[blynn/dlx](https://github.com/blynn/dlx)** `C` - C library featuring Sudoku and logic grid puzzle solvers.

**Language-Specific Implementations:**

- **[bluss/dlx](https://github.com/bluss/dlx)** `Rust` - Idiomatic Rust implementation leveraging type safety.

- **[DancingLinksX](https://github.com/vijeycreative/DancingLinksX)** `Python` - Python 3 implementation with clear documentation.

- **[desmondcheongzx/dancing-links](https://github.com/desmondcheongzx/dancing-links)** `Common Lisp` - Lisp implementation with Sudoku solver demonstration.

- **[declanvk/dancing-links](https://github.com/declanvk/dancing-links)** `Rust` - Alternative Rust version with clean API design.

- **[razimantv/DancingLinks](https://github.com/razimantv/DancingLinks)** `C++` - Solves games reducible to exact cover problems.

- **[sc546/dlx](https://github.com/sc546/dlx)** `Python` - Implementation with Graphviz visualization capabilities.

### Exact Cover Solvers

- **[calendar-polyomino-solver](https://github.com/jimmckeeth/calendar-polyomino-solver)** `JavaScript` - Calendar puzzle solver using DLX. [Interactive demo](https://jimmckeeth.github.io/calendar-polyomino-solver/).

- **SAT-based approaches** - Convert tiling problems to Boolean satisfiability for alternative solving strategies.

### Polyomino Packing

- **[pypolyomino](https://github.com/CatherineH/pypolyomino)** `Python` - Scripts for packing polyominoes into rectangular regions.

- **[meiji-choko-solver](https://github.com/kevinferrare/meiji-choko-solver)** `Java` - Solver for Meiji chocolate puzzles and general polyomino problems with GUI.

- **[fafaro/polyomino_solver](https://github.com/fafaro/polyomino_solver)** `C#` - Interactive solver with intuitive graphical interface.

- **[aaronsnoswell/polyomino-solver](https://github.com/aaronsnoswell/polyomino-solver)** `Python/MATLAB` - Multihedral tiling solver for complex patterns.

- **[polyomino-puzzle-solver](https://github.com/dmarchuk/polyomino-puzzle-solver)** `JavaScript` - Web-based solver with visual editor.

---

## Related Puzzle Types

### Tangram Solvers

Tangram puzzles share algorithmic challenges with block placement games.

- **[Common-Lisp-Tangram-Solver](https://github.com/lambdamikel/Common-Lisp-Tangram-Solver)** `Common Lisp` - Sophisticated solver with CLIM GUI. Featured in European Lisp Symposium '21.

- **[tangram_solver](https://github.com/Invisibility17/tangram_solver)** `Python` - Computer vision-based solver reading tangrams from images.

- **[TangramAI](https://github.com/timothewt/TangramAI)** `Python` - Complete solution with built-in editor, solves most puzzles in seconds.

- **[TangramPuzzleSolver](https://github.com/JozefJarosciak/TangramPuzzleSolver)** `JavaScript` - Advanced solver using Dancing Links for 11 block types. [Online tool](https://www.tetrissolver.com/).

- **[Artificial_Intelligence_Project1](https://github.com/Wuziyi616/Artificial_Intelligence_Project1)** `Python` - Academic project with 7-piece, 13-piece, and any-shape tangram solvers.

- **[tangram_python](https://github.com/ChenDRAG/tangram_python)** `Python` - Clean implementation with GUI support.

- **[3d-tangram-solver](https://github.com/ohnorobo/3d-tangram-solver)** `Python` - 3D variant solver for hexagonal wooden puzzles.

- **[BlockPuzzleSolver](https://github.com/JozefJarosciak/BlockPuzzleSolver)** `JavaScript` - Monomino through pentomino solver with rotation/reflection support.

### Pentomino & Polyomino

- **[polyomino-solver](https://github.com/cemulate/polyomino-solver)** `JavaScript` - Universal polyomino fitting problem solver.

- **[pypolyomino](https://github.com/CatherineH/pypolyomino)** `Python` - Pentomino rectangle packing algorithms.

- **[meiji-choko-solver](https://github.com/kevinferrare/meiji-choko-solver)** `Java` - General polyomino puzzle framework.

- **[polyomino_solver](https://github.com/fafaro/polyomino_solver)** `C#` - Interactive placement and solution visualization.

### 3D Block Puzzles

- **[block-puzzle-solver](https://github.com/fmoessbauer/block-puzzle-solver)** `C++` - Solves 5×5×5 and 6×6×6 cube puzzles in under one second using minimal-vertex-cover approach.

- **[3d-tangram-solver](https://github.com/ohnorobo/3d-tangram-solver)** `Python` - Hexagonal 3D wooden puzzle solver.

---

## Development Tools

### Game Engines & Libraries

- **[Blokie](https://github.com/gary-z/blokie)** `JavaScript` - Reusable Woodoku game engine with clean API.

- **[BlockBlast-Game-AI-Agent](https://github.com/RisticDjordje/BlockBlast-Game-AI-Agent)** `Python` - OpenAI Gym environment for Block Blast research.

- **[gym-woodoku](https://github.com/helpingstar/gym-woodoku)** `Python` - Gymnasium environment with multiple game modes.

- **libGDX** - Used by Klooni1010 for cross-platform game development.

### OCR & Computer Vision

- **[Block Blast OCR](https://github.com/dffge552/block-blast)** `Python` - Perspective transform OCR achieving 99.5% accuracy:
  - No machine learning dependencies
  - Adaptive to screenshot angles
  - User calibration system

- **[tangram_solver](https://github.com/Invisibility17/tangram_solver)** `Python` - Computer vision pipeline for tangram recognition.

### Puzzle Generators

- **[Block Blast Training](https://github.com/dffge552/block-blast)** `Python` - Five sophisticated generation algorithms:
  1. Intelligent random generation
  2. Heuristic path search
  3. Reverse construction
  4. Path-dependency puzzles
  5. Hybrid with decoy traps

- **[block-puzzle-solver](https://github.com/stevenlanders/block-puzzle-solver)** `Java` - RESTful API for puzzle generation.

### Visualization Tools

- **[sc546/dlx](https://github.com/sc546/dlx)** `Python` - DLX solver with Graphviz visualization of search tree.

- **[polyomino-puzzle-solver](https://github.com/dmarchuk/polyomino-puzzle-solver)** `JavaScript` - Web-based interactive visualizer.

- **[block-puzzle-solver](https://github.com/fmoessbauer/block-puzzle-solver)** `C++` - 3D visualization using point clouds and layer printing.

---

## Learning Resources

### Academic Papers

- **Donald E. Knuth** - ["Dancing Links"](https://arxiv.org/abs/cs/0011047) (2000) - Seminal paper introducing Algorithm X and the Dancing Links technique.

- **Polyomino Tiling Complexity** - The problem of tiling arbitrary grids with polyominoes is NP-Complete.

- **European Lisp Symposium '21** - [Paper on geometric tiling](https://github.com/lambdamikel/Common-Lisp-Tangram-Solver) in Common Lisp with constraint solving.

### Educational Projects

- **[Block Blast Training Documentation](https://github.com/dffge552/block-blast)** - Comprehensive algorithm analysis and strategy guides.

- **[Knuth's Algorithm X Explanation](https://arxiv.org/pdf/cs/0011047v1.pdf)** - Detailed mathematical foundation of exact cover solving.

- **[polyomino-solver](https://cemulate.github.io/polyomino-solver/)** - Interactive learning tool demonstrating polyomino algorithms.

- **[Artificial_Intelligence_Project1](https://github.com/Wuziyi616/Artificial_Intelligence_Project1)** `Python` - University AI course project with detailed educational documentation.

### Video Tutorials

- Various YouTube tutorials on block puzzle implementation (search "block puzzle javascript tutorial", "1010 game development")

- Block Blast strategy guides and gameplay optimization

---

## Community

### Discussion & Contribution

- **GitHub Discussions** - Most active projects host discussion boards:
  - [Block Blast Training Discussions](https://github.com/dffge552/block-blast/discussions)
  - [Blokie Issues](https://github.com/gary-z/blokie/issues)

### How to Contribute

This awesome list thrives on community contributions! We especially welcome:

✅ **New game implementations** in any programming language  
✅ **Novel solving algorithms** and research  
✅ **Educational resources** and tutorials  
✅ **Tools and libraries** for puzzle generation/solving  
✅ **Research papers** on complexity or AI approaches  
✅ **Community resources** (Discord servers, forums, subreddits)

**Before contributing:**
1. Read the [contribution guidelines](CONTRIBUTING.md)
2. Ensure your project fits the scope (block/polyomino placement puzzles)
3. Verify it's not already listed
4. Choose the appropriate category
5. Write a clear, concise description
6. Test all links

### Communication Channels

- **Reddit**:
  - r/puzzles - General puzzle discussion including block puzzles
  - r/gamedev - Game development including puzzle games

- **Discord Servers** - Community servers welcome! (Submit via PR)

- **GitHub Issues** - Use this repo's issue tracker for suggestions or questions

---

## Related Awesome Lists

- [awesome-algorithms](https://github.com/tayllan/awesome-algorithms) - Algorithm implementations and resources
- [awesome-gamedev](https://github.com/Calinou/awesome-gamedev) - Comprehensive game development resources
- [awesome-rust-gamedev](https://github.com/rust-gamedev/awesome-rust-gamedev) - Rust game development ecosystem
- [awesome-typescript](https://github.com/dzharii/awesome-typescript) - TypeScript resources for web development
- [awesome-cpp](https://github.com/fffaraz/awesome-cpp) - C++ libraries and frameworks

---

## Project Statistics

📊 **Current Status** (February 2026):
- **Total Resources:** 90+
- **Categories:** 15
- **Programming Languages:** Python, JavaScript, TypeScript, Java, C++, Rust, C#, Common Lisp, Ruby, Go
- **Game Variants Covered:** Block Blast (8×8), 1010! (10×10), Woodoku (9×9), Blockudoku (9×9), Generic/Custom
- **Algorithm Types:** Reinforcement Learning, Heuristic Search, Genetic Algorithms, Dancing Links, Exact Cover, SAT Solvers

---

## License

[![CC0](https://licensebuttons.net/publicdomain/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, all contributors have waived all copyright and related rights to this work.

---

**Maintained with ❤️ by the block puzzle community**

*Last updated: February 2026 · [Submit corrections or additions](https://github.com/YOUR_USERNAME/awesome-block-puzzle/issues)*
