# 📘 Git Commands: Complete Guide with Explanations

This guide documents essential Git commands with their real-world usage, examples, and developer tips. Follow this as you practice!

---

## 🔰 1. Initializing and Configuring Git

git init

📌 What it does: Initializes a Git repository in your current project directory.

git config --global user.name "Your Name"
git config --global user.email "your@email.com"

📌 What it does: Sets your Git identity globally (used in all repos).

## 🌐 2. Connecting to GitHub

gh auth login

📌 What it does: Authenticates your system with GitHub using CLI (one-time setup).

gh repo create my-repo-name --source=. --public --push

📌 What it does: Creates a new GitHub repo from your current folder and pushes the code there.

## 📁 3. Creating and Working with Files

touch index.html
mkdir components

📌 What it does: Creates a new file or directory.

## 🌿 4. Branching

git branch
git branch feature/login
git checkout feature/login

📌 What it does: Lists branches, creates a new branch, and switches to it.

## ✅ 5. Staging and Committing Changes

git status
git add .
git commit -m "feat: add login UI"

📌 What it does: Shows change status, stages changes, and commits them with a meaningful message.

## 🚀 6. Pushing to Remote Repo

git push origin feature/login

📌 What it does: Pushes your local branch to GitHub.

## 🔄 7. Pulling and Syncing Code

git pull origin main

📌 What it does: Pulls latest code from main branch of remote repo.

## 🔀 8. Merging

git checkout dev
git merge feature/login

📌 What it does: Switches to dev and merges feature/login into it.

## 🧪 9. Undo & Revert

git restore file.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit-id>

📌 What it does: Used to undo uncommitted and committed changes safely.

## 🧹 10. Clean Up & Delete Branches

git branch -d feature/login
git push origin --delete feature/login

📌 What it does: Deletes local and remote branches once your feature is merged.

## 🔍 11. View History and Logs

git log

📌 What it does: Shows full commit history (author, date, message, ID).

git log --oneline

📌 What it does: Displays a summarized version of commit history (great for quick views).

## 📦 12. Clone Existing GitHub Repo

git clone git@github.com:username/repo-name.git

📌 What it does: Downloads an existing GitHub repo to your local system using SSH.

## 🔗 13. Link Local Project to GitHub (SSH)

git remote add origin git@github.com:username/repo-name.git

📌 What it does: Links your local repo to the remote GitHub repo so you can push/pull code.

#📋 Bonus Tips

1. Always pull before pushing
2. Use meaningful commit messages (feat:, fix:, chore:)
3. Work on branches, not directly on main

✅ Made by Rakshit | For self-practice and real dev workflows
🕒 Last Updated: April 2025
