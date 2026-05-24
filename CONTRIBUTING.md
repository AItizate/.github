# Contributing to AItizate

Thanks for showing up. Pull requests are welcome across every repo in this org.

This is the org-wide guide. Individual repos may add their own on top — when the repo-level guide says something different, that one wins.

## Before you write code

For anything bigger than a typo, open an issue first. I'd rather discuss the approach than ask you to throw away work after a review. If you're unsure whether something is worth a PR, ask in the issue — I'll tell you honestly.

## Branch and commit conventions

- Branch off `main`. Branch names: `feat/short-description`, `fix/short-description`, `docs/short-description`, `chore/short-description`, etc. Lowercase, hyphen-separated.
- Commit messages follow [Conventional Commits](https://www.conventionalcommits.org/). Most repos here run [`pr-validation-template.yml`](https://github.com/AItizate/gh-actions-templates/blob/main/.github/workflows/pr-validation-template.yml) which will tell you on the PR if a commit or the title doesn't match.

Examples that match the style:

```
feat(overlays): add bare-metal-starter validation Job
fix(ci): seed .env placeholders before kustomize build
docs(prompts): version the iteration log for ci-pipeline diagram
```

## Pull requests

1. Push your branch.
2. Open the PR against `main`. Use a Conventional Commits title.
3. Describe what changes, **why**, and what you tested. A short test plan goes a long way.
4. CODEOWNERS assigns a reviewer. One approving review to merge.
5. Stale reviews are dismissed automatically when you push new commits — re-request review when you're ready.
6. No force-pushing to `main`. No deleting `main`. The branch protection rules will block you anyway.

If your PR is a work-in-progress and you want early feedback, open it as a **draft**.

## Releases

Repos that ship versioned artifacts (notably `gh-actions-templates`) use **semver**. Breaking changes get a major version bump. Consumers pin to `@v1` to roll forward inside the major line without surprises.

See the repo's `CHANGELOG.md` for what's in each release.

## Code style

Each repo declares its own linters and formatters. Run them locally before pushing — most run in CI anyway and will fail loudly.

Two guidelines that apply everywhere:

- **No commented-out code in commits.** Either delete it or keep it.
- **No half-finished work in `main`.** Use feature flags or separate branches. If a PR adds something the platform can't use yet, the PR explains when and how it gets activated.

## Reporting issues

Bug reports: tell me what you ran, what you expected, what happened. Logs and reproduction steps beat screenshots.

Security issues: do **not** open a public issue. Open a [private security advisory](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability) on the repo where the issue lives, or reach out to the maintainer listed in `CODEOWNERS`.

## Code of conduct

Be the kind of person someone would want to collaborate with. I don't enforce a formal code of conduct because the alternative — endless rules for edge cases — usually makes things worse. If someone behaves in a way that drives others away, I talk to them directly, and if needed, ask them to leave.

## License

By contributing to a repo in this org, you agree your contribution is licensed under the same license as the repo (almost always Apache 2.0). You retain copyright; you grant the project a license to use it.

---

Thanks again. Boring tech for people who'd rather ship than argue about it.
