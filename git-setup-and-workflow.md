# Git Setup & First Push (Clean Log)

## 1. Configure Git

```bash
git config --global user.name "<your-username>"
git config --global user.email "<your-email>"
```

---

## 2. Create Project

```bash
cd ~/Desktop
mkdir git-test
cd git-test
git init
```

---

## 3. Add File

```bash
echo "hello git" > test.txt

git add .
git commit -m "test: initial commit"
```

---

## 4. Set Branch

```bash
git branch -M main
```

---

## 5. Connect to GitHub

```bash
git remote add origin git@github.com:<your-username>/git-test.git
```

---

## 6. Setup SSH Key (Summary)

```bash
ssh-keygen -t ed25519 -C "<your-email>"
ssh -T git@github.com
```

Add public key to GitHub:

* Settings → SSH and GPG keys → New SSH key

---

## 7. Push to GitHub

```bash
git push -u origin main
```

---

## 8. Add Documentation

```bash
touch git-command.md

git add .
git commit -m "docs: add git commands cheat sheet"
git push
```

---

## 9. Useful Commands

```bash
git log --oneline
git log -p
git show <commit-id>
```

---

## Notes

* SSH authentication configured successfully
* First repository pushed to GitHub
* Practicing Git workflow and version control
