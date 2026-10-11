# Telmoni

Telmoni is building privacy-first telemetry and monitoring for AI agents: every run and the steps inside it, every model and tool call with its tokens, latency and cost, and an alert when an agent stalls, loops, fails or overspends. It keeps them as metadata, leaving prompts and completions out unless a project turns them on.

What exists today: the foundation — organizations and projects, members and roles, API keys, notifications, a hash-chained audit log and a console agent, run by one Rust binary behind a Next.js console — and the first of the telemetry on it: SDKs in four languages that record an agent's runs and send them to ingest, which keeps each as metadata with prompts and completions dropped at the door, and a console that reads them as traces, conversations and users. Monitors and alerts are not built yet, and Telmoni has not launched.

| Repository | What it holds |
|---|---|
| [`telmoni`](https://github.com/telmoni/telmoni) | The platform: the server, the console, the four SDKs (Python, TypeScript, Go, Rust), the documentation it serves at [telmoni.com/docs](https://telmoni.com/docs), and the Docker Compose file and Helm chart for self-hosting |
| [`telmoni-cli`](https://github.com/telmoni/telmoni-cli) | `telmoni`, the command-line client |
| [`skills`](https://github.com/telmoni/skills) | Agent skills that teach coding agents (Claude Code, Codex, Cursor and others) to work with Telmoni: the SDKs, the CLI, the API, webhooks and self-hosting |

All three are Apache-2.0. [Contributing](https://telmoni.com/docs/contributing/introduction) · [Support](https://github.com/telmoni/.github/blob/main/SUPPORT.md) · [Security](https://telmoni.com/docs/legal/security#reporting-a-vulnerability)
