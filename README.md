# ADD Framework Plugin for Claude Cowork

[![GitHub stars](https://img.shields.io/github/stars/dragosroua/claude-assess-decide-do-mega-prompt?style=social)](https://github.com/dragosroua/claude-assess-decide-do-mega-prompt)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**The first human cognitive framework integrated into an LLM — now as a Claude Cowork plugin.**

This plugin brings the Assess-Decide-Do (ADD) framework to Claude Cowork, enabling Claude to detect your cognitive realm and respond appropriately.

## Installation

### GitHub Marketplace
```bash
/plugin marketplace add dragosroua/add-framework-cowork-plugin
/plugin install add-framework
```

### Direct Install (alternative)
```bash
/plugin install github:dragosroua/add-framework-cowork-plugin
```

### From Local Directory

```bash
git clone https://github.com/dragosroua/add-framework-cowork-plugin.git
/plugin marketplace add ./add-framework-cowork-plugin
/plugin install add-framework
```

## Commands

| Command | Description |
|---------|-------------|
| `/add-framework:assess` | Enter ASSESS mode — explore and capture |
| `/add-framework:decide` | Enter DECIDE mode — prioritize and commit |
| `/add-framework:do` | Enter DO mode — pure execution |
| `/add-framework:status` | Check current realm and flow status |
| `/add-framework:balance` | Diagnose realm imbalances |
| `/add-framework:add-help` | Framework overview and help |

## Skills

The plugin includes universal ADD skills that Claude uses automatically:

| Skill | Purpose |
|-------|---------|
| `add-core` | Core framework awareness |
| `add-assess` | Assess realm support |
| `add-decide` | Decide realm support |
| `add-do` | Do realm support |
| `add-imbalance` | Stuck pattern detection |
| `add-realm-detection` | Realm detection patterns |

Skills are pulled from [add-framework-skills](https://github.com/dragosroua/add-framework-skills) — the single source of truth for ADD methodology.

## Usage Examples

### Feeling Overwhelmed?
```
/add-framework:assess
> "I have so many things going on..."
```
Claude helps you capture and organize without pressure.

### Need to Prioritize?
```
/add-framework:decide
> "I know my options. Now I need to choose."
```
Claude helps you make clear, confident decisions.

### Ready to Execute?
```
/add-framework:do
> "I've committed. Help me get it done."
```
Claude provides focused execution support.

### Stuck in a Pattern?
```
/add-framework:balance
```
Claude diagnoses your realm balance and suggests rebalancing.

## Architecture

```
add-framework-cowork-plugin/
├── .claude-plugin/
│   └── plugin.json           # Plugin manifest
├── commands/                  # Cowork-specific commands
│   ├── assess.md
│   ├── decide.md
│   ├── do.md
│   ├── status.md
│   ├── balance.md
│   └── add-help.md
└── skills/                    # Universal ADD skills (from add-framework-skills)
    ├── add-core/
    ├── add-assess/
    ├── add-decide/
    ├── add-do/
    ├── add-imbalance/
    └── add-realm-detection/
```

## Updating Skills

Skills are managed via git subtree from [add-framework-skills](https://github.com/dragosroua/add-framework-skills):

```bash
# Update to latest skills
git subtree pull --prefix=skills \
  https://github.com/dragosroua/add-framework-skills.git main --squash
```

## Related Projects

- **[add-framework-skills](https://github.com/dragosroua/add-framework-skills)** — Universal ADD skills (source of truth)
- **[claude-assess-decide-do-mega-prompt](https://github.com/dragosroua/claude-assess-decide-do-mega-prompt)** — Full Claude Code integration
- **[addTaskManager](https://itunes.apple.com/app/apple-store/id1492487688?mt=8)** — iOS/macOS app implementing ADD
- **[Assess - Decide - Do hubpage on dragosroua.com](https://dragosroua.com/assess-decide-do-framework/)** — all related framework posts from 2009 to 2026

## License

MIT License

## Author

Created by [Dragos Roua](https://dragosroua.com)

---

*"When AI understands where you are in your thinking, collaboration transforms from transactional to relational."*
