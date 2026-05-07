# HTML Apps

A workspace for standalone HTML5 applications. Each app is fully self-contained — no build tools, no bundlers, no `npm install`. Open the `index.html` in any modern browser and it just works.

Built with [Claude Code](https://claude.com/claude-code) as a reference for what an LLM-assisted single-file app workflow can look like.

## Apps in this repo

### Game guides

#### [`exiles-of-khorne/`](./exiles-of-khorne/) — Exiles of Khorne: New Player's Guide
A beginner-friendly guide to Skarbrand the Exiled and the Khornate horde faction in Total War: Warhammer III. Covers lore, Khorne and Exiles-specific mechanics, full unit roster, campaign and battle strategy, settlement decisions, diplomacy, economy, and tech priorities. Includes a sibling `titlecard.html` that renders a 1200×630 Open Graph share image.

#### [`ursun-revivalists/`](./ursun-revivalists/) — Ursun Revivalists: New Player's Guide
A new player's guide to Boris Ursus and his Kislev faction in Total War: Warhammer III. Covers Boris's awakening from the ice, Kislev mechanics (Devotion, Motherland Rituals, Atamans, Supporters), Ursun Revivalists faction effects, hero management, the War Bear Riders doomstack template, and both Immortal Empires opening paths.

#### [`masters-of-innovation/`](./masters-of-innovation/) — Masters of Innovation: New Player's Guide
A new player's guide to Malakai Makaisson and the Dwarf engineering faction in Total War: Warhammer III. Covers The Forge / Grudges / Underway, Malakai's Adventures, the Spirit of Grungni airship buildings, Gotrek & Felix as starting heroes, the artillery / flying-war-machine doomstack template, and the Kraka Drak surrounded-start campaign plan.

#### [`sm2-loadout/`](./sm2-loadout/) — Astartes Loadout Cogitator
A quick-reference loadout planner for [Warhammer 40,000: Space Marine 2](https://spacemarine2.fandom.com/) Operations co-op. All 12 missions across Avarax, Demerium, Kadaku, Agathon, and Orbit; all 7 classes; loadout suggestions adapt to mission faction (Tyranid / Chaos / Mixed) and difficulty (Minimal → Absolute); weapons color-coded by rarity tier; per-class role descriptions; team-composition synergy notes; hazard intel and mission rewards. Keyboard navigation: `←`/`→` cycles missions, `↑`/`↓` changes difficulty.

#### [`fs25-guide/`](./fs25-guide/) — FS25 Field Guide
A field-side reference for Farming Simulator 25 — crop rotations, equipment costs, and other practical look-ups for an active save.

#### [`shogun2-aup-encyclopedia/`](./shogun2-aup-encyclopedia/) — Shogun 2 AUP Encyclopedia (preview)
A standalone, locally-browsable encyclopedia of units, buildings, and technologies for the Shogun 2 AUP mod. Generated from JSON data via the included `generate.py`.

### Reference & planning tools

#### [`pocket-guide/`](./pocket-guide/) — Toolbox for Digital Artists
A tabbed pocket reference for digital artists — colour theory, composition, lighting, anatomy, software shortcuts, and other quick look-ups. Tab order is kept alphabetical when adding or renaming sections.

#### [`environmental-art-flowchart/`](./environmental-art-flowchart/) — Tropical Environment Art Project Flowchart
A planning visualisation for a tropical-environment 3D-art project — production stages, dependencies, and milestones laid out as a navigable flowchart.

#### [`regime-change-analysis/`](./regime-change-analysis/) — Rendszerváltás Reconsidered
A side-by-side comparative reading of five Hungarian essays on the post-1989 regime change. Long-form scholarly layout with both light and dark themes. (Filename: `regime_change_analysis.html`.)

## Project conventions

See [`CLAUDE.md`](./CLAUDE.md) for the full project rules. The short version:

- Every app is a valid HTML5 document (`<!DOCTYPE html>`)
- Each app lives in its own subdirectory
- No build step — the file you open is the file that runs
- Vanilla HTML/CSS/JS unless a library is genuinely needed
- External libraries via CDN only (no `npm`, no bundlers)

## Claude Code agents

The [`.claude/agents/`](./.claude/agents/) directory contains four specialized agent personas pulled from the [official Anthropic claude-code repo](https://github.com/anthropics/claude-code) for use when developing apps in this workspace:

- **code-architect** — designs feature architectures before implementation
- **code-explorer** — analyzes existing code structure and patterns
- **code-reviewer** — reviews code quality and convention compliance
- **silent-failure-hunter** — audits error handling for swallowed exceptions

If you use Claude Code to work on this repo, those agents are available out of the box.

## License

The code in this repo is provided as-is for reference and learning. Game-related names, marks, and imagery (Warhammer 40,000, Total War: Warhammer III, Space Marine 2, Farming Simulator 25, Shogun 2) belong to their respective rights holders — Games Workshop, Creative Assembly / SEGA, Saber Interactive, GIANTS Software. These are unofficial fan tools with no affiliation.
