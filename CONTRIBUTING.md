# Contribution Guidelines

Thank you for considering contributing to Awesome Block Puzzle! This list aims to be a comprehensive resource for grid-based placement puzzle games, solvers, and research.

Please ensure your pull request adheres to the following guidelines.

## Adding to this list

* **Search first**: Check previous suggestions and existing entries to avoid duplicates.
* **One item per PR**: Make an individual pull request for each suggestion.
* **Follow the format**: Use `[Project Name](link) - Description.`
* **Clear descriptions**: Should be concise, informative, and end with a period.
* **Multiple items**: If adding 3+ related items, you may group them in one PR (e.g., "Add 5 Dancing Links implementations").
* **Categories**: New categories or improvements to existing categorization are welcome.
* **Quality**: Check spelling, grammar, and remove trailing whitespace.

## Quality Standards

Your suggestion should meet these criteria:

### ✅ Relevance

Must be related to **grid-based placement puzzles** with row/column elimination:

- **Games**: Block Blast (8×8), 1010! (10×10), Woodoku/Blockudoku (9×9), or similar variants
- **Algorithms**: Polyomino tiling, exact cover problems (Algorithm X, Dancing Links)
- **AI/Solvers**: Agents, heuristics, or optimization for these puzzle types
- **Tools**: Game engines, OCR, visualization, or generation tools
- **Research**: Academic papers, datasets, benchmarks related to these puzzles

### ✅ Quality Criteria

- **Working**: All links must be functional and point to legitimate resources
- **Documented**: Projects should have README or clear documentation
- **Maintained OR Significant**: Either actively maintained OR has historical/educational value
- **Open Source**: Preference for open source projects (exceptions for exceptional closed-source tools)
- **Description**: Must explain what makes it awesome/useful

### ❌ Not Accepted

- **Tetris variants** - Falling block games belong in [Awesome Tetris](https://github.com/search?q=awesome-tetris) (different game mechanics)
- **2048 and variants** - Sliding tile games (different puzzle category)
- **Match-3 games** - Candy Crush style (not placement puzzles)
- **Unrelated puzzles** - Jigsaw, crossword, etc.
- **Commercial apps without source** - Unless they're exceptional online platforms
- **Abandoned projects** - Must work or have educational value

## Project Categories

### Acceptable Submissions

| Category | Examples |
|----------|----------|
| **Games** | Block Blast, 1010!, Woodoku implementations |
| **AI Agents** | RL agents (DQN, PPO), heuristic solvers |
| **Algorithms** | Dancing Links, exact cover, polyomino tiling |
| **Solvers** | Genetic algorithms, search algorithms |
| **Tools** | Game engines, OCR tools, visualizers |
| **Libraries** | Reusable code for puzzle generation/solving |
| **Research** | Papers, datasets, academic implementations |
| **Educational** | Tutorials, courses, strategy guides |

### Borderline Cases (Discuss First)

- **Related puzzles**: Tangram, Pentomino (currently accepted as "Related Solvers")
- **3D variants**: Polycube puzzles (discuss if relevant)
- **New categories**: Open an issue to discuss before submitting

## Pull Request Process

1. **Fork** the repository
2. **Add your link** in the appropriate category (alphabetically if applicable)
3. **Test the link** - Ensure it works and points to the correct resource
4. **Format check**: 
   ```bash
   npx awesome-lint
   ```
5. **Commit** with a clear message:
   - Good: `Add BlockBlast-Solver - RL agent using PPO`
   - Okay: `Add BlockBlast-Solver`
   - Bad: `Update README.md`
6. **Create PR** with descriptive title:
   - Good: `Add BlockBlast-Solver (RL agent)`
   - Okay: `Add new AI solver`
   - Bad: `Update`

## Description Guidelines

### Good Descriptions ✅

- **Specific**: "PyTorch-based RL agent achieving 1M+ average score"
- **Features**: "React implementation with themes, no ads, offline support"
- **Technical**: "Dancing Links solver with visualization and 10+ language implementations"

### Bad Descriptions ❌

- **Too vague**: "A game" (what makes it special?)
- **Marketing**: "The best solver ever made!" (be objective)
- **Too long**: Should fit in 1-2 lines

## Updating Your PR

If maintainers request changes:

1. **Don't open a new PR** - Just edit the existing one
2. **Push to the same branch** - Changes will appear automatically
3. **Reply to feedback** - Let maintainers know you've updated

[Guide on updating PRs](https://github.com/RichardLitt/knowledge/blob/master/github/amending-a-commit-guide.md)

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).

By participating, you agree to:
- Be respectful and inclusive
- Accept constructive criticism gracefully
- Focus on what's best for the community

## Questions?

- **Not sure if it fits?** Open an issue to discuss before submitting
- **Need help?** Check existing PRs or ask in discussions
- **Found a broken link?** Please report it or submit a fix

## Recognition

Contributors will be recognized in:
- GitHub's automatic contributor list
- Special thanks for significant contributions

---

**Thank you for helping make this list awesome!** 🎮

*Every contribution, big or small, makes this resource better for the community.*
