<p align="center">
  <a href="https://agentvera.dev/en/"><img src="assets/banner.png" alt="AgentVera: every coding agent you use, in one window" width="100%"></a>
</p>

<h1 align="center">AgentVera</h1>

<p align="center">
  <b>Run Claude Code, Codex, Gemini CLI, Copilot and 14 more AI coding agents side by side, on macOS, Windows and Linux.</b><br>
  <a href="https://agentvera.dev/en/">Website</a> ·
  <a href="https://agentvera.dev/en/download/">Download</a> ·
  <a href="https://agentvera.dev/en/features/">Features</a> ·
  <a href="https://agentvera.dev/en/pricing/">Pricing</a> ·
  <a href="https://agentvera.dev/en/blog/">Blog</a> ·
  <a href="#türkçe">Türkçe</a>
</p>

---

AgentVera is a desktop app that runs the coding agents already installed on your computer in real terminals, side by side, per project. Every agent uses its own CLI and its own login (your Claude Pro/Max or ChatGPT plan works as is; no API key needed), and AgentVera adds what is missing between them: layouts, git worktrees, flows, reviews, limits and cost.

This repository is AgentVera's public home: **releases, issues and feature requests**. The app itself is closed source.

<p align="center">
  <img src="assets/workspace.png" alt="Claude Code, Codex, Gemini CLI and Copilot running side by side in AgentVera" width="100%">
</p>

## New in 0.7: agent teams

Build a team from the agents already open in your workspace. Pick a manager, give every agent a role (researcher, planner, developer, reviewer or your own), and draw who hands work to whom. Then write one request: the manager splits it up, the members pass work along, and you watch it happen.

<p align="center">
  <img src="assets/team.png" alt="Team view: a manager hands work to research, planning, UI and review agents" width="100%">
</p>

- **Live team view.** Every card shows the agent's request, current step and time. Answer permission prompts on the card, interrupt an agent and redirect it, or flip a card into its live terminal.
- **Any CLI in any seat.** A Claude Code manager can lead Codex, Gemini and Copilot members; the team only works when you give it work.
- **Agents start teams too.** An agent can split a big task into parallel teams on its own, and night shifts can run per group.

<p align="center">
  <img src="assets/team-detail.png" alt="An agent's card opened in the team view with its request, steps and terminal" width="100%">
</p>

## Supported agents

