# 09-advanced-git-topics.md

## Advanced Git Topics – A deeper dive into tricky concepts

---

## 📚 Table of Contents
1. [Git Rebase](#1-git-rebase)  
2. [Git Cherry-Pick](#2-git-cherry-pick)  
3. [Git Stash](#3-git-stash)  
4. [Squashing Commits](#4-squashing-commits)  
5. [Git Bisect](#5-git-bisect)  

---

## 1. Git Rebase
**Subtitle:** Rewriting history for a cleaner commit timeline.

### What it does:
`git rebase` moves or combines commits onto a new base commit. It’s used to:
- Sync feature branches with `main`
- Tidy up commit history

### Example:
```bash
git checkout feature-branch
git rebase main
```

### Interactive Rebase:
```bash
git rebase -i HEAD~4
```
Reorders, squashes, or edits the last 4 commits.

### ⚠️ Caution:
- Don’t rebase public/shared branches.
- Rewriting history can cause conflicts if others depend on it.

---

## 2. Git Cherry-Pick
**Subtitle:** Apply specific commits across branches.

### What it does:
Selects a commit from one branch and applies it to another.

### Example:
```bash
git cherry-pick <commit-hash>
```

### Use Case:
You made a hotfix on `dev` that needs to be applied to `main`.

---

## 3. Git Stash
**Subtitle:** Temporarily shelve uncommitted changes.

### What it does:
Puts aside your changes so you can work on something else.

### Basic usage:
```bash
git stash       # Save changes
git stash pop   # Reapply and remove stash
```

### Other commands:
```bash
git stash list
git stash apply
git stash clear
```

### Use Case:
Switching branches quickly without committing WIP changes.

---

## 4. Squashing Commits
**Subtitle:** Combine commits into one.

### What it does:
Used via interactive rebase to reduce clutter in history.

### Example:
```bash
git rebase -i HEAD~3
```
In the editor, change all but the first `pick` to `squash`.

### Benefit:
Keeps commit history clean, especially before merging PRs.

---

## 5. Git Bisect
**Subtitle:** Find the bug through binary search.

### What it does:
Helps track down which commit introduced a bug.

### Example:
```bash
git bisect start
git bisect bad HEAD
git bisect good <last-working-commit>
```

Git checks out commits between those two. After each test:
```bash
git bisect good    # if bug is not present
git bisect bad     # if bug is present
```

Once done:
```bash
git bisect reset
```

---

## Final Notes

These topics are powerful tools in a developer’s Git arsenal. Practice them in a safe environment (like a test repo) to build confidence before using them in production.

*~Created by [Piyush](https://github.com/piyerx)*