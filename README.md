# armory

A codeandkin plugin. Curated skills for AI-powered development.

## Installation

First, add the marketplace:

```shell
/plugin marketplace add codeandkin/armory
```

Then install plugins:

```shell
/plugin install web-ui@codeandkin-armory
/plugin install git-personal@codeandkin-armory
```

Skills will be available under each plugin's namespace (e.g., `web-ui:`, `git-personal:`).

## Local Development

To test the plugin locally during development, use the `--plugin-dir` flag:

```bash
claude --plugin-dir /path/to/armory
```

Skills will be available under the `armory:` namespace (e.g., `armory:web-ui`).

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
