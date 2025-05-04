  # Git Cheat Sheet

Your go-to reference for everyday Git commands and workflows. This file covers the essential Git commands used in individual and team projects, explained simply and clearly.

---

## 📚 Table of Contents

* [1. Git Setup](#1-git-setup)
* [2. Initializing a Repository](#2-initializing-a-repository)
* [3. Adding and Committing Changes](#3-adding-and-committing-changes)
* [4. Working with Remote Repositories](#4-working-with-remote-repositories)
* [5. Branching](#5-branching)
* [6. Merging and Conflicts](#6-merging-and-conflicts)
* [7. Pulling and Pushing](#7-pulling-and-pushing)
* [8. Undoing Changes](#8-undoing-changes)
* [9. Checking Status and Logs](#9-checking-status-and-logs)

---

## 1. Git Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

> Sets your identity globally for all Git repositories.

---

## 2. Initializing a Repository

```bash
git init
```

> Initializes a new Git repository in your current directory.

---

## 3. Adding and Committing Changes

```bash
git add .
```

> Stages all changes in the directory for the next commit.

```bash
git commit -m "Your commit message"
```

> Records the staged changes with a message.

---

## 4. Working with Remote Repositories

```bash
git remote add origin https://github.com/yourname/your-repo.git
```

> Links your local repo to a remote GitHub repo.

```bash
git branch -M main
```

> Renames your current branch to `main` (GitHub's default).

```bash
git push -u origin main
```

> Pushes your local commits to the remote repo and sets upstream tracking.

---

## 5. Branching

```bash
git branch new-feature
```

> Creates a new branch called `new-feature`.

```bash
git checkout new-feature
```

> Switches to the `new-feature` branch.

```bash
git checkout -b new-feature
```

> Creates and switches to the `new-feature` branch in one command.

---

## 6. Merging and Conflicts

```bash
git checkout main
git merge new-feature
```

> Merges the `new-feature` branch into `main`.

> If there's a conflict, Git will prompt you to resolve it manually in the affected files.

```bash
git add conflicted-file.js
git commit
```

> After resolving conflicts, add the file and commit to complete the merge.

---

## 7. Pulling and Pushing

```bash
git pull origin main
```

> Pulls the latest changes from the `main` branch of the remote repository.

```bash
git push
```

> Pushes your local commits to the tracked remote branch.

---

## 8. Undoing Changes

```bash
git restore filename.txt
```

> Reverts uncommitted changes in the working directory.

```bash
git reset HEAD filename.txt
```

> Unstages a file (after `git add` but before `git commit`).

```bash
git revert <commit_hash>
```

> Creates a new commit that undoes the changes made by a previous commit.

---

## 9. Checking Status and Logs

```bash
git status
```

> Shows the current state of your working directory and staging area.

```bash
git log
```

> Displays the commit history.

```bash
git log --oneline --graph --all
```

> Shows a summarized visual commit history.

---

## Final Notes

* Always pull before pushing to avoid conflicts.
* Write meaningful commit messages.
* Use branches to work safely on new features.

This sheet will evolve as you learn more commands and workflows. Keep it handy!

*~Created by [Piyush](https://github.com/piyerx)*

