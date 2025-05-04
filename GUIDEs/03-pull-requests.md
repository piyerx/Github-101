 # Pull Requests Guide

Understand what pull requests (PRs) are, how to create one, and best practices to collaborate efficiently on GitHub.

---

## 📚 Table of Contents

* [1. What is a Pull Request?](#1-what-is-a-pull-request)
* [2. Why Use Pull Requests?](#2-why-use-pull-requests)
* [3. Creating a Pull Request](#3-creating-a-pull-request)
* [4. Reviewing a Pull Request](#4-reviewing-a-pull-request)
* [5. Merging a Pull Request](#5-merging-a-pull-request)
* [6. Best Practices](#6-best-practices)

---

## 1. What is a Pull Request?

A pull request is a way to propose changes from one branch to another (usually feature → main). It allows for code review and discussion before merging.

## 2. Why Use Pull Requests?

* Collaboration: Multiple people can work on the same codebase.
* Review: Team members can review and comment before merging.
* History: Keeps track of why changes were made.

## 3. Creating a Pull Request

1. Push your feature branch to GitHub.
2. Navigate to the repository on GitHub.
3. Click on **"Compare & pull request"**.
4. Add a meaningful title and description.
5. Click **"Create pull request"**.

> ⚠️ Make sure your branch is up to date with the target branch to avoid conflicts.

## 4. Reviewing a Pull Request

* Click on the PR in GitHub.
* Use the **"Files changed"** tab to view diffs.
* Add comments inline.
* Approve or request changes.

```diff
+ Looks good to me
- Missing validation logic on this part
```

## 5. Merging a Pull Request

* Once approved, click **"Merge pull request"**.
* Choose one of the following:

  * **Create a merge commit** (default, preserves history)
  * **Squash and merge** (combine all commits into one)
  * **Rebase and merge** (apply commits one by one, cleaner history)

## 6. Best Practices

* Always create a new branch for every feature or fix.
* Keep PRs small and focused.
* Add screenshots or demo gifs for UI changes.
* Mention related issues with `Fixes #issue_number`.
* Use draft PRs to share WIP (Work in Progress).

---

## Final Notes

Pull requests are the core of collaboration on GitHub. Use them regularly to ensure clean, reviewed, and traceable code updates.

*~Created by [Piyush](https://github.com/piyerx)*