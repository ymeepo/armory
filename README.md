# Armory

Claude plugin marketplace for AI-powered development skills.

## Overview

Armory is a collection of agent skills designed to accelerate development workflows with Claude Code. Each skill provides specialized knowledge and best practices that Claude can apply automatically when relevant.

## Installation

Add armory as a plugin source in your Claude Code settings:

```bash
claude plugins add armory /path/to/armory
```

Or install specific plugins:

```bash
claude plugins install web-ui@armory
```

## Available Plugins

### web-ui

UI prototyping and interface design skills.

**Skills:**
- `web-ui-prototyper` - Creates polished, production-ready web UI interfaces

## Project Structure

```
armory/
├── .claude-plugin/
│   └── marketplace.json     # Plugin marketplace configuration
├── skills/                  # Agent reference skills
│   └── web-ui-prototyper/
│       └── SKILL.md
├── commands/                # User-invoked interactive workflows
└── README.md
```

## Creating New Skills

1. Create a new directory under `skills/`
2. Add a `SKILL.md` file with YAML frontmatter:

```yaml
---
name: your-skill-name
description: Brief description of when to use this skill.
---

# Skill Title

[Skill content and instructions for Claude]
```

3. Update `marketplace.json` to include your skill

## Contributing

1. Fork the repository
2. Create a new skill in `skills/`
3. Test with Claude Code
4. Submit a pull request

## License

MIT
