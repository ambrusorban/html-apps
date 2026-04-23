# HTML Apps

A workspace for standalone HTML5 applications. Each app is fully self-contained — no build tools, no bundlers, no `npm install`. Open the `index.html` in any modern browser and it just works.

Built with [Claude Code](https://claude.com/claude-code) as a reference for what an LLM-assisted single-file app workflow can look like.

## Apps in this repo

### [`sm2-loadout/`](./sm2-loadout/) — Astartes Loadout Cogitator

A quick-reference loadout planner for [Warhammer 40,000: Space Marine 2](https://spacemarine2.fandom.com/) Operations co-op mode. Designed to be glanced at alongside the game when picking a mission.

**Features:**
- All 12 Operations missions across Avarax, Demerium, Kadaku, Agathon, and Orbit
- All 7 classes (Tactical, Bulwark, Heavy, Sniper, Vanguard, Assault, Techmarine)
- Loadout suggestions adapt to selected mission **faction** (Tyranid / Chaos / Mixed) and **difficulty** (Minimal → Absolute)
- Weapon recommendations color-coded by rarity tier: Standard / Master-Crafted / Artificer / Relic
- Per-class mission role descriptions explaining what each Battle-Brother should be doing
- Synergy rationale for the recommended team composition
- Hazard intel and active difficulty modifiers per mission
- Mission rewards (XP, Requisition, Armory Data tier) scale with difficulty
- Keyboard navigation: `←`/`→` to cycle missions, `↑`/`↓` to change difficulty
- Dark, high-contrast, GTFO-inspired UI

**To run:** double-click `sm2-loadout/index.html`.

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

The code in this repo is provided as-is for reference and learning. Warhammer 40,000, Space Marine 2, all related names, marks, and imagery are © Games Workshop / Saber Interactive — this is an unofficial fan tool with no affiliation.
