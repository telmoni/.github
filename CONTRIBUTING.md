# Contributing to Telmoni

Thanks for helping build Telmoni. Everyone taking part follows the [Code of Conduct](https://github.com/telmoni/.github/blob/main/CODE_OF_CONDUCT.md).

## The repositories

Each repository's README says how to set it up, and its `ARCHITECTURE.md` explains how it is built: read it before changing anything structural.

| Repository | The gate |
|---|---|
| [`telmoni/telmoni`](https://github.com/telmoni/telmoni): the platform, the four SDKs (`sdk/`) and the docs | `make ci` |
| [`telmoni/telmoni-cli`](https://github.com/telmoni/telmoni-cli): the CLI | `cargo xtask ci` |
| The [Claude Code](https://github.com/telmoni/claude-code-observability-plugin), [Codex](https://github.com/telmoni/codex-observability-plugin) and [Antigravity](https://github.com/telmoni/antigravity-observability-plugin) plugins | `npm run verify` and `npm run validate` |

The gate is what CI runs; a pull request is reviewed once it passes. The Antigravity plugin's CI cannot run `validate`, so run it yourself before you push.

## Before you start

Open an issue first for a new feature, a schema change or anything architectural, so the shape is agreed before the work. A bug fix or a small improvement can go straight to a pull request.

## Commits and pull requests

- Keep a pull request to one change.
- Commits follow [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, `refactor:`, `chore:`).
- Every commit is signed off by its author: `git commit -s` adds `Signed-off-by: Your Name <you@example.com>`, certifying the [Developer Certificate of Origin](https://developercertificate.org/): that you may submit the change under the project's Apache-2.0 licence. A pull request with a commit not signed off is sent back to be signed.

## AI policy

Use whatever tools help you, AI among them. The one rule: **understand every line you submit.** Whatever drafted a change, it is yours once you open the pull request: know what it does and why, and be ready to explain it and answer a reviewer's questions yourself. A change its author can't explain is sent back, however good it looks.

## Security

A suspected vulnerability is never a public issue: see the [security policy](https://github.com/telmoni/.github/blob/main/SECURITY.md).
