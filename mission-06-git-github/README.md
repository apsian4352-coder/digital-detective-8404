# Mission 6 — Git and GitHub

## 1. Task / objective
Understand how Git works, practice staging and committing, create a feature branch (`update-about`), prepare a Pull Request, and write a quick Git glossary.

## 2. Work completed
- Checked status and history with `git status` and `git log`.
- Practiced staging individual files and explained staging vs committing.
- Created branch `update-about`, added a "My Learning" section to `README.md`, and committed it.
- Kept the branch 1 commit ahead of `main` so the GitHub Pull Request button activates right away.
- Wrote a 1-line summary for 9 core Git commands.

## 3. Commands / tools used
- `git status`: Checked modified and staged files.
- `git add filename`: Staged changes.
- `git commit -m "..."`: Saved a commit snapshot.
- `git log --oneline`: Checked commit history.
- `git branch`: Listed branches.
- `git checkout -b update-about`: Created and switched to the new branch.
- `git checkout main`: Switched back to main.

## 4. My understanding

### Task 6.1 — Git Workflow

| Git operation | What it does in your own words |
| :--- | :--- |
| Check repository status (`git status`) | Tells you what files have changed and what is staged. |
| Stage selected changes (`git add filename`) | Picks specific files to be included in the next commit. |
| Create a commit (`git commit -m "..."`) | Saves a permanent snapshot of staged files with a message. |
| View commit history (`git log --oneline`) | Shows a list of past commits. |

**Staging vs Committing:** Staging is like putting files into a box. Committing is sealing the box and saving it to history. You can stage a few files at a time before making the commit.

### Tasks 6.2 & 6.3 — Branches and Pull Requests
- **What is a branch?** An independent copy of the project where you can make changes without messing up the working code on `main`.
- **What is a Pull Request?** A way on GitHub to show teammates what you changed on your branch and ask them to review and merge it into `main`.
- **Status of branch:** I created `update-about`, committed the `My Learning` update, and left it 1 commit ahead of `main`. When pushed, it is ready to open a Pull Request immediately.

### Task 6.4 — Git Command Glossary

| Git Operation | One-Line Explanation |
| :--- | :--- |
| `git init` | Starts a new Git repository in the current folder. |
| `git status` | Shows which files are modified, staged, or untracked. |
| `git add` | Stages files so they are ready for the next commit. |
| `git commit` | Saves the staged changes permanently with a message. |
| `git log` | Lists previous commits in chronological order. |
| `git branch` | Shows existing branches or creates a new one. |
| `git checkout` / `git switch` | Switches between different branches. |
| `git push` | Uploads local commits to GitHub. |
| `git pull` | Downloads and merges changes from GitHub into local. |

## 5. Difficulties faced
I had to make sure my changes were committed before switching branches so nothing got mixed up.

## 6. How I resolved them
I ran `git status` before switching branches to make sure my working directory was completely clean.

## 7. Evidence / files
- `mission-06-git-github/README.md`
- Branch `update-about` (1 commit ahead).

## 8. Commit details
- Commit message: `Complete Git and GitHub collaboration mission`
- Status: Committed to `main`.
