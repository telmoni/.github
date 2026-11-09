<picture>
  <source media="(prefers-color-scheme: dark)" srcset="logo-white.svg">
  <img src="logo.svg" alt="Telmoni" width="320">
</picture>

## What is Telmoni?

**Privacy-first, open-source monitoring for AI agents.** Know when your agents fail, stall, loop or overspend, and stop them at the cap you set. Prompts stay in your process unless you turn content on.

Telmoni watches the agents you run, whether a Python service, a nightly batch, a LangGraph graph or a Claude Code session. It alerts you when a run fails, loops on one tool, is left open, costs past its cap, or when runs stop arriving, and shows you the run that did it. The SDKs' guard stops a run at the caps on its steps and spend, inside your own process. Telemetry is metadata by default; prompts, replies, tool calls and images are kept in full only where a project's owner turns content on and your code asks for it, sealed under that project's own key.

## WARNING

Telmoni is still in the early stages of development. Until it is, expect it to change every month: better each time, and sometimes incompatibly, as names, endpoints and console pages move while we find out what works.
 

| Repository | What it holds |
|---|---|
| [`telmoni`](https://github.com/telmoni/telmoni) | The platform: the server, the console, the four SDKs (Python, TypeScript, Go, Rust), the documentation the console serves at `/docs` ([telmoni.com/docs](https://telmoni.com/docs)), and the Docker Compose file and Helm chart for self-hosting |
| [`claude-code-observability-plugin`](https://github.com/telmoni/claude-code-observability-plugin) | The Claude Code plugin, which records Claude Code's own turns in Telmoni as runs: the models and their tokens, the tools, the subagents and the times, and the conversation only where you turn content on. |
| [`codex-observability-plugin`](https://github.com/telmoni/codex-observability-plugin) | The Codex plugin, which records Codex's own turns in Telmoni as runs: the models and their tokens, the commands, edits and other tools, the compactions and the times, and the conversation only where you turn content on. |
| [`antigravity-observability-plugin`](https://github.com/telmoni/antigravity-observability-plugin) | The Antigravity plugin, which records Antigravity's own turns in Telmoni as runs: the models and their tokens, the tools, the compactions and the times, and the conversation only where you turn content on. |
| [`telmoni-cli`](https://github.com/telmoni/telmoni-cli) | `telmoni`, the command-line client: sign in from a terminal or CI, see who you are, and switch organizations |

All five are Apache-2.0. [Contributing](https://telmoni.com/docs/contributing/introduction) · [Support](https://github.com/telmoni/.github/blob/main/SUPPORT.md) · [Security](https://telmoni.com/docs/legal/security#reporting-a-vulnerability)
