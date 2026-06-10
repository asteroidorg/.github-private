# .github-private

Internal, members-only organization files for **Asteroid Studio**.

## What this repo does

GitHub treats this repository specially: the file at [`profile/README.md`](profile/README.md) is rendered on the [organization profile page](https://github.com/asteroidorg), but **only for members** of the organization. The public-facing profile README lives in the `.github` repo instead.

## Structure

```
.github-private/
├── README.md            # This file, explains the repo
├── CONTRIBUTING.md      # Generic contribution guidelines (copy into any project)
└── profile/
    └── README.md        # Member-only org profile page
```

## Contribution guidelines

[`CONTRIBUTING.md`](CONTRIBUTING.md) holds our standard engineering guidelines: branch naming, Conventional Commits, PR/issue rules, and code review etiquette. It's written to be project-agnostic, with no assumptions about language or tooling, so it can be copied into any new repository as-is. Project-specific setup commands belong in each project's own `README.md`.

## Editing the profile page

1. Branch from `main`.
2. Edit `profile/README.md`.
3. Open a PR; changes appear on the org profile as soon as they land on `main`.

Keep this repo **private**. Making it public would expose the internal profile content.
