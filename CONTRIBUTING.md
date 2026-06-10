# Contributing Guidelines

<!--toc:start-->

- [Getting Started](#getting-started)
- [Contribution Workflow](#contribution-workflow)
- [Branch Naming Guidelines](#branch-naming-guidelines)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Issue Guidelines](#issue-guidelines)
- [Code Review Guidelines](#code-review-guidelines)
<!--toc:end-->

> Engineering guidelines for Asteroid Studio projects, independent of language or tooling.

## Getting Started

Setup, build, and run instructions are project-specific; see the project's `README.md` for the exact commands. Every project should document at least:

- **Install**: how to install dependencies and prerequisites
- **Run**: how to start the project locally (development mode)
- **Build**: how to produce a production build or release artifact
- **Check**: how to run the linter, formatter, type checker, and tests

Before opening a pull request, all of the project's checks must pass locally.

<!--
When copying this file into a project, you may replace the section above
with the project's actual commands, e.g.:

### Run the development server

```bash
pnpm dev
```

### Run checks

```bash
pnpm lint && pnpm tsc:check && pnpm test
```
-->

## Contribution Workflow

1. **Clone the Repository**: Clone the repository to your local machine (fork first if you don't have write access).

2. **Create a New Branch**: Always create a new branch for your changes; never commit directly to `main`. This keeps the project history clean and easy to navigate.

3. **Make Your Changes**: Make your changes in the new branch. Follow the coding standards and conventions used throughout the project.

4. **Test Your Changes**: Before submitting your changes, make sure all of the project's checks (lint, tests, build) pass locally.

5. **Commit Your Changes**: Commit your changes with a clear and concise commit message following the [Commit Message Guidelines](#commit-message-guidelines).

6. **Push Your Changes**: Push your branch to the remote repository.

7. **Submit a Pull Request**: Open a pull request against `main` following the [Pull Request Guidelines](#pull-request-guidelines).

## Branch Naming Guidelines

Use lowercase, hyphen-separated names prefixed with the type of change:

```text
<type*>/<short-description*>/<ticket-number?>
```

Examples:

- `feat/user-authentication/223`
- `hotfix/navbar-overflow`
- `docs/api-usage-examples`
- `chore/upgrade-dependencies`

## Commit Message Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification for our commit messages. This leads to more readable messages that are easy to follow when looking through the project history, and enables automated changelogs and versioning.

A commit message should be structured as follows:

```gitcommit
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

Where `type` must be one of the following:

| Type       | Description                                                                                       |
| ---------- | ------------------------------------------------------------------------------------------------- |
| `feat`     | A new feature                                                                                     |
| `fix`      | A bug fix                                                                                         |
| `hotfix`   | A bug fix required for immediate deployment                                                       |
| `quickfix` | Small bug fix that doesn't require a new version                                                  |
| `docs`     | Documentation only changes                                                                        |
| `style`    | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons) |
| `refactor` | A code change that neither fixes a bug nor adds a feature                                         |
| `perf`     | A code change that improves performance                                                           |
| `test`     | Adding missing tests or correcting existing tests                                                 |
| `chore`    | Changes to the build process or auxiliary tools and libraries                                     |

Additional rules:

- Use the imperative mood in the description: "add login page", not "added login page".
- Keep the first line under 72 characters.
- Add a `!` after the type/scope (e.g. `feat!:`) or a `BREAKING CHANGE:` footer for breaking changes.
- Reference issues in the footer when applicable: `Closes #123`.

Examples:

```gitcommit
feat(auth): add OAuth2 login flow
fix(api): handle empty response from CMS endpoint
docs: update environment setup instructions
chore!: drop support for legacy runtime versions
```

## Pull Request Guidelines

Follow the same naming convention for your pull request titles as you do for your commits (e.g. `feat(auth): add OAuth2 login flow`). Keep pull requests small and focused on a single change.

1. **Reference Related Issues**: If your pull request is related to an existing issue, reference it in your PR description (e.g. `Closes #123`).

2. **Describe Your Changes**: Provide a clear and detailed description of what changes you've made and why.

3. **Include Screenshots**: If your changes include UI updates, include before/after screenshots or a short recording in your PR description.

4. **Keep CI Green**: Make sure all checks (lint, types, tests, build) pass before requesting review. Don't merge with failing checks.

5. **Wait for Review**: After submitting your PR, wait for it to be reviewed and approved before merging. At least one approval is required.

6. **Keep It Up to Date**: Resolve conflicts by rebasing or merging `main` into your branch before merge.

## Issue Guidelines

When opening an issue, make it actionable for whoever picks it up:

1. **Search First**: Check existing issues (open and closed) to avoid duplicates.

2. **Use a Clear Title**: Summarize the problem or request in one line, e.g. `Bug: image upload fails for files > 5MB`.

3. **Bug Reports** should include:
   - Steps to reproduce
   - Expected behavior vs. actual behavior
   - Environment details (OS, browser, runtime/tool versions) where relevant
   - Screenshots, logs, or error messages

4. **Feature Requests** should include:
   - The problem you're trying to solve (not just the solution)
   - The proposed solution or behavior
   - Any alternatives you've considered

5. **One Issue per Issue**: Don't bundle multiple unrelated problems into a single issue.

## Code Review Guidelines

For authors:

- Review your own diff before requesting a review.
- Respond to every comment: either make the change or explain why not.
- Don't take feedback personally; it's about the code, not you.

For reviewers:

- Be respectful and constructive; suggest, don't demand.
- Distinguish blocking issues from nitpicks (prefix optional comments with `nit:`).
- Review promptly; aim to respond within one working day.
- Approve once concerns are addressed; don't let PRs go stale.
