# Assistant Assembly
![GitHub License](https://img.shields.io/github/license/Feamaika/Assistant_Assembly)  


*"Assistants... assemble!"* ~CaptAIn America

Custom AI agents for IDEs are mostly Markdown and metadata. I wanted to share a small, GitHub-first collection of shareable GitHub Copilot custom agents and related guidance. I made these using VS Code, but the format is also useable with Cursor or OpenCode.  

This repository is meant to stay simple:

- The agent files are the product.
- The README and License explain how to use and share them.

## Current Contents

There are currently 3 AI agents:
- `Agent Builder`: a special custom agent for creating, reviewing, and tightening other `.agent.md` files.
- `PR Reviewer`: a custom agent that reviews a PR's code changes in the context of the linked work item and the PR description, surfacing potential misalignments, risks, and open questions in clear language.
- `UI Translator`: a custom agent that checks and translates a solution's front-end language, that was created by `Agent Builder`


## Repository Layout

```text
Assistant_Assembly/
  .github/
    agents/
      agent-builder.agent.md
      pr_reviewer.agent.md
      ui-translator.agent.md
  examples/
    agent-builder-prompts.md
  .gitignore
  LICENSE
  README.md
```

## What Agent Builder does

`Agent Builder` is designed to:

- Create a new custom agent from a rough idea.
- Review an existing `.agent.md` file and tighten it.
- Reduce bloated tool lists.
- Improve discoverability with better descriptions and trigger words.
- Decide whether the user really needs an agent or should use instructions, a prompt, or a skill instead.

### Example prompts

See `examples/agent-builder-prompts.md` for copy-paste prompt patterns.

## What PR Reviewer does
`PR Reviewer` is designed to:
- Review a Pull Request's code changes in the context of the linked work item and the PR description, using read-only Azure DevOps tools when available.
- Surface potential misalignments, risks, and open questions in clear language.

## What UI Translator does

`UI Translator` is designed to:

- Translate visible UI text from one language to another.
- Preserve logic, structure, identifiers, and behavior.
- Keep repeated terms and interface copy consistent across files.
- Leave brand names, placeholders, and ambiguous domain terms alone unless the user says otherwise.


## How to use
### Option 1: Quick install

Use the buttons below to install an agent directly into VS Code.

| Agent | Install |
|-------|---------|
| **Agent Builder** | [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://aka.ms/awesome-copilot/install/agent?url=vscode%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2FFeamaika%2FAssistant_Assembly%2Fmain%2F.github%2Fagents%2Fagent-builder.agent.md)  |
| **PR Reviewer** | [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://aka.ms/awesome-copilot/install/agent?url=vscode%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2FFeamaika%2FAssistant_Assembly%2Fmain%2F.github%2Fagents%2Fpr_reviewer.agent.md)  |
| **UI Translator** | [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://aka.ms/awesome-copilot/install/agent?url=vscode%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2FFeamaika%2FAssistant_Assembly%2Fmain%2F.github%2Fagents%2Fui-translator.agent.md)  |

### Option 2: Manual setup

Choose manual setup if you want to inspect, edit, version, or reuse the agent files yourself.

- **Workspace-local:** open this repository in VS Code. Agents placed in `.github/agents/` can be discovered as workspace custom agents.
- **Repo-local:** copy one or both agent files from `.github/agents/` into another repository's `.github/agents/` folder.
- **Personal:** keep one or both agent files in your VS Code user custom agents location to make them available across projects.

Current agent files:

- `.github/agents/agent-builder.agent.md`
- `.github/agents/pr_reviewer.agent.md`
- `.github/agents/ui-translator.agent.md`



## Future additions

- ~~A lightweight install script.~~
- ~~Agents to add to the collection.~~
- A changelog for changes to shared agents.