# Telmoni

Telmoni is building privacy-first observability for AI agents: every run and the steps inside it, every model and tool call with its tokens, latency and cost, and an alert when an agent stalls, loops, fails or overspends. It keeps them as metadata, leaving prompts and completions out unless a project turns them on.

Telmoni has not launched and is not at 1.0. Until it is, expect it to change every month: better each time, and sometimes incompatibly, as names, endpoints and console pages move while we find out what works. Not everything above is built yet; alerts, for one, are not.

| Repository | What it holds |
|---|---|
| [`telmoni`](https://github.com/telmoni/telmoni) | The platform: the server, the console, the four SDKs (Python, TypeScript, Go, Rust), the documentation the console serves at `/docs` ([telmoni.com/docs](https://telmoni.com/docs)), and the Docker Compose file and Helm chart for self-hosting |
| [`telmoni-cli`](https://github.com/telmoni/telmoni-cli) | `telmoni`, the command-line client |
| [`skills`](https://github.com/telmoni/skills) | Agent skills that teach coding agents (Claude Code, Codex, Cursor and others) to work with Telmoni: the SDKs, the coding-agent plugins, the CLI, the API, webhooks and self-hosting |
| [`claude-observability-plugin`](https://github.com/telmoni/claude-observability-plugin), [`codex-observability-plugin`](https://github.com/telmoni/codex-observability-plugin), [`opencode-observability-plugin`](https://github.com/telmoni/opencode-observability-plugin), [`cursor-observability-plugin`](https://github.com/telmoni/cursor-observability-plugin) | A plugin each that records a coding agent's own turns in Telmoni as runs, metadata only: the models and their tokens, the tools, the subagents and the times, never a prompt, a reply or a file |

All seven are Apache-2.0. [Contributing](https://telmoni.com/docs/contributing/introduction) · [Support](https://github.com/telmoni/.github/blob/main/SUPPORT.md) · [Security](https://telmoni.com/docs/legal/security#reporting-a-vulnerability)
