# Changelog

What changed in each AgentVera desktop release. The app updates itself; installers for every platform are on [agentvera.dev/en/download](https://agentvera.dev/en/download/).

## 0.9.0 (2026-11-01)

- Themes: pick a light or dark color theme in Settings > Appearance (Midnight, Forest, Rose, Amber, Ocean, Violet, Sepia, Mint, Sky, Graphite); terminal colors follow the theme.
- New languages: the interface and release notes now come in German, Spanish, French, Portuguese and Russian.
- Memory: project maps and the code map use less memory in the main process, so long sessions no longer grow the way they did.
- Project board (agentvera-board MCP): agents post decisions, findings and todos as short notes on the project board, and the other agents and you can read them and pick up from there.
- Different plans on one email: add the same email once for your personal plan and once for your team plan; account cards and the account picker show each one's organization and plan, and warn when two accounts share one organization.
- When usage can't be read, the limit bar at the bottom of the window shows the last reading instead of "No data".
- Windows: missing agent CLIs install through winget/PowerShell, and the Windows build is built and launch-tested automatically on every release.
- Templates: share your flows and teams as a file or a link, and add ready-made templates from the community gallery to a project in one click; templates never include addresses, secrets or file paths.
- Night shift summary: what your agents did while you were away is waiting in one card in the morning.
- Invite a friend: when the person you invite joins, you both get a free month of Pro.
- First run has a short quick start, and you can install missing agent CLIs in a terminal inside the app.

## 0.8.18 (2026-10-30)

- The new agent dialog shows the install command when Claude Code or Codex is missing: copy it, install, then check again with one click.
- When an agent on the Free plan hits its account limit, you see that on Pro it would move to your other account by itself and carry on.

## 0.8.17 (2026-10-29)

- Smoother switching when an account runs out: agents move to the next account as soon as the CLI reports the limit, and near the limit they switch between turns instead of cutting a running turn off.
- Lower memory use: diagnostics, conversation search and other CLIs' histories no longer load whole files into memory.
- A suggestion card shows skills that fit your project's stack and the kind of work you do.
- Agents launch at their pane's size, so the terminal looks right from the start.

## 0.8.15 (2026-10-28)

- Better terminal on Windows: Ctrl+letter shortcuts go to the terminal, typing with AltGr no longer fires shortcuts, Ctrl+C/Ctrl+V copy and paste, and the terminal menu has Paste.
- On Windows, closing an SSH tab ends the connection fully, background processes no longer flash console windows and cmd shows non-ASCII text correctly.
- Signed-out users see what an account adds (phone control, sync) after an agent finishes real work.

## 0.8.14 (2026-10-28)

- opencode agents can be resumed and forked again: session creation with opencode 2.x is fixed.
- Read-only server and database modes are stricter: commands and queries that could change the system now ask for approval.
- Removing a team backs up uncommitted changes first, so no work is lost.
- Preview and dev servers now stop when the app quits.
- Tasks on remote servers are more reliable: long tasks no longer run twice and status updates survive a dropped connection.
- File names show correctly on Windows, plus small translation fixes.

## 0.8.13 (2026-10-26)

- In the file browser, drag and drop files between the server and your computer; server files can also be dragged to Finder or the desktop.

## 0.8.12 (2026-10-26)

- Small improvements and stability fixes.

## 0.8.11 (2026-10-25)

- Kimi Code 2.x now starts inside AgentVera: the "unknown option '--mcp-config-file'" error is fixed, and your MCP servers load through Kimi Code's own config folder.
- Settings → Permission rules: view and edit each agent CLI's own permission rules (allow / ask / deny) per scope and account.
- A tidier sidebar: the link row under each agent is gone.

## 0.8.10 (2026-10-25)

- The SFTP / FTP browser is redesigned: folder tree, back/forward, sortable columns, a filter, hidden files and keyboard shortcuts.
- Type or paste a path (~, file:// and sftp:// work too) to go straight there; a file path opens its folder with the file selected. Local files open in their app or show in their folder.
- The games are livelier: new effects and graphics, better mechanics and a map in the dungeon.
- On Windows the terminal scrolls back now, so earlier Claude Code and Codex output is reachable again.

## 0.8.9 (2026-10-24)

- When you correct an agent (say, "no, use pnpm" in the chat), AgentVera suggests a lasting rule; the ones you accept are written to AGENTS.md, CLAUDE.md, GEMINI.md, .cursorrules and the other instruction files at once, so every agent follows them.
- The new Rules tab in the Brain panel lists the learned rules; edit or remove one and every file follows.

## 0.8.7 (2026-10-24)

- Editing an agent now keeps its conversation and memory, and moving it to another account continues the same conversation. Only changing the tool starts a new one.
- Automatic account switching now reaches every session that hits a limit, including when several hit it at once or a session has no account set.

## 0.8.6 (2026-10-24)

- Send feedback from the Help menu, the status bar or Settings → About, with optional diagnostics.
- When the app crashes or an agent exits with an error, a scrubbed error report is sent; turn it off in Settings → About.
- Emails to your account now follow the language you chose in the app.
- The memory guard counts the Windows commit limit and warns you when the machine runs low on memory.
- The web panel is available in English, with its pages in a single top bar.
- Payment receipts are sent with the subscription-started email.

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
