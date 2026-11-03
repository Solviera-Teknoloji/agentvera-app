# Auto-switch Claude Code and Codex accounts at the usage limit

AgentVera, a desktop app for macOS, Windows and Linux, moves a Claude Code or Codex agent to your next account when the current one runs low on its 5-hour or weekly limit. You put your accounts in a chain; when one runs out, the agent moves to the next one and goes on with the same conversation. It is on the Pro and Team plans.

AgentVera is closed source and is made by Solviera Teknoloji, the owner of this repository. This page describes our own app.

## How it works

- **Account chains.** In the account switching settings you build one chain for Claude Code and one for Codex. A chain needs at least two accounts and has no upper limit. After the last account it wraps around to the first.
- **Threshold.** You set how much of the 5-hour or weekly limit must be left before a switch. The default is 3% left. Switching is off until you turn it on.
- **When it checks.** AgentVera reads each account's usage every 90 seconds. It also switches right away when the CLI itself prints its limit message.
- **Running turns are not cut off.** If an agent is only near the threshold and is still working, the switch waits until the turn ends, for up to 20 minutes. After that it switches anyway.
- **Cooldown.** The same agent is not switched again within 5 minutes, unless the account it just moved to is out of quota too; then it goes on along the chain.
- **Same conversation.** With "Move the conversation to the new account" on (the default), the conversation is copied to the new account and the agent is told to continue where it stopped. With it off, the switch starts a new conversation.
- **Bad logins are skipped.** An account that is signed out, or whose login the provider rejects, is skipped. An account that hit its limit is skipped until its window resets.
- **When every account is out.** The agent waits. You get a notice, and when a limit resets the agent goes on by itself.
- **Other CLIs.** Cursor, Gemini CLI, Copilot, opencode and other agents have their own accounts and a per-agent fallback order under Settings → Accounts → Accounts of other agents.

Limits are read from Anthropic's usage service for Claude and from `codex app-server` for Codex. These are not stable public APIs, so treat the numbers as a guide.

Only chain accounts you are entitled to use.

## Plans

- **Free:** the app and unlimited agents, with no automatic switching. When an agent hits its limit, it stops and the app tells you that Pro would move it to your other account.
- **Pro and Team:** automatic account switching. Pro has a 7-day free trial.

See [pricing](https://agentvera.dev/en/pricing/) for current plans.

## Alternatives

Other tools also switch accounts automatically, such as claude-swap, ccswap, ccam and the AgentPool VS Code extension. Several are open source and free. Our comparison lists what each one does, based on its own page.

## Links

- Full guide: [Automatic account switching](https://agentvera.dev/en/features/account-switching/)
- Comparison: [Claude Code account switchers compared](https://agentvera.dev/en/blog/claude-code-account-switchers/)
- [Download AgentVera](https://agentvera.dev/en/download/) · [Pricing](https://agentvera.dev/en/pricing/) · [All docs](README.md)
