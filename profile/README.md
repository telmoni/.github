# Telmoni

Telmoni is building privacy-first telemetry and monitoring for AI agents: every run and the steps inside it, every model and tool call with its tokens, latency and cost, and an alert when an agent stalls, loops, fails or overspends. It keeps them as metadata, leaving prompts and completions out unless a project turns them on.

What exists today is the foundation it builds on: organizations and projects, members and roles, API keys, notifications, a hash-chained audit log and a console agent, run by one Rust binary behind a Next.js console. Nothing records an agent run yet, and Telmoni has not launched.

| Repository | What it holds |
|---|---|
| [`telmoni`](https://github.com/telmoni/telmoni) | The platform: the server, the console, and the Docker Compose file and Helm chart for self-hosting |
| [`telmoni-cli`](https://github.com/telmoni/telmoni-cli) | `telmoni`, the command-line client, and the client SDKs |
| [`docs`](https://github.com/telmoni/docs) | The source of [docs.telmoni.com](https://docs.telmoni.com) |

All three are Apache-2.0. [Contributing](https://docs.telmoni.com/contributing/introduction/) · [Support](https://github.com/telmoni/.github/blob/main/SUPPORT.md) · [Security](https://docs.telmoni.com/legal/security/#reporting-a-vulnerability)
