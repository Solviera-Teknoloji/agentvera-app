# Changelog

What changed in each AgentVera desktop release. The app updates itself; installers for every platform are on [agentvera.dev/en/download](https://agentvera.dev/en/download/).

## 0.8.5 (2026-10-23)

- When a new version is out, a window shows what it brings and updates in one click.
- The first launch after an update shows what is new in that version.
- The assistant and the chat no longer get stuck at the "do you trust this folder?" question.
- An agent whose CLI ended on its own keeps its last screen.
- Sessions opened from a phone show as "AgentVera Mobile" in the device list.
- A confirmation email is sent when a paid subscription starts.
- Security hardening across the app and the server.

## 0.8.4 (2026-10-22)

- On the Free plan, a prompt on launch shows what Pro adds.

## 0.8.3 (2026-10-22)

- A personal assistant that knows every project, your notes, tasks and past conversations. It reads your day, follows your agents and chats in its own window.
- Project memory: agents leave handoff notes with open threads, recall and remember decisions (`brain_recall`, `brain_remember`), and the memory is compiled every night.

## 0.8.2 (2026-10-21)

- Agents can start in auto or full-permission mode, set per agent.
- A full menu bar with the app's own actions, your shortcuts and your projects.
- Fixes: Gemini agents get their MCP servers again, Codex and Gemini agents resume after a relaunch, and the browser stays smooth on busy sites.

## 0.8.1 (2026-10-18)

- The browser remembers: history, bookmarks, suggestions and tabs that come back.
- A sleeping agent keeps its conversation on screen.

## 0.8.0 (2026-10-18)

- A built-in browser you can live in.
- A catalog of 1,036 permissively licensed skills for every agent.
- Sleep prevention follows the setting.
- Four new games, including a Doom-style shooter.
- macOS releases are signed with a Developer ID and notarized.

## 0.7.2 (2026-10-17)

- Local agents reach remote MCP servers through AgentVera's gateway: OAuth sign-in happens once in the app, and every CLI can use SSE servers.
- Agents list the MCP servers, attach them to themselves or their group and ask you for new ones.
- Groups and team roles carry MCP servers, so ready-made teams start with their tools. The catalog adds Canva, fal.ai and Meta Ads.
- Customer board tabs count the cards added since the board was last opened.

## 0.7.1 (2026-10-16)

- The team view shows each agent's request, its current step and how long it has been working.
- Permission prompts of a team's agents are answered from the team view, without opening each agent.
- An agent of a team can be redirected mid-task from the team view.
- The team view stays with its group and shows what the team is doing now.

## 0.7.0 (2026-10-15)

- Teams: open agents work as a team led by a manager agent, run from a team view in the workspace.
- Agents can start parallel teams themselves; night shifts can run per project or per group with chosen agents.
- Flows send requests, chat messages, Telegram and e-mail, run commands, write files and wait until a set time.
- Automatic `/compact` for every agent, on by default, and leaner reading for every agent.
- Accounts of other CLIs are added by signing in, as with Claude Code and Codex; Cursor accounts sign in on a Mac.
- Hooks for Hermes and Crush agents.
- AI ROI shows where the spend goes by context size.
- Files and folders can be managed from the file tree with a right click.

## 0.6.19 (2026-10-14)

- Orchestration works with every agent CLI, not only Claude Code and Codex.
- Permission prompts of every CLI are answered with the right keys.
- Usage and cost of every agent CLI in statistics, AI ROI and budgets; replies and context size read from each CLI's own history.
- Hooks for Droid and Cursor agents.
- A kanban card's files go to the agent with the card.

## 0.6.18 (2026-10-14)

- Paste files and screenshots into an agent.

## 0.6.17 (2026-10-14)

- Accounts and limit fallback for every CLI agent, not only Claude Code and Codex.
- Every local agent can message the others.
- MCP servers for every agent CLI that can take them.

## 0.6.14 – 0.6.16 (2026-10-12 – 2026-10-13)

- The app follows a language option (English or Turkish); new installs start in English.
- Account chains skip every account out of quota, and agents go on by themselves after an automatic switch.
- A memory guard restarts an agent that grew to several GB, with the same conversation.
- Project map redesigned with folders, drag-to-pin and level of detail.
- Night shift redesign and a night shift tab in the project.
- Drop files on an agent to hand them over.
- Fixes: agent status follows real work, statistics on long conversations, saves after a failed save.

## 0.6.13 (2026-10-12)

- Review inbox, file ownership, shared tasks, token budgets, agents in Docker, team timeline, phone view and approval reminders.
- Agents of a group message each other across CLIs.

## 0.6.12 (2026-10-11)

- Orchestration: automations, playbooks, merge queue, supervisor and resource planner.
- Agents open agents of their own when the work calls for it.
- Personal tasks with reminders in the right panel.
- Telegram relay through the official AgentVera bot, with a topic per agent.
- A local agent can use chosen SSH servers while it works in the project folder.
