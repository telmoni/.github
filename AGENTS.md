# Telmoni's .github — Agent Guidelines

The organization's community files ([`telmoni/.github`](https://github.com/telmoni/.github)): the profile (`profile/README.md`) and the defaults every Telmoni repository without its own falls back to — `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `SUPPORT.md`, the pull request template and the issue forms (`.github/ISSUE_TEMPLATE/`). Most point into the book (telmoni.com/docs, `web/content/docs` in [`telmoni/telmoni`](https://github.com/telmoni/telmoni)), which holds the substance. The repository is public, and every file in it is published as written.

## Git Rules
- Commit only when asked: never `git add` or `git commit` unprompted.
- Conventional commits (`feat:`, `fix:`, `refactor:`, `docs:`, `chore:`) of 1–5 lines and the sign-off: a subject, then optionally a blank line and up to 3 lines on *why*. No file lists, test output, AI signatures or `Co-authored-by` trailers.
- Every commit is signed off by the developer it is made for, certifying the [Developer Certificate of Origin](https://developercertificate.org/): `git commit -s` adds `Signed-off-by: Name <email>` from git's `user.name` and `user.email`, which name a person, never an agent. A merge commit too: a branch is merged in a clone, `git merge --no-ff --signoff`, and pushed, never from GitHub's merge button, whose commit carries none.
- No branches, worktrees, pushes or pull requests.
