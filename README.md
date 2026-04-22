# Git Test Repository

## Overview
This repository demonstrates a complete Git workflow, including installation, GitHub account setup, SSH authentication, and basic version control operations using Git.

---

## Features
- Git installation and configuration
- GitHub account creation
- SSH key authentication
- Repository initialization and push
- Basic Git workflow (add, commit, push, pull)

---

## Prerequisites
```bash
- Windows / macOS / Linux
- Internet connection
```

## 1. Install Git
```bash
# Check if Git is installed
git --version

# If not installed (Windows)
Download from: https://git-scm.com/downloads

# Verify installation
git --version
```

## 2. Create GitHub Account
```bash
# Go to GitHub website
https://github.com/

# Steps:
# 1. Click "Sign up"
# 2. Enter email, username, password
# 3. Verify email
# 4. Complete account setup
```

## 3. Configure Git Identity
```bash
git config --global user.name "<your-username>"
git config --global user.email "<your-email>"
```

## 4. Create Local Repository
```bash
cd ~/Desktop
mkdir git-test
cd git-test
git init
```

## 5. First Commit
```bash
echo "hello git" > test.txt

git add .
git commit -m "test: initial commit"
```

## 6. Set Main Branch
```bash
git branch -M main
```

## 7. Create Repository on GitHub
```bash
# Steps:
# 1. Click "New Repository"
# 2. Repository name: git-test
# 3. Set to Public or Private
# 4. Do NOT initialize with README
# 5. Click "Create repository"
```

## 8. Connect to GitHub
```bash
git remote add origin git@github.com:<your-username>/git-test.git
```

## 9. Setup SSH Authentication
```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "<your-email>"

# Test connection
ssh -T git@github.com
# Add SSH key to GitHub:
# 1. Go to Settings
# 2. SSH and GPG keys
# 3. Click "New SSH key"
# 4. Paste content from ~/.ssh/id_ed25519.pub
```

## 10. Push to GitHub
```bash
git push -u origin main
```

## 11. Daily Workflow
```bash
git add .
git commit -m "message"
git push
```

## Useful Commands
```bash
git status
git log --oneline
git log -p
git show <commit-id>
git diff
git diff --staged
git pull
```

## Notes
- SSH authentication configured successfully
- Repository successfully pushed to GitHub
- Workflow includes commit tracking and remote synchronization
- Documentation maintained in git-notes.md and git-setup-and-workflow.md
