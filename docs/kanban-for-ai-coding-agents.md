# A team kanban that hands cards to AI coding agents

AgentVera's team kanban is a shared board inside the desktop app where you hand a card to a coding agent running on your own computer. The card goes to the agent as a task, and when the agent finishes, its reply is posted on the card. Your team sees the board live; your code stays on your machine. It is on the Pro and Team plans.

AgentVera is closed source and is made by Solviera Teknoloji, the owner of this repository. This page describes our own app.

## How it works

- **Link a project.** Sign in, then link a local project to a cloud project in your organization. The server never learns your local folder; only cards, comments and assignments are shared.
- **The board.** Default columns are To do, In progress, Test and Done; rename them or add more. Cards have labels, members, due dates, descriptions, checklists, attachments up to 25 MB and comments. Changes show live on your team's screens.
- **Assign a card to an agent.** In the card window, pick one of the project's running agents or start a new agent with an agent CLI on your computer. The card moves to In progress. A busy agent takes the card after its current work.
- **The reply comes back.** When the agent finishes its turn, its last reply (up to 4,000 characters) is posted as a card comment and the card moves to a Test or Review column. That reply text is stored on the AgentVera server so your team can see it.
- **Your login, your machine.** The agent runs on your computer with your own CLI sign-in.
- **Client boards.** A separate board for a client, with its own columns. Send a client card to the dev board; the client card follows as the dev card moves. Clients never see the dev board or internal notes.
- **Sharing.** A board can be shared by link or with invited e-mails only. Guests sign in with an e-mail link that lasts 15 minutes.
- **Team sync (Team plan).** See your team's open agents (repo, branch, status and changed file paths, never file contents), get a warning when two people's agents touch the same file, and hand an agent's work to a teammate through a card.

## Plans

- **Free:** no boards.
- **Pro:** up to 10 boards. 7-day free trial.
- **Team:** unlimited boards, team sync, shared MCP servers and policies, and a custom domain for public boards. Priced per seat.

See [pricing](https://agentvera.dev/en/pricing/) for current plans.

## Alternatives

Cards can also reach agents through GitHub issues assigned to Copilot, Claude or Codex, through Linear's agent delegation, or through boards that agents pull work from over MCP. Our comparison describes each one from its own site.

## Links

- Full guide: [Team kanban](https://agentvera.dev/en/features/teams-and-kanban/)
- Comparison: [Kanban boards for AI coding agents](https://agentvera.dev/en/blog/kanban-boards-for-ai-coding-agents/)
- [Download AgentVera](https://agentvera.dev/en/download/) · [Pricing](https://agentvera.dev/en/pricing/) · [All docs](README.md)
