# hello-world

[![CI](https://img.shields.io/github/actions/workflow/status/nitindudeja2107/hello-world/ci.yml?branch=main)](https://github.com/nitindudeja2107/hello-world/actions)
[![License](https://img.shields.io/github/license/nitindudeja2107/hello-world)](LICENSE)
[![Issues](https://img.shields.io/github/issues/nitindudeja2107/hello-world)](https://github.com/nitindudeja2107/hello-world/issues)

Light, automation-first README template for practicing GitHub Flow and wiring up CI/CD, Dependabot and workflow shortcuts.

## Quick overview
- Purpose: Practice GitHub Flow, CI, PRs and automation.
- Repo owner: nitindudeja2107

## Quick start (shortest path to run)
```bash
# clone
git clone https://github.com/nitindudeja2107/hello-world.git
cd hello-world

# recommended: use gh CLI to create a feature branch and PR quickly
gh auth status || gh auth login
git checkout -b feat/quick-start
# make changes, then
git add -A && git commit -m "feat: quick start" && git push --set-upstream origin feat/quick-start
gh pr create --fill --base main --head feat/quick-start
```

## Automation & shortcuts (what to add next)
- CI: Add `.github/workflows/ci.yml` to run tests/lints and expose a status badge.
- Dependabot: Add `.github/dependabot.yml` to auto-update deps.
- PR template: `.github/PULL_REQUEST_TEMPLATE.md` with checklist (tests, changelog, impact).
- Issue template: `.github/ISSUE_TEMPLATE/bug.md` and `feature_request.md`.
- Labels: Add consistent labels (ci, docs, chore, bug, feature) and map automation.
- GitHub CLI quick commands: use `gh pr create`, `gh pr view --web`, `gh issue create` to speed workflow.

## Useful commands (automation-friendly)
- Run tests locally: `npm ci && npm test` or `make test` (add Makefile if helpful).
- Run lints: `npm run lint` or `make lint`.
- Release: `gh workflow run release.yml --ref main` (requires a release workflow).

## Contributing (shortcuts)
- Branch naming: `feat/<short-desc>`, `fix/<short-desc>`, `chore/<desc>`.
- Commit messages: Conventional Commits (feat, fix, chore, docs).
- PR process: Create small PRs, add reviewers, link issues, use `gh pr merge --squash` after approvals.

## Minimal recommended files to add (automation-ready)
- `.github/workflows/ci.yml` — CI pipeline
- `.github/dependabot.yml` — dependency updates
- `.github/PULL_REQUEST_TEMPLATE.md` — PR checklist
- `.github/ISSUE_TEMPLATE/` — templates
- `Makefile` or `package.json` scripts — standardize commands
- `LICENSE` — pick MIT/Apache/etc

## Contact / Maintainer
- Maintainer: @nitindudeja2107 (use GitHub issues or PRs for collaboration)

## License
This repository should include a LICENSE file (e.g., MIT). Add one at the root.

----

If you want, I can also create the CI workflow, PR/issue templates, and a basic Makefile in separate commits to fully automate the onboarding experience.