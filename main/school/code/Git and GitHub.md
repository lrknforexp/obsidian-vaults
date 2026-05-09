# Git and GitHub

> [!info] Quick Facts
> **Git Created:** 2005 by Linus Torvalds (creator of Linux)
> **GitHub Founded:** 2008 (acquired by Microsoft in 2018)
> **Type:** Version control system (Git) + code hosting platform (GitHub)
> **Used For:** Tracking code changes, collaborating, saving history, portfolio
> **Difficulty:** ⭐ to ⭐⭐ — Basic commands are simple; branching/merging takes practice
> **Download Git:** https://git-scm.com/
> **GitHub:** https://github.com/

---

**Git** is a version control system — it tracks every change you make to your code so you can undo mistakes, revert to earlier versions, and collaborate with others without overwriting each other's work. **GitHub** is the website where you store your Git repositories online. Think of Git as the tool and GitHub as the cloud storage.

> [!info] Why This is Non-Negotiable
> **Every professional developer uses Git daily.** If you apply for any tech job, interviewers will look at your GitHub profile. A blank GitHub = you look like you don't code. Start using it from Day 1, even for solo projects.

---

## Setup

```bash
# Install Git from https://git-scm.com/
# Then configure your identity:
git config --global user.name "Your Name"
git config --global user.email "you@email.com"

# Verify setup
git config --list
```

---

## The Basic Workflow

```bash
# 1. Initialize a new repository (do this once per project)
git init

# 2. Check what's changed
git status

# 3. Stage changes (prepare them for saving)
git add filename.txt        # stage one file
git add .                   # stage everything

# 4. Commit (save a snapshot with a message)
git commit -m "Add navigation bar to homepage"

# 5. Push to GitHub (upload your code)
git push origin main
```

---

## Working with GitHub

```bash
# Clone an existing repo from GitHub to your computer
git clone https://github.com/username/repo-name.git

# Connect a local repo to GitHub for the first time
git remote add origin https://github.com/username/repo-name.git
git branch -M main
git push -u origin main

# Pull latest changes from GitHub
git pull

# Check your remote connections
git remote -v
```

---

## Branching and Merging

```bash
# See all branches
git branch

# Create a new branch
git branch feature/login-page

# Switch to a branch
git checkout feature/login-page

# Create AND switch in one command (modern)
git switch -c feature/login-page

# Merge a branch into main
git checkout main
git merge feature/login-page

# Delete a branch after merging
git branch -d feature/login-page
```

> [!info] Why Branches?
> Branches let you work on new features without breaking your working code. The `main` branch is always stable — you work in feature branches and only merge when it's ready.

---

## Viewing History

```bash
# See commit history
git log
git log --oneline         # compact view

# See what changed in a specific commit
git show abc1234

# See difference between current code and last commit
git diff
```

---

## Undoing Mistakes

```bash
# Undo unstaged changes (restore a file to last commit)
git restore filename.txt

# Unstage a file (undo git add)
git restore --staged filename.txt

# Undo the last commit (keep changes in working directory)
git reset HEAD~1

# DANGER — completely erase last commit and changes
git reset --hard HEAD~1
```

---

## .gitignore

Create a `.gitignore` file to tell Git which files to NOT track:

```
# .gitignore

# Dependencies
node_modules/

# Environment variables (NEVER push API keys)
.env
.env.local

# Build outputs
dist/
build/

# OS files
.DS_Store
Thumbs.db

# Editor files
.vscode/
.idea/
```

---

## Good Commit Message Format

```
Short summary (under 50 characters)

Optional longer description if needed. Explain WHY
you made this change, not just what you changed.

Examples of good messages:
- "Add user login form with validation"
- "Fix bug where cart total didn't update"
- "Refactor auth middleware for readability"

Examples of bad messages:
- "stuff"
- "fix"
- "asdfasdf"
- "updated files"
```

---

## Free Tutorials

- 🌐 **GitHub Docs:** https://docs.github.com/
- 🌐 **Learn Git Branching (interactive):** https://learngitbranching.js.org/
- 🎓 **GitHub Skills (official free courses):** https://skills.github.com/

## YouTube Tutorials

| Video | Link |
|---|---|
| Git and GitHub for Beginners (freeCodeCamp, 1hr) | ![](https://www.youtube.com/watch?v=RGOj5yH7evk) |
| Git Crash Course (Traversy Media) | ![](https://www.youtube.com/watch?v=SWYqp7iY_Tc) |
| Git Tutorial for Beginners (Programming with Mosh) | ![](https://www.youtube.com/watch?v=8JJ101D3knE) |
| GitHub Actions CI/CD (TechWorld with Nana) | ![](https://www.youtube.com/watch?v=R8_veQiYBjI) |

---

## Related Notes
- [[Coding - Master Index]]
- [[Tools and Setup]]
- [[Amateur Stage]]
- [[Master Stage]]
- [[Practice and Projects]]
