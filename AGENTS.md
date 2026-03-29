# AI Agent Guidelines

## Basic Rules

1. Prohibited to add emoji in any code and documents.

## Pull Request Rules

- PR titles must follow [Conventional Commits](https://www.conventionalcommits.org/) spec.
- Format: `type(scope): subject` — scope is optional.
- Use `!` to indicate breaking changes, e.g. `refactor!: drop Node 12 support`.
- Subject must not start with an uppercase letter.

## Allowed Types

- `feat` – new feature
- `fix` – bug fix
- `chore` – maintenance / tooling
- `docs` – documentation only
- `refactor` – code restructuring
- `test` – adding or fixing tests
- `ci` – CI/CD changes

## Commit Message Rules

- Follow the same Conventional Commits format as PR titles.
- Place `BREAKING CHANGE:` in the commit footer, not the subject line.

## Work-in-Progress

- Prefix the PR title with `[WIP]` to skip validation while in draft.
- Remove `[WIP]` before requesting review.

