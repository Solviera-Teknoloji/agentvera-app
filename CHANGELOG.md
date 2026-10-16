# Changelog

What changed in each AgentVera desktop release. The app updates itself; installers for every platform are on [agentvera.dev/en/download](https://agentvera.dev/en/download/).

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
