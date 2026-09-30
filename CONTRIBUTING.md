# Contributing

Thanks for taking the time to help. These defaults apply to every repository in `deadczarvc-labs` that does not ship
its own `CONTRIBUTING.md`.

## Before you start

- For a bug, open an issue with the bug form. Include the version, how you ran it and the smallest input that shows
  the problem.
- For a change in behaviour, open an issue first, so we can agree on the approach before you write code.
- Security problems go through private reporting, never a public issue. See [SECURITY.md](SECURITY.md).

## Pull requests

1. Fork the repository and branch from `main`.
2. Keep the change focused: one problem per pull request.
3. Add or update tests. The test suite must pass (`npm test` in TypeScript projects, `pytest` in Python ones).
4. When a change affects what the tool keeps, drops or measures, include the numbers before and after, and say how
   you measured them.
5. Describe what changed and why in the pull request. Link the issue it closes.

## Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org/): `<type>(<scope>): <description>`, with types such
as `feat`, `fix`, `docs`, `test`, `refactor`, `perf` and `chore`.

## Data and privacy

Never commit secrets, API keys, `.env` files or real session transcripts. Test fixtures must be synthetic or
scrubbed of personal paths, names and tokens.

## Code of conduct

Everyone taking part is expected to follow the [code of conduct](CODE_OF_CONDUCT.md).

## License

By contributing, you agree that your contributions are licensed under the license of the repository you contribute
to.
