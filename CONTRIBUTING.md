# Contributing Guide

## Branches
- `main` is always stable. Never commit directly to it.
- Use a prefix: `feature/`, `fix/`, `docs/`, `test/`, `chore/`.
- Example: `feature/ticket-creation`

## Commit messages
Format: `type: short description`
Types: feat, fix, docs, test, chore, ci, refactor
Example: `test: add negative tests for ticket priority`

## Pull requests
- One purpose per PR.
- Describe what changed and how it was tested.
- Link the related requirement or defect where one exists.

## Data safety
- Never commit passwords, tokens, `.env` files, or real company data.
- Use fake test data only.