# Contributing to Hybrid Forge Lab projects

Thanks for taking the time to help. This guide applies to every public repository in the
[hybridforgelab](https://github.com/hybridforgelab) organization, unless a repository has its own `CONTRIBUTING.md`.

*Português: as contribuições são bem-vindas em português ou em inglês. Este guia está em inglês para servir toda a
gente.*

## Before you start

- **Bugs and ideas:** open an issue first, using the templates. For a small, obvious fix (a typo, a broken link) a pull
  request on its own is fine.
- **A problem with one of our paid APIs** (Distill, Shipshape, Luz Indexada…), not with the code in a repository:
  use the [contact page](https://hybridforgelab.com/contact.html) instead. API support doesn't happen in these issues.
- **Security issues:** never in a public issue. See [SECURITY.md](SECURITY.md).

## Making a change

1. Fork the repository and create a branch from `main`.
2. Set it up as the **Development** section of that repository's README describes (install, run, test).
3. Keep the change focused: one pull request per fix or feature.
4. Add or update tests for what you change. Tests and linting must pass locally before you open the pull request;
   the same checks run in CI (for example `pytest` and `ruff check .` in our Python projects; the Home Assistant
   integration also runs the HACS and hassfest validations).
5. Update the README if behaviour, options or setup change.
6. Open the pull request and fill in the template.

## Commit and pull request titles

We use [Conventional Commits](https://www.conventionalcommits.org/): `type: description`, in the imperative, lower
case, no full stop.

| type | when |
|---|---|
| `feat` | a new feature |
| `fix` | a bug fix |
| `docs` | documentation only |
| `test` | tests only |
| `refactor` | code change that neither fixes a bug nor adds a feature |
| `ci`, `chore` | build, CI, tooling, dependencies |

Examples: `fix: handle the autumn DST day (100 quarter-hours)`, `docs: explain the API usage limits`.
Where a repository uses release-please, these titles decide the next version and the changelog, so please follow
them. Pull requests are squash-merged, so the pull request title becomes the commit message.

## Review

- A maintainer reviews every pull request. We may ask for changes, and we may close changes that don't fit the
  project's scope; we'll always say why.
- Please be patient: this is a small team.
- Everyone taking part follows our [Code of Conduct](CODE_OF_CONDUCT.md).

## Licence

Our public repositories are MIT-licensed. By contributing, you agree that your contribution is licensed under the
licence of the repository you contribute to.