Claude Code · Codex · Gemini CLI · GitHub Copilot CLI · Cursor Agent · Antigravity · opencode · Hermes · Qwen Code · Kimi Code · Kiro · Amp · Factory Droid · Goose · Mistral Vibe · Crush · Aider · Cline, plus plain terminals for any other CLI. [One page per agent →](https://agentvera.dev/en/agents/)

## What it does

- **Parallel agents, one window.** Grids from 1×1 to 5×4, agent groups with their own layout and shared notice board, an optional git worktree per agent, and a warning when two agents edit the same file.
- **Work between agents.** [Flows](https://agentvera.dev/en/features/flows/) pass one agent's reply to the next and can send HTTP requests, chat, Telegram and e-mail messages, run commands and write files; a [research → plan → build](https://agentvera.dev/en/features/research-plan-build/) pipeline; [night shift](https://agentvera.dev/en/features/night-shift/) runs queued tasks overnight and opens draft PRs.
- **Quality.** Automatic [code review](https://agentvera.dev/en/features/code-review/) when a turn ends, acceptance checks (Verify), [checkpoints and replay](https://agentvera.dev/en/features/checkpoints-and-replay/), and a project map (a tree-sitter code graph over MCP) so agents find the right files without reading the repo.
- **Every CLI, fully supported.** Sign in to the accounts of every agent CLI without an API key; orchestration, agent-to-agent messages, MCP servers, permission prompts, usage and cost work the same for all of them.
- **Limits and cost.** [Account switching](https://agentvera.dev/en/features/account-switching/) when a 5-hour or weekly limit runs low, context profiles, automatic `/compact`, bundled [RTK](https://github.com/rtk-ai/rtk) that compresses shell output before it reaches the model, and an "Automatic" model that picks Haiku, Sonnet or Opus per task.
- **Skill gallery.** Share agent skills with everyone or your organization; every version is security-scanned and public ones are moderator-approved. [Browse skills →](https://app.agentvera.dev/skills)
- **Hand work over easily.** Paste or drop files and screenshots onto an agent; right-click the file tree to create, rename, duplicate, reveal or delete files.
- **From your phone.** Control your agents remotely: projects, git, statistics, voice input, tasks, Docker and limits.
- **Tools agents need.** [MCP manager](https://agentvera.dev/en/features/mcp-manager/), [database manager](https://agentvera.dev/en/features/database-manager/), [SSH/SFTP](https://agentvera.dev/en/features/ssh-and-sftp/) with per-host rules and an encrypted vault, Docker, an API client, an agent browser, and a [runner](https://agentvera.dev/en/runner/) for agents on your own server.
- **Teams.** Organizations, a [team kanban](https://agentvera.dev/en/features/teams-and-kanban/) whose cards go to your running agents, invite-only customer boards and [webhooks](https://agentvera.dev/en/webhooks/).

Your code, conversations and settings stay on your computer; agents talk to their own providers under your accounts.

## Download

| Platform | Installer |
| --- | --- |
| macOS (Apple silicon) | [AgentVera-mac-arm64.dmg](https://agentvera.dev/downloads/latest/AgentVera-mac-arm64.dmg) |
| macOS (Intel) | [AgentVera-mac-x64.dmg](https://agentvera.dev/downloads/latest/AgentVera-mac-x64.dmg) |
| Windows (x64) | [AgentVera-win-x64.exe](https://agentvera.dev/downloads/latest/AgentVera-win-x64.exe) |
| Linux (x64) | [AppImage](https://agentvera.dev/downloads/latest/AgentVera-linux-x86_64.AppImage) · [.deb](https://agentvera.dev/downloads/latest/AgentVera-linux-amd64.deb) |

The app updates itself. Core features are free with unlimited agents; Pro and Team plans add flows, the pipeline, night shift, auto approval, account switching, the database manager and team features. [Compare plans →](https://agentvera.dev/en/pricing/)

## Alternatives and comparisons

Looking at Conductor, Vibe Kanban, Claude Squad, Nimbalyst or Superset? See the side-by-side comparisons at [agentvera.dev/en/alternatives](https://agentvera.dev/en/alternatives/).

## Changelog

What changed in each release: [CHANGELOG.md](CHANGELOG.md).

## Feedback

- **Bug or crash:** [open an issue](../../issues/new?template=bug.yml)
- **Idea or missing agent:** [request a feature](../../issues/new?template=feature.yml)

---

## Türkçe

**AgentVera; Claude Code, Codex, Gemini CLI, Copilot ve 14 kodlama ajanını daha macOS, Windows ve Linux'ta yan yana çalıştıran bir masaüstü uygulaması.** Her ajan bilgisayarındaki kendi CLI'ıyla ve kendi hesabınla, gerçek bir terminalde çalışır; Claude ya da ChatGPT aboneliğin olduğu gibi kullanılır, API anahtarı gerekmez. AgentVera aralarındaki işi yönetir: düzenler, git worktree'ler, akışlar, kod incelemesi, limitler ve token tasarrufu.

**0.7 ile ajan ekipleri geldi:** çalışma alanındaki ajanlardan bir yönetici ve ekip kurarsın, her ajana rol verir, kimin kime iş devredeceğini çizersin. Tek bir istek yazarsın; yönetici işi böler, ekip işi birbirine devreder, sen de ekip görünümünden her ajanın ne yaptığını, hangi adımda olduğunu izler, izinleri kartın üstünden verirsin. Ayrıca her CLI için oturum açarak hesap ekleme, akışlarda HTTP/Telegram/e-posta adımları, dosya ağacında sağ tık menüsü ve telefondan uzaktan kontrol var.

[Türkçe site](https://agentvera.dev/) · [İndir](https://agentvera.dev/indir/) · [Özellikler](https://agentvera.dev/ozellikler/) · [Fiyatlar](https://agentvera.dev/fiyatlar/) · [Alternatifler](https://agentvera.dev/alternatifler/)

Hata ve önerilerini bu depodaki Issues bölümüne yazabilirsin.

---

<sub>AgentVera is built by <a href="https://solviera.com.tr">Solviera Teknoloji</a>. Claude, Codex, Gemini and other names are trademarks of their owners; AgentVera is not affiliated with them.</sub>
