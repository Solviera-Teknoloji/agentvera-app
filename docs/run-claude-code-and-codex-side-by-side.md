# Run Claude Code, Codex, Gemini CLI and others side by side

AgentVera is a desktop app for macOS, Windows and Linux that runs the coding agent CLIs already on your computer in real terminals, side by side, in one window per project. Each agent uses its own CLI and its own login, so your Claude or ChatGPT plan works as it is and no API key is needed. Running agents side by side is on the free plan, with no limit on the number of agents.

AgentVera is closed source and is made by Solviera Teknoloji, the owner of this repository. This page describes our own app.

## How it works

- **Supported agents.** Claude Code, Codex, Gemini CLI, GitHub Copilot CLI, Cursor Agent, Antigravity, opencode, Hermes, Qwen Code, Kimi Code, Kiro, Amp, Factory Droid, Goose, Mistral Vibe, Crush, Aider and Cline, plus plain terminals (zsh, bash, fish) for any other CLI.
- **A grid per project.** Lay out agents in anything from 1×1 to 5×4. Column widths, row heights and placement are remembered per project. Drag panes to swap them, double-click a title to maximize, or open an agent in its own window.
- **Projects keep running.** Switch to another project and the agents of the first keep working in the background.
- **Git worktrees.** Each agent can work in its own git worktree, and you get a warning when two agents edit the same file.
- **Groups.** Agent groups have their own layout and a shared notice board.
- **Keyboard.** A ⌘K command palette, ⌘1–9 to jump to panes, and shortcuts you can remap.
- **Missing CLIs.** The new agent dialog shows the install command when a CLI is missing, and you can install it in a terminal inside the app.
- **Coming back.** When you quit, terminals close cleanly. Next time, every agent except plain terminals returns to its conversation from its CLI's local history.

Your code, conversations and settings stay on your computer. Agents talk to their own providers under your accounts.

## Plans

- **Free:** every core feature, including the multi-agent workspace, worktrees, MCP, Git, Docker, SSH and code review. No account is needed for the core.
- **Pro and Team:** add automation and team features such as flows, night shift, auto approval, account switching and team kanban.

See [pricing](https://agentvera.dev/en/pricing/) for current plans.

## Alternatives

You can also run agents side by side in tmux panes or in other desktop apps for parallel agents. Our comparison pages describe each one from its own site.

## Links

- Full guide: [Workspace](https://agentvera.dev/en/features/workspace/) · [All features](https://agentvera.dev/en/features/)
- One page per agent: [agentvera.dev/en/agents](https://agentvera.dev/en/agents/)
- Comparison: [Best tools to run AI coding agents in parallel](https://agentvera.dev/en/blog/best-tools-parallel-ai-coding-agents/)
- [Download AgentVera](https://agentvera.dev/en/download/) · [All docs](README.md)
