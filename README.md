# 📘 Git Commands: Complete Guide with Explanations

This guide documents essential Git commands with their real-world usage, examples, and developer tips. Follow this as you practice!

---

## 🔰 1. Initializing and Configuring Git

```bash
git init
```
> Initializes a Git repository in your current project directory.

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```
> Sets your Git identity globally, used to tag commits with your name and email.

---

## 🌐 2. Connecting to GitHub

```bash
gh auth login
```
> Authenticates your terminal with GitHub using the GitHub CLI.

```bash
gh repo create my-repo-name --source=. --public --remote=origin --push
```
> Creates a GitHub repository, links it to your project, and pushes your code in one command.

> **Note:** If `--remote=origin` is not provided, GitHub CLI will auto-generate a remote name. It's safer to use `origin` for consistency.

---

## 📁 3. Creating and Working with Files

```bash
touch index.html
mkdir components
```
> Creates a file (`touch`) and a folder (`mkdir`) in your project directory.

---

## 🌿 4. Branching

```bash
git branch
```
> Lists all local branches.

```bash
git branch feature/login
```
> Creates a new branch called `feature/login`.

```bash
git checkout feature/login
```
> Switches to the `feature/login` branch.

> **Warning:** Always commit or stash your changes before switching branches to avoid losing work.

```bash
git branch --merged
git branch --no-merged
git log --graph --oneline --all
```
> Shows merged branches, unmerged branches, and a visual representation of the commit history.

---

## ✅ 5. Staging and Committing Changes

```bash
git status
```
> Shows modified, added, or deleted files.

```bash
git add .
```
> Stages all changes in the current directory.

```bash
git commit -m "feat: add login UI"
```
> Commits staged changes with a message. Prefixes like `feat:`, `fix:`, `chore:` are standard in teams.

---

## 🚀 6. Pushing to Remote Repo

```bash
git push origin feature/login
```
> Pushes your local branch to the remote repository on GitHub.

---

## 🔄 7. Pulling and Syncing Code

```bash
git pull origin main
```
> Pulls the latest changes from the `main` branch of the remote repo. Always do this before pushing.

---

## 🔀 8. Merging Branches

```bash
git checkout dev
git merge feature/login
```
> Switches to the `dev` branch and merges changes from `feature/login` into it.

---

## 🔁 9. Pull Requests (PRs)

```bash
gh pr create --base main --head feature/about-page --title "Add about page" --body "Added a simple about.html page"
```
> Creates a PR from your branch to `main` with a title and description.

> **Note:** A Pull Request (PR) is a request to merge code from one branch into another. It allows code review, CI checks, and team collaboration.

```bash
gh pr merge --squash --delete-branch
```
> Squash merges all commits into one clean commit and deletes the branch remotely.

> **Tip:** Squash = Cleaner history. Ideal for merging feature branches.

---

## 💾 10. Undoing Changes

```bash
git restore file.txt
```
> Restores `file.txt` to the last committed state.

```bash
git reset --soft HEAD~1
```
> Undoes the last commit, keeps changes staged.

```bash
git reset --hard HEAD~1
```
> Removes the last commit and discards changes completely.

```bash
git revert <commit-id>
```
> Creates a new commit that reverses a specific commit without affecting history.

```bash
git log
```
> Find commit IDs here for revert.

---

## 🔒 11. Stashing Work (Temporary Save)

```bash
git stash
```
> Saves your uncommitted changes temporarily.

```bash
git stash pop
```
> Applies the last stash and removes it.

---

## 🧹 12. Clean Up & Delete Branches

```bash
git branch -d feature/login
```
> Deletes the local branch `feature/login`.

```bash
git push origin --delete feature/login
```
> Deletes the branch from GitHub.

> **Note:** If you already ran `gh pr merge --delete-branch`, the remote is deleted. You'll still need to delete the local branch manually unless you switch branches first.

---

## 🧼 13. Removing Stale Remote Branches

```bash
git remote prune origin
```
> Cleans up remote-tracking branches that no longer exist on GitHub.

> **Tip:** Red branches shown by `git branch -r` are usually stale and need pruning.

---

## 🔍 14. View History and Logs

```bash
git log
git log --oneline
```
> Detailed vs. summarized commit history.

```bash
git log --graph --oneline --all
```
> Visualizes commits and branches in a tree structure.

---

## 📦 15. Cloning and Remote Setup

```bash
git clone git@github.com:username/repo-name.git
```
> Clones a GitHub repo to your system using SSH.

```bash
git remote add origin git@github.com:username/repo-name.git
```
> Links your project to a GitHub repository manually.

---

## 📋 Bonus Tips

- ✅ Always pull before you push to avoid conflicts.
- ✅ Use meaningful commit messages.
- ✅ Use branches to manage features or bug fixes.
- ✅ Clean up merged branches from time to time.
- ✅ Set correct email using:
  ```bash
  git config --global user.email "youremail@example.com"
  ```
- ✅ Use `gh auth login` to log in GitHub CLI once on new machines.

---

### 🛠️ Made by Rakshit | For self-practice and real dev workflows | 🕒 Last Updated: April 2025
