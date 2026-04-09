# Agent Builder Prompt Patterns

These are good copy-paste starting points for invoking `Agent Builder`.

## Create A New Personal Agent

```text
Create a personal GitHub Copilot agent for cross-project use. It should help me review Python scripts for reliability and maintainability. Keep the tool list minimal, make it user-invocable, and put it in the right location for a personal agent. Also give me two test prompts.
```

## Create A Repo-Specific Agent

```text
Create a workspace agent at `.github/agents/frontend-reviewer.agent.md` for reviewing React UI changes. It should focus on regressions, accessibility, and design-system consistency. Limit the tools to what it actually needs and make the output format strict.
```

## Tighten An Existing Agent

```text
Review my existing `.agent.md` file and tighten it. I want fewer tools, a sharper description, better trigger phrases, and clearer constraints. Keep the original intent but remove anything vague.
```

## Split One Broad Agent Into Two

```text
I have one broad agent that tries to plan, code, and review. Decide whether that should be split into multiple agents. If yes, design the split, explain the tradeoff, and rewrite the files.
```

## Decide If An Agent Is Even The Right Primitive

```text
I want always-on guidance for writing SQL safely across one repository. Decide whether this should be a custom agent, instructions, a prompt, or a skill. If an agent is not the right fit, say so clearly and create the better alternative instead.
```

## Build A Safer Agent

```text
Create a deployment helper agent, but keep it conservative. It should read deployment docs and prepare commands, but it must not execute destructive operations unless the user explicitly asks. Make the restrictions explicit in the file.
```

## Review Checklist Prompt

```text
Audit this custom agent against a strong review checklist: single role, correct scope, minimal tools, discoverable description, explicit boundaries, useful output format, and valid frontmatter. Then apply the fixes.
```