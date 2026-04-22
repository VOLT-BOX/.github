# AI Agent Guidelines
> AI Agent Guidelines, Maintained by @erbanku and Fellow AI Agents.

## CHANGELOG (mandatory)

After completing work in this repository, **add or update** the root [CHANGELOG.md](CHANGELOG.md). Conventions:

- **One `## MM/DD/YYYY` H2 per calendar day** (US month/day/year), **newest day first** below the title and attribution line.
- Under that day, add bullet points for **finished** work (user-visible changes, features, bug fixes, refactors, documentation, or infrastructure) that belong in a release history.
- If a section for that calendar day **already exists**, **append** bullets to it; do **not** add a second H2 for the same date.
- If [CHANGELOG.md](CHANGELOG.md) is missing, create it with the same pattern as other sibling repos: `# Changelogs for .github`, the `> Created and Maintained by @erbanku and fellow AI agents` line, then date sections (newest first).

**Mandatory:** every AI agent working in this repository must update the changelog when completing a task here.

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

