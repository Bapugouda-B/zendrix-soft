# Project Details/Workflow
 
This repository demonstrates the Gitflow workflow for managing monthly product releases.

## GitHub Repository Link
Click Here To View
[Zendriix Software Git Workflow](https://github.com/Bapugouda-B/zendrix-soft)


## Branches

- **master**: Production-ready code.
- **develop**: Latest completed development code.
- **feature/xyz**: Individual feature branches.
- **QA**: Branch for final testing and bug fixing before release.
- **hotfix/xyz**: Branch for critical production bug fixes.

## Workflow Steps

1. **Feature Development**:
    - Create a feature branch from `develop`.
    - Work on the feature and commit changes.
    - Merge the feature branch back into `develop`.

2. **Preparing for Release**:
    - Create a QA and UAT branch from `develop`.
    - Perform final testing and bug fixes on QA and UAT branch.
    - After QA and UAT Verify Merge the release branch into `master` and `develop`.

3. **Hotfixes**:
    - Create a hotfix branch from `master` if a critical bug is found in production.
    - Fix the bug and merge the hotfix branch back into `master` and `develop`.

## Simulated Workflow

### Initialize a Git Repository
```bash
mkdir zendriix-software
cd zendriix-software
git init
echo "# Zendriix Software" > README.md
git add README.md
git commit -m "Initial commit"
git branch -M master
