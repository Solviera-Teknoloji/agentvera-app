# One MCP server manager for many coding agent CLIs

AgentVera has an MCP manager where you add an MCP server once and every coding agent CLI that takes MCP gets it: Claude Code, Codex, Gemini CLI, Copilot, Cursor and more. You no longer edit each CLI's own config file. The MCP manager is on the free plan.

AgentVera is closed source and is made by Solviera Teknoloji, the owner of this repository. This page describes our own app.

## How it works

- **Add a server once.** Register stdio, HTTP or SSE servers on the MCP page (⌘⌥M). They connect when agents start: to all agents, to the ones you choose, to a group's agents or to a team role.
- **Which agents.** Claude Code, Codex, opencode, Copilot, Qwen Code, Goose, Amp, Cursor, Antigravity, Gemini CLI, Droid, Kimi, Vibe, Crush, Kiro, Cline and Hermes. Aider does not take MCP.
- **A ready catalog.** "+" lists 23 ready servers by category, such as Playwright, Chrome DevTools, Context7, GitHub, Sentry, Supabase, Linear, Notion, Stripe and Figma.
- **Test and token cost.** A connection test lists the server's tools, prompts and resources and an approximate token cost per tool, so you can see how much context a server adds.
- **Secrets.** Secret environment variables and headers are kept in your operating system's keychain and left out of settings backups. Servers can be limited to certain projects.
- **Remote servers and OAuth.** Remote servers go through AgentVera's gateway. Sign in once in the app to a server that needs OAuth, and every agent uses that sign-in; the agent's CLI holds no token.
- **Agents can ask.** An agent can attach a registered server to itself or to an agent of its group. A new server is only added after you approve it in the app.
- **In step with your CLIs.** Servers already in Claude Code's and Codex's own settings are listed with their health; import them or remove them from the CLI.
- **Shared board.** Each project also gets the `agentvera-board` server, where agents post notes, decisions and todos. It is also available as a standalone, MIT-licensed server: [agentvera-board-mcp](https://github.com/Solviera-Teknoloji/agentvera-board-mcp).

## Plans

- **Free:** the MCP manager, the catalog, connection tests and remote servers.
- **Team:** admins can also share MCP servers with the organization (without secret values).

See [pricing](https://agentvera.dev/en/pricing/) for current plans.

## Alternatives

Each CLI has its own MCP commands and config file (for example `claude mcp add`), and there are other MCP managers and registries. If you use only one agent, its own config may be all you need.

## Links

- Full guide: [MCP manager](https://agentvera.dev/en/features/mcp-manager/)
- [Download AgentVera](https://agentvera.dev/en/download/) · [All features](https://agentvera.dev/en/features/) · [All docs](README.md)
