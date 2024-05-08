# Git Training

This repository is used for training purposes about `Trunk-based Development` workflow.

## Daily Workflow

1. Start a feature branch: Start by creating a new short-lived feature branch from the `main/trunk` branch.
```bash
git checkout -b feature/new-feature main
```
2. Work on the short-lived feature branch (< 2 days) & few file changes
3. Merge the feature branch into the `main` branch
```bash
git checkout main
git merge --no-ff feature/new-feature
git push origin main
```
4. Delete the feature branch
