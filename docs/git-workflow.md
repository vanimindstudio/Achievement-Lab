# Git Workflow Guide

Standard development workflow for Achievement-Lab.

## 1. Branch Strategy

The `main` branch contains the stable version of the project.

All changes should be developed in separate branches.

| Branch         | Purpose                       |
| :------------- | :---------------------------- |
| `main`         | Stable project version        |
| `feature/*`    | New features and improvements |
| `docs/*`       | Documentation updates         |
| `fix/*`        | Bug fixes                     |
| `experiment/*` | GitHub experiments            |

## 2. Creating a Branch

Create a new branch before making changes.

```bash
git checkout main
git pull origin main
git checkout -b docs/update-roadmap
```

## 3. Making Changes

After editing files, inspect the changes:

```bash
git status
git diff
```

Stage the files:

```bash
git add .
```

## 4. Commit Convention

Use clear and descriptive commit messages.

| Prefix      | Purpose            |
| :---------- | :----------------- |
| `feat:`     | New features       |
| `fix:`      | Bug fixes          |
| `docs:`     | Documentation      |
| `refactor:` | Code restructuring |
| `chore:`    | Maintenance        |
| `test:`     | Tests              |

Example:

```bash
git commit -m "docs: update achievement roadmap"
```

## 5. Pull Request Workflow

1. Push your branch to GitHub.
2. Open a Pull Request targeting `main`.
3. Describe the changes.
4. Review the changes.
5. Merge the Pull Request.
6. Delete the merged branch if it is no longer needed.

```bash
git push -u origin docs/update-roadmap
```

## 6. Synchronizing Main

After merging a Pull Request:

```bash
git checkout main
git pull origin main
```

## 7. Laboratory Rules

- Keep `main` stable.
- Use descriptive branch names.
- Write meaningful commit messages.
- Avoid unnecessary commits.
- Keep documentation updated.
- Never create artificial activity just to increase achievement counts.
- Prefer real collaboration and meaningful contributions.

## 8. Achievement Experiments

Achievement-Lab is also an environment for learning GitHub features.

Experiments may include:

- Issue creation and management.
- Pull Request creation and merging.
- Code reviews.
- GitHub Discussions.
- Collaborative commits.
- Repository maintenance.

---

**Project:** Achievement-Lab  
**Maintainer:** Vanimind Studio

_Experiment. Develop. Achieve._
