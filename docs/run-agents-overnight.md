# Run coding agents overnight: night shift, auto approval and the morning summary

AgentVera's night shift lets you queue tasks in the evening, give each one to a coding agent, and read one report in the morning with each task's result, the draft pull requests opened and anything that got stuck. Auto approval answers Claude Code's safe permission prompts so agents don't wait for you all night. Both are on the Pro and Team plans.

AgentVera is closed source and is made by Solviera Teknoloji, the owner of this repository. This page describes our own app.

## How it works

### Night shift

- **A shift per project and group.** Each has its own hours, queue and morning report. The default window is 23:00–07:00, and it can start on its own every night.
- **Who does the task.** Give a task to an open agent, or have a new Claude Code or Codex agent opened for the night. A new agent works in its own git worktree on a `night/<date>-<slug>` branch and closes when done.
- **Parallel tasks.** Two tasks run at once by default, up to six. Tasks given to the same agent run one after another.
- **Rules for the agent.** The agent is told you are asleep: it must not ask questions, it commits but does not push, runs the tests and ends with a done or stuck marker. If it stops without a marker, it is nudged up to twice, then marked stuck.
- **Draft pull requests.** A draft pull request is opened on GitHub for a new agent's finished work.
- **Approvals.** Requests waiting for an approval are not approved overnight by the night shift; they are listed in the morning report.

### Auto approval (Claude Code)

- Approves only requests known to be safe: read tools, read-only shell and git commands, and test, lint, typecheck and build commands.
- Commands with redirects (`>`), `$()` or backticks are never approved automatically.
- File edits inside the project are approved only if you turn that option on; `.git` and `.env` files never are.
- A never-approve list starts with `git push`, `npm publish`, `rm`, `git reset --hard` and `git clean`, and you can add your own. Your own Claude allow and deny rules still apply.

### The morning summary

When the window ends you get a desktop notification, and the report is saved as a Markdown file. A summary card shows what your agents did while you were away. With Telegram on, a summary with counts only (done, PRs opened, stuck, still running) is sent too.

The night shift needs the app open and the computer awake. If an account runs out of quota at night, [account switching](auto-switch-claude-code-accounts.md) can move the agent to your next account.

## Plans

- **Free:** run agents yourself; no night shift or auto approval. On Free, the auto approval switch looks on but requests still come to you.
- **Pro and Team:** night shift and auto approval. Pro has a 7-day free trial.

See [pricing](https://agentvera.dev/en/pricing/) for current plans.

## Links

- Full guide: [How to run Claude Code overnight](https://agentvera.dev/en/blog/run-claude-code-overnight/) (also covers doing it with the Claude Code CLI alone)
- Features: [Night shift](https://agentvera.dev/en/features/night-shift/) · [Auto approval](https://agentvera.dev/en/features/auto-approval/)
- [Download AgentVera](https://agentvera.dev/en/download/) · [Pricing](https://agentvera.dev/en/pricing/) · [All docs](README.md)
