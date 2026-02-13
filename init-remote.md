# Connect this folder to GitHub

Run these commands in **Git Bash** or a terminal where `git` works (same folder as this file):

```bash
# 1. Initialize git (if not already)
git init

# 2. Add the remote
git remote add origin https://github.com/MinzhiP/minzhip.github.io.git

# 3. Fetch and set main as default branch (optional but recommended)
git fetch origin
git branch -M main
git branch --set-upstream-to=origin/main main

# 4. If the remote already has commits and you want to keep them:
#    git pull origin main --allow-unrelated-histories

# 5. Add, commit, and push your local files (when ready)
git add .
git commit -m "Initial commit"
git push -u origin main
```

**If the repo on GitHub already has content** (e.g. README, index.html) and you want to **replace** it with your local files:

```bash
git push -u origin main --force
```

Use `--force` only if you are sure you want to overwrite the remote; it discards the current history on GitHub.

**If you don’t have Git installed:**  
Install [Git for Windows](https://git-scm.com/download/win), then open **Git Bash** and run the commands above from this folder.
