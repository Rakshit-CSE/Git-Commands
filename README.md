# 📘 Git Commands: Complete Guide with Explanations

This guide documents essential Git commands with their real-world usage, examples, and developer tips. Follow this as you practice!

---

## 🔰 1. Initializing and Configuring Git

```bash
git init
```

- Initializes a Git repository in your current project directory.

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

- Sets your Git identity globally (used in all repositories).

```bash
gh auth login
```

- Authenticates your system with GitHub using CLI (one-time setup).

```bash
gh repo create my-repo-name --source=. --public --push
```

- Creates a new GitHub repository from your current folder and pushes the code there.

```bash
touch index.html
mkdir components
```

- Creates a new file or directory.

```bash
git branch
git branch feature/login
git checkout feature/login
```

- Lists branches, creates a new branch, and switches to it.

```bash
git status
git add .
git commit -m "feat: add login UI"
```

- Shows change status, stages changes, and commits them with a meaningful message.

```bash
git push origin feature/login
```

- Pushes your local branch to GitHub.

```bash
git pull origin main
```

- Pulls the latest code from the main branch of the remote repository.

```bash
git checkout dev
git merge feature/login
```

- Switches to the `dev` branch and merges `feature/login` into it.

```bash
git restore file.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit-id>
```

- Used to undo uncommitted and committed changes safely.

```bash
git branch -d feature/login
git push origin --delete feature/login
```

- Deletes local and remote branches once your feature is merged.

```bash
git log
```

- Shows the full commit history (author, date, message, ID).

```bash
git log --oneline
```

- Displays a summarized version of the commit history (great for quick views).

```bash
git clone git@github.com:username/repo-name.git
```

- Downloads an existing GitHub repository to your local system using SSH.

```bash
git remote add origin git@github.com:username/repo-name.git
```

- Links your local repository to the remote GitHub repository so you can push/pull code.

#📋 Bonus Tips

1. Always pull before pushing
2. Use meaningful commit messages (feat:, fix:, chore:)
3. Work on branches, not directly on main

✅ Made by Rakshit | For self-practice and real dev workflows
🕒 Last Updated: April 2025
