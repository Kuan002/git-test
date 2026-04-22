# Git Setup & Workflow Log (Clean Version)

# 1. Configure Git

```bash
git config --global user.name "<username>"
git config --global user.email "<email>"
```

--- 

# 2. Create Project

```bash
cd ~/Desktop
mkdir git-test
cd git-test
git init
```

--- 

# 3. Add First File

```bash
echo "hello git" > test.txt
git add .
git commit -m "test: initial commit"
```

--- 

# 4. Set Branch

```bash
git branch -M main
```

--- 

# 5. Connect to GitHub

```bash
git remote add origin git@github.com:<username>/git-test.git
```

--- 

# 6. Setup SSH Key

```bash
ssh-keygen -t ed25519 -C "<email>"
cat ~/.ssh/id_ed25519.pub
ssh -T git@github.com
```

--- 

# 7. First Push

```bash
git push -u origin main
```

--- 

# 8. Add Documentation File

```bash
touch git-command.md
git add .
git commit -m "docs: add git commands cheat sheet"
git push
```

--- 

# 9. Improve Documentation

```bash
git add .
git commit -m "docs: improve git command notes"
git push
```

--- 

# 10. Add More Notes

```bash
git add .
git commit -m "docs: add git add variations"
git push
```

--- 

# 11. Sync Changes from Remote

```bash
git pull
```

--- 

# 12. Handle File Rename (from remote)

```bash
git pull
```

--- 

# 13. Add Setup & Workflow Guide

```bash
touch git-setup-and-workflow.md
git add git-setup-and-workflow.md
git commit -m "docs: add git setup and workflow guide"
git push
```

--- 

# 14. Update Setup Guide

```bash
git add git-setup-and-workflow.md
git commit -m "docs: modify setup and workflow guide"
git push
```

--- 

# 15. View Logs

```bash
git log
git log --oneline
git log -p
```

--- 

# 16. Inspect Commit

```bash
git show <commit-id>
```

--- 

# Notes
 - SSH authentication configured
 - Repository successfully pushed and tracked
 - Documentation updated incrementally
 - Remote changes synchronized locally
