<div align="center">
  <h1>
    <div style="display: inline-flex; align-items: center; gap: 4px;">
      <img src="https://www.asteroidstudio.org/logo.svg" alt="Asteroid Studio" height="25px" />
    </div>
  </h1>
  <p>Welcome to the <a target="_blank" href="https://www.asteroidstudio.org">Asteroid Studio</a> team. This is our internal landing page with a quick map of how we work, where things live, and how to get unblocked fast.</p>
</div>

> This page is only visible to members of the **Asteroid Studio** organization.

---

## 🚀 Getting Started

New here? Work through this list:

1. **Set up your accounts**: make sure 2FA is enabled on your GitHub account (required for org membership).
2. **Join the team channels**: ask your lead for invites to our communication and project-management spaces.
3. **Get repo access**: access is managed through GitHub Teams. If you're missing a repo, ask your lead rather than requesting individual access.
4. **Read the engineering conventions** below before opening your first PR.

## 🗂 Key Repositories

| Repository        | What it is                                            |
| ----------------- | ----------------------------------------------------- |
| `.github`         | Public org profile, shared community health files     |
| `.github-private` | This repo: internal docs and the page you're reading |

### Public Repositories

<!-- public-repos:start -->

| Repository | Description |
| --- | --- |
| [.github](https://github.com/asteroidorg/.github) |  |
| [asteroid-nepali-date-utils](https://github.com/asteroidorg/asteroid-nepali-date-utils) |  |
| [cms-core-utils](https://github.com/asteroidorg/cms-core-utils) | Seamless integration utilities for Asteroid CMS - Apollo provider, content hooks, and rich-text rendering. |

<!-- public-repos:end -->

> This table is regenerated automatically by the [`update-repo-list`](https://github.com/asteroidorg/.github-private/blob/main/.github/workflows/update-repo-list.yml) workflow. Don't edit it by hand; your changes will be overwritten.

## 🛠 Engineering Conventions

📖 **Full guidelines:** [CONTRIBUTING.md](https://github.com/asteroidorg/.github-private/blob/main/CONTRIBUTING.md) covers branch naming, commit messages, PRs, issues, and code review. It's generic by design, so copy it into any new project.

The short version:

- **Branches**: branch from `main`, use descriptive names: `feat/...`, `fix/...`, `chore/...`
- **Commits**: follow [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, `refactor:`, ...)
- **Pull requests**: keep them small and focused; every PR needs at least one review before merge
- **Secrets**: never commit credentials. Use the org's secret management; if something leaks, rotate it immediately and tell your lead
- **CI**: don't merge red. If a check is flaky, fix or flag it, don't bypass it

## 🔐 Security & Access

- Report security concerns privately to your lead, never in a public issue.
- Production access and deploy permissions are granted per-project; ask your lead.
- Off-boarding: leads are responsible for removing access when someone leaves a project.

## 🙋 Who to Ask

| Topic                    | Contact               |
| ------------------------ | --------------------- |
| GitHub org / repo access | Org admins            |
| Project questions        | Your project lead     |
| Security issues          | Your lead (privately) |

---

<sub>Maintained by the Asteroid Studio team · Edit this page in <a href="https://github.com/asteroidorg/.github-private">asteroidorg/.github-private</a></sub>
