---
name: git-personal
description: Use personal GitHub account for git operations. Triggers when user mentions personal github, personal credentials, personal profile, ymeepo, or github-personal.
---

# Personal GitHub Configuration

Use this configuration when working with the user's personal GitHub account.

## SSH Configuration

Use the `github-personal` SSH alias for all remote operations:

```
github-personal:ymeepo/<repo>.git
```

## Git Identity

Configure commits with:

- **Name:** Ronald Leung
- **Email:** rcmleung@gmail.com

Set locally per repository:
```
git config user.name "Ronald Leung"
git config user.email "rcmleung@gmail.com"
```

## Commit Message Guidelines

Write concise, human-authored commit messages:

- Use imperative mood ("Add feature" not "Added feature")
- Keep subject line under 50 characters
- Focus on what and why, not how
- No AI attribution or co-author tags
- No references to code generation tools

**Good:**
```
Add user authentication endpoint

Implements JWT-based auth with refresh tokens.
```

**Avoid:**
```
Add user authentication endpoint

Co-Authored-By: Claude...
Generated with AI assistance...
```
