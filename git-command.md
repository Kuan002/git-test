# Git Commands Cheat Sheet

## Basic Workflow
- git init → Initialize repository
- git add . → Add all files to staging
- git commit -m "message" → Commit changes
- git push → Push to remote repository

## Status & Info
- git status → Check current changes
- git log --oneline → View commit history

## Remote
- git remote add origin <repo-url> → Link to GitHub
- git push -u origin main → First push
- git pull → Get latest changes

## Branching
- git branch → List branches
- git checkout -b feature/test → Create new branch
- git checkout main → Switch branch
- git merge feature/test → Merge branch

## Undo
- git checkout -- file → Discard changes
- git reset file → Unstage file
- git reset --hard HEAD~1 → Reset commit (dangerous)

## Notes
- SSH key configured for GitHub access
- Successfully pushed first repository