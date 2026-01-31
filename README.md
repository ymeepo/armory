# codeandkin armory

Curated skills for AI-powered development.

## Installation

Add to your Claude Code settings (`.claude/settings.json`):

```json
{
  "plugins": ["github-personal:ymeepo/armory.git"]
}
```

Or clone and add locally:

```bash
git clone github-personal:ymeepo/armory.git
```

Then add to settings:

```json
{
  "plugins": ["/path/to/armory"]
}
```

## Available Skills

### web-ui

Build polished, production-ready web interfaces. Guides to shadcn/ui, Cult UI, and Tailwind CSS.

### git-personal

Personal GitHub account configuration with SSH alias, identity settings, and commit guidelines.

## Project Structure

```
armory/
├── .claude-plugin/
│   └── marketplace.json
├── skills/
│   ├── web-ui/
│   │   └── SKILL.md
│   └── git-personal/
│       └── SKILL.md
└── README.md
```

## Creating Skills

1. Create a directory under `skills/`
2. Add `SKILL.md` with YAML frontmatter:

```yaml
---
name: skill-name
description: When to trigger this skill.
---

# Skill Title

[Instructions for Claude]
```

3. Update `marketplace.json` to include the skill

## License

MIT
