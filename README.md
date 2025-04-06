# 📘 Git Commands: Complete Guide with Explanations

This guide documents essential Git commands with their real-world usage, examples, and developer tips. Follow this as you practice!

---

## 🔰 1. Initializing and Configuring Git

```bash
git init
```

<sub>- Initializes a Git repository in your current project directory.</sub>

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

<sub>- Sets your Git identity globally.</sub>

## 🌐 2. Connecting to GitHub

```bash
gh auth login
```

<sub>- Authenticates your system with GitHub using CLI.</sub>

```bash
gh repo create my-repo-name --source=. --public --remote=origin --push
```

<sub>- Creates a GitHub repository and pushes code.</sub>

## 📁 3. Creating and Working with Files

```bash
touch index.html
mkdir components
```

<sub>- Creates a file or directory.</sub>

## 🌿 4. Branching

```bash
git branch
git branch feature/login
git checkout feature/login
```

<sub>- Lists, creates, and switches branches.</sub>

```bash
git branch --merged
git branch --no-merged
git log --graph --oneline --all
```

<sub>- Lists branches already merged into current branch.</sub>
<br>
<sub>- Lists branches not yet merged.</sub>
<br>
<sub>- Visualize branch history & merges.</sub>

## ✅ 5. Staging and Committing Changes

```bash
git status
git add .
git commit -m "feat: add login UI"
```

<sub>- Shows status, stages, and commits changes.</sub>

## 🚀 6. Pushing to Remote Repo

```bash
git push origin feature/login
```

<sub>- Pushes a branch to GitHub.</sub>

## 🔄 7. Pulling and Syncing Code

```bash
git pull origin main
```

<sub>- Pulls the latest code from the main branch.</sub>

## 🔀 8. Merging

```bash
git checkout dev
git merge feature/login
```

<sub>- Switches branches and merges changes.</sub>

## 🧪 9. Undo & Revert

```bash
git restore file.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit-id>
```

<sub>- Undoes changes safely.</sub>

## 🧹 10. Clean Up & Delete Branches

```bash
git branch -d feature/login
git push origin --delete feature/login
```

<sub>- Deletes local and remote branches.</sub>

## 🔍 11. View History and Logs

```bash
git log
```

<sub>- Shows the full commit history.</sub>

```bash
git log --oneline
```

<sub>- Displays a summarized commit history.</sub>

## 📦 12. Clone Existing GitHub Repo

```bash
git clone git@github.com:username/repo-name.git
```

<sub>- Clones a repository using SSH.</sub>

```bash
git remote add origin git@github.com:username/repo-name.git
```

<sub>- Links your local repository to a remote one.</sub>

#📋 Bonus Tips

1. Always pull before pushing
2. Use meaningful commit messages (feat:, fix:, chore:)
3. Work on branches, not directly on main

<sub>✅ Made by Rakshit | For self-practice and real dev workflows | 🕒 Last Updated: April 2025</sub>
