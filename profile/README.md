<picture>
  <source media="(prefers-color-scheme: dark)" srcset="logo-white.svg">
  <img src="logo.svg" alt="Telmoni" width="320">
</picture>

## What is Telmoni?

**Privacy-first, open-source monitoring for AI agents.** Know when your agents fail, stall, loop or overspend, and stop them at the cap you set. Prompts stay in your process unless you turn content on.

Telmoni watches the agents you run, whether a Python service, a nightly batch, a LangGraph graph or a Claude Code, Codex or Antigravity session. Use the SDKs in [`telmoni`](https://github.com/telmoni/telmoni) to instrument your own agents, or install a coding-agent plugin to record each turn of Claude Code, Codex or Antigravity as a run, with its model calls, tokens, tools, timings and outcome, with no code to write.

It alerts you when a run fails, loops on one tool, is left open, costs past its cap, or when runs stop arriving, and shows you the run that did it. The SDKs' guard stops a run at the caps on its steps and spend, inside your own process. Telemetry is metadata by default; prompts, replies, tool calls and images are kept in full only where a project's owner turns content on and you enable capture in your code or plugin, sealed under that project's own key.

Telmoni is self-hosted: you run it yourself with Docker Compose or Helm. There is no hosted service.

> [!WARNING]
> Telmoni is early and changes often: names, endpoints and console pages still move, sometimes incompatibly.

| Repository | What it holds |
|---|---|
| [`telmoni`](https://github.com/telmoni/telmoni) | The platform: the server, the console, the four SDKs (Python, TypeScript, Go, Rust), the documentation, and the Docker Compose file and Helm chart for self-hosting |
| [`claude-code-observability-plugin`](https://github.com/telmoni/claude-code-observability-plugin) | The Claude Code plugin: records Claude Code's turns as runs, with the models and their tokens, the tools, the subagents and the times, and the conversation only where you turn content on |
| [`codex-observability-plugin`](https://github.com/telmoni/codex-observability-plugin) | The Codex plugin: records Codex's turns as runs, with the models and their tokens, the commands, edits and other tools, the compactions and the times, and the conversation only where you turn content on |
| [`antigravity-observability-plugin`](https://github.com/telmoni/antigravity-observability-plugin) | The Antigravity plugin: records Antigravity's turns as runs, with the models and their tokens, the tools, the compactions and the times, and the conversation only where you turn content on |
| [`telmoni-cli`](https://github.com/telmoni/telmoni-cli) | `telmoni`, the command-line client: sign in from a terminal or CI, see who you are, and switch organizations |

All five are Apache-2.0. [Contributing](https://github.com/telmoni/.github/blob/main/CONTRIBUTING.md) · [Support](https://github.com/telmoni/.github/blob/main/SUPPORT.md) · [Security](https://github.com/telmoni/.github/blob/main/SECURITY.md)
