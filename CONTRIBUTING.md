# Contributing to phos-org

These conventions apply to every phos-org project. Each project's own
`CONTRIBUTING.md` adds what is specific to it (how to run it, how its code is
laid out) and takes precedence where the two differ.

## Issues

- Search first; add to an existing issue rather than opening a duplicate.
- Use the project's issue forms. One problem or idea per issue.
- Say in the issue that you are working on it, so nobody duplicates the work.
- Security problems never go in an issue: see [SECURITY.md](SECURITY.md).

## Branches

`main` is protected and always releasable: changes arrive through pull
requests, squash-merged, so its history is linear. Work on a branch named
`<type>/<short-description>`, lowercase: `feat/weather-alerts`,
`fix/stack-rotation`, `docs/install-debian`.

## Commits and pull request titles

[Conventional Commits](https://www.conventionalcommits.org):
`<type>(<optional scope>): <description>`, at most 72 characters, imperative,
no full stop. Types: `feat`, `fix`, `refactor`, `perf`, `docs`, `test`,
`build`, `ci`, `chore`, `style`, `revert`. A breaking change takes a `!`.

The pull request title becomes the commit on `main`, so it follows the same
rules. Commits describe the change: no AI-tool attribution trailers or
session links; credit people with `Co-Authored-By` as usual.

Projects ship the checks as git hooks: `git config core.hooksPath .githooks`.

## Pull requests

- Small and focused: one change per pull request; code and its docs together.
- Linked to its issue (`Fixes #12`), with how you checked it and a
  screenshot for anything visible.
- Required checks green, conversations resolved, then squash-merged.

## Privacy is a feature

Tools that read personal data keep it local and read-only, read only what
they show, and document it. Nothing may send data anywhere a user would not
expect.

## Code of conduct

Everyone taking part follows the [Code of Conduct](CODE_OF_CONDUCT.md).
