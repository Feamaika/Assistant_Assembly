# Assistant Assembly
*"Assistants... assemble!"* ~CaptAIn America


Custom AI agents for IDEs are mostly Markdown and metadata. I wanted to share a small, GitHub-first collection of shareable GitHub Copilot custom agents and related guidance. I made these using VS Code, but the format is also useable with Cursor or OpenCode.  

This repository is meant to stay simple:

- The agent files are the product.
- The README and License explain how to use and share them.

## Current Contents

Two AI agents:
- `Agent Builder`: a special custom agent for creating, reviewing, and tightening other `.agent.md` files.
- `UI Translator`: a custom agent that checks and translates a solution's front-end language, that was created by `Agent Builder`


## Repository Layout

```text
Assistant_Assembly/
  .github/
    agents/
      agent-builder.agent.md
      ui-translator.agent.md
  examples/
    agent-builder-prompts.md
  .gitignore
  LICENSE
  README.md
```

## How to use

### Option 1: Use this repo as its own workspace

Open this folder in VS Code. Because the agent lives at `.github/agents/agent-builder.agent.md`, it can be discovered as a workspace custom agent.

### Option 2: Copy the Agent into another repository

Copy `.github/agents/agent-builder.agent.md` into the target repository's `.github/agents/` folder.

### Option 3: Keep a personal copy

If you want the agent available across projects, keep a personal copy in your VS Code user customization location for custom agents.

## What Agent Builder does

`Agent Builder` is designed to:

- Create a new custom agent from a rough idea.
- Review an existing `.agent.md` file and tighten it.
- Reduce bloated tool lists.
- Improve discoverability with better descriptions and trigger words.
- Decide whether the user really needs an agent or should use instructions, a prompt, or a skill instead.

## Example prompts

See `examples/agent-builder-prompts.md` for copy-paste prompt patterns.


## Future additions

- ~~A second or third agent so the repo becomes a real collection.~~
- A lightweight install script for Windows and macOS.
- A changelog for changes to shared agents.