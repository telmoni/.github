# Telmoni

Telmoni is building privacy-first observability for AI agents: every run and the steps inside it, every model and tool call with its tokens, latency and cost, and an alert when an agent stalls, loops, fails or overspends. It keeps them as metadata, leaving prompts and completions out unless a project turns them on.

What exists today: the foundation — organizations and projects, members and roles, API keys, notifications, a hash-chained audit log and a console agent, run by one Rust binary and a Next.js console — and the first of the telemetry on it: SDKs in four languages that record an agent's runs, a plugin each for Claude Code, Codex, OpenCode and Cursor that records the coding agent's own turns, ingest, which keeps each run as metadata with prompts and completions dropped at the door, and a console that reads them as traces, sessions and users. Alerts are not built yet, and Telmoni has not launched.

| Repository | What it holds |
|---|---|
| [`telmoni`](https://github.com/telmoni/telmoni) | The platform: the server, the console, the four SDKs (Python, TypeScript, Go, Rust), and the Docker Compose file and Helm chart for self-hosting |
| [`docs`](https://github.com/telmoni/docs) | The documentation, which the console builds in and serves at `/docs`: [telmoni.com/docs](https://telmoni.com/docs) |
| [`telmoni-cli`](https://github.com/telmoni/telmoni-cli) | `telmoni`, the command-line client |
| [`skills`](https://github.com/telmoni/skills) | Agent skills that teach coding agents (Claude Code, Codex, Cursor and others) to work with Telmoni: the SDKs, the coding-agent plugins, the CLI, the API, webhooks and self-hosting |
| [`claude-observability-plugin`](https://github.com/telmoni/claude-observability-plugin), [`codex-observability-plugin`](https://github.com/telmoni/codex-observability-plugin), [`opencode-observability-plugin`](https://github.com/telmoni/opencode-observability-plugin), [`cursor-observability-plugin`](https://github.com/telmoni/cursor-observability-plugin) | A plugin each that records a coding agent's own turns in Telmoni as runs, metadata only: the models and their tokens, the tools, the subagents and the times, never a prompt, a reply or a file |

All eight are Apache-2.0. [Contributing](https://telmoni.com/docs/contributing/introduction) · [Support](https://github.com/telmoni/.github/blob/main/SUPPORT.md) · [Security](https://telmoni.com/docs/legal/security#reporting-a-vulnerability)
