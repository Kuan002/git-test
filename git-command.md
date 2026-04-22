# Git Commands Cheat Sheet

## 🔧 Basic Workflow
- git init → Initialize repository（初始化仓库）
- git add . → Add all files to staging（加入暂存区）
- git commit -m "message" → Commit changes（提交代码）
- git push → Push to remote（上传到 GitHub）

---

## 🔍 Status & Info
- git status → Show working directory status（查看状态）
- git status -s → Short status（简洁模式）
- git log --oneline → View commit history（简洁查看历史）
- git log --oneline --graph --all → Visualize branches（图形化分支）

---

## 🌐 Remote (GitHub)
- git remote add origin <url> → Link to remote（连接远端）
- git push -u origin main → First push（首次上传）
- git pull → Fetch + merge（拉取代码）
- git clone <url> → Clone repository（下载仓库）

---

## 🌿 Branching
- git branch → List branches（查看分支）
- git checkout -b feature/test → Create branch（创建分支）
- git checkout main → Switch branch（切换分支）
- git merge feature/test → Merge branch（合并分支）
- git branch -d branch → Delete branch（删除分支）

---

## ⏪ Undo / Reset
- git restore file → Discard changes（撤销修改）
- git reset file → Unstage file（取消 add）
- git reset --soft HEAD~1 → Undo commit keep changes（回退但保留代码）
- git reset --hard HEAD~1 → Hard reset（危险）

---

## 🕒 Time Travel
- git checkout <commit-id> → Go to old version（切换历史版本）
- git switch -c debug <id> → New branch from old commit（从历史开分支）

---

## 📦 Stash
- git stash → Save changes temporarily（暂存修改）
- git stash pop → Restore changes（恢复修改）

---

## 🔍 Debugging
- git diff → Show changes（查看改动）
- git diff --staged → Show staged changes（已暂存改动）
- git show <id> → Show commit details（查看某次提交）
- git blame file → Who changed each line（查看责任人）

---

## ⚡ Tips
- Use meaningful commit messages（写清楚 commit）
  - feat: new feature
  - fix: bug fix
  - docs: documentation

- Commit small changes（小步提交）

- Use branches for features（用分支开发）

- Prefer SSH over HTTPS（推荐 SSH）

---

## 📌 Notes
- SSH key configured successfully
- First repo pushed to GitHub
- Practicing Git commands for DevOps role

## 🧠 git add Variations

| Command | Description | Usage |
|--------|-------------|------|
| `git add .` | Add all changes in current directory | Quick commit |
| `git add -A` | Add all changes in the repository | Recommended (complete) |
| `git add file.txt` | Add a specific file | Precise control |
| `git add *.js` | Add files by pattern | Batch add |
| `git add -u` | Add modified and deleted files only | Excludes new files |
| `git add -p` | Interactive (partial) add | Fine-grained control |

---

## 🔍 Key Differences

| Command | New Files | Modified | Deleted |
|--------|----------|----------|----------|
| `git add .` | ✔ | ✔ | ✔ |
| `git add -A` | ✔ | ✔ | ✔ |
| `git add -u` | ✘ | ✔ | ✔ |

---

## ⚡ Tips

- Use `git add .` for quick commits  
- Use `git add -A` for full consistency  
- Use `git add file` for precise control  
- Use `git add -p` to commit partial changes  
- Prefer small, meaningful commits  

---

## 📌 Example

```bash
git add .
git commit -m "feat: update git notes"