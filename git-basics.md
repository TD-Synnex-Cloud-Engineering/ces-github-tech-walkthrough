# Git basics: one-page reference

Core loop: edit → `git add` → `git commit` → `git push`; `git pull` to update.

| Command | What it does |
| --- | --- |
| **Start** |  |
| `git config --global user.name "You"` | Set your name (repeat for `user.email`) |
| `git init` | Turn the current folder into a new repo |
| `git clone <url>` | Copy a GitHub repo to your computer |
| **Save your work** |  |
| `git status` | Show what changed and what is staged |
| `git add <file>` | Stage a file (`git add .` stages all) |
| `git commit -m "message"` | Save staged changes as a local snapshot |
| `git log --oneline` | List past commits, one line each |
| **Branch** |  |
| `git branch` | List branches; `*` marks the one you are on |
| `git switch -c <name>` | Create a new branch and switch to it |
| `git switch <name>` | Switch to an existing branch |
| `git merge <name>` | Merge that branch into the one you are on |
| **Sync with GitHub** |  |
| `git pull` | Get the latest changes from GitHub |
| `git push` | Upload your commits to GitHub |
| `git push -u origin <name>` | First push of a new branch; links it to GitHub |
| **Undo** |  |
| `git restore <file>` | Discard unstaged edits to a file (no undo) |

Older guides use `git checkout` for `git switch` and `git restore`.
