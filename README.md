# command-add-feature

A Claude Code slash command for implementing features from GitHub issues.

## Installation

```bash
# Clone to your claude-commands directory
git clone git@github.com:claude-commands/command-add-feature.git ~/projects/claude-commands/command-add-feature

# Create symlink
ln -s ~/projects/claude-commands/command-add-feature/add-feature.md ~/.claude/commands/add-feature.md
```

## Usage

```
/add-feature 123
```

Where `123` is the GitHub issue number.

## What it does

1. Fetches issue details from GitHub
2. Explores the codebase for relevant patterns
3. Plans the implementation approach
4. Creates a feature branch (`feat/123-short-desc`)
5. Implements the feature following project conventions
6. Writes comprehensive tests
7. Runs the test suite and linting
8. Creates a PR referencing the issue

## Requirements

- `gh` CLI installed and authenticated
- Git repository with GitHub remote
- Claude Code with Opus 4.5 model access

## Updates

```bash
cd ~/projects/claude-commands/command-add-feature && git pull
```
