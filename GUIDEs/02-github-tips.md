 # GitHub Tips

A collection of practical tips and lesser-known tricks to improve your GitHub workflow and project visibility.

---

## 📚 Table of Contents

* [1. Writing a Great README](#1-writing-a-great-readme)
* [2. Organizing Your Repository](#2-organizing-your-repository)
* [3. Using `.gitignore` Effectively](#3-using-gitignore-effectively)
* [4. Making Commits Meaningful](#4-making-commits-meaningful)
* [5. Keeping a Clean Commit History](#5-keeping-a-clean-commit-history)
* [6. GitHub Repository Settings](#6-github-repository-settings)
* [7. Managing Issues and Discussions](#7-managing-issues-and-discussions)
* [8. Adding Badges to README](#8-adding-badges-to-readme)
* [9. Keeping Projects Public-Ready](#9-keeping-projects-public-ready)

---

## 1. Writing a Great README

* Always include a `README.md` file to describe your project.
* Use headings, installation steps, usage examples, and contribution guidelines.

## 2. Organizing Your Repository

* Create folders like `assets/`, `src/`, `docs/` to keep things clean.
* Place all markdown guides or docs inside a `guide/` or `docs/` folder.

## 3. Using `.gitignore` Effectively

* Avoid committing unnecessary files like OS/system files, IDE configs, or build outputs.
* Use [gitignore.io](https://www.toptal.com/developers/gitignore) to generate a `.gitignore` based on your tech stack.

## 4. Making Commits Meaningful

* Write clear commit messages: `Add login form validation`, not `Fix stuff`.
* Use imperative mood: "Add", "Update", "Fix", etc.

## 5. Keeping a Clean Commit History

* Avoid committing generated files or temporary folders.
* Use `git rebase` or squash commits before merging feature branches.

## 6. GitHub Repository Settings

* Set the default branch (usually `main`).
* Add a license file (MIT, Apache 2.0, etc.).
* Enable Discussions or Issues if you're open to community input.

## 7. Managing Issues and Discussions

* Use labels like `bug`, `enhancement`, `question`, etc.
* Assign issues and set milestones for better planning.

## 8. Adding Badges to README

* Use shields.io to generate custom badges like:

```md
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen)
```

* Popular badges: License, Build status, Last commit, Contributors, etc.

## 9. Keeping Projects Public-Ready

* Hide secrets/API keys using environment variables.
* Include a LICENSE file.
* Add `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md` for open source repos.

---

## Final Notes

* GitHub is not just a code host—it's your portfolio.
* Keep projects tidy, README polished, and commit messages clear.
* Use GitHub features like releases, wikis, and GitHub Pages to showcase your work.

*~Created by [Piyush](https://github.com/piyerx)*