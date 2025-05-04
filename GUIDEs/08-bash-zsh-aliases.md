 # Bash & Zsh Aliases

A guide on useful Bash and Zsh aliases to speed up your command-line workflow.

---

## 📚 Table of Contents

* [1. What are Aliases?](#1-what-are-aliases)
* [2. Common Aliases](#2-common-aliases)
* [3. Setting up Aliases](#3-setting-up-aliases)
* [4. Advanced Aliases](#4-advanced-aliases)
* [5. Useful Aliases for Development](#5-useful-aliases-for-development)

---

## 1. What are Aliases?

Aliases are shortcuts or abbreviations for longer commands. They help save time when you need to run the same command frequently.

For example, instead of typing `git status` every time, you can create an alias like `gs`.

## 2. Common Aliases

* **`ll`**: `ls -alF` — List files with details (permissions, size, etc.)
* **`la`**: `ls -A` — List all files (including hidden files)
* **`grep`**: `grep --color=auto` — Make `grep` output more readable
* **`gs`**: `git status` — Check Git status
* **`gp`**: `git pull` — Pull changes from the remote repo
* **`gco`**: `git checkout` — Checkout a branch or commit

## 3. Setting up Aliases

To set up aliases in **Bash** or **Zsh**, you need to edit the appropriate configuration file:

* **Bash**: `~/.bashrc`
* **Zsh**: `~/.zshrc`

Example:

```bash
alias gs='git status'
alias ll='ls -alF'
```

Once you've added your aliases, reload your shell configuration:

```bash
source ~/.bashrc  # for Bash
source ~/.zshrc   # for Zsh
```

## 4. Advanced Aliases

* **`..`**: `cd ..` — Go to the parent directory
* **`...`**: `cd ../..` — Go up two directories
* **`extract`**: `tar -xzvf` — Extract tar files
* **`cls`**: `clear` — Clear the terminal screen
* **`update`**: `sudo apt-get update && sudo apt-get upgrade` — Update the system (Linux)

## 5. Useful Aliases for Development

* **`dev`**: `cd ~/projects` — Go to the projects directory
* **`work`**: `cd ~/work` — Go to the work directory
* **`docs`**: `cd ~/docs` — Go to the docs directory
* **`log`**: `tail -f /var/log/syslog` — View logs in real-time

---

## Final Notes

Aliases can greatly speed up your workflow and make it more efficient. You can create custom aliases for any command you use frequently. Just remember to always reload your configuration file after adding new aliases!

*~Created by [Piyush](https://github.com/piyerx)*