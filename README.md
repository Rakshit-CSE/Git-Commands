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

```bash
gh auth login
```

<sub>- Authenticates your system with GitHub using CLI.</sub>

```bash
gh repo create my-repo-name --source=. --public --push
```

<sub>- Creates a GitHub repository and pushes code.</sub>

```bash
touch index.html
mkdir components
```

<sub>- Creates a file or directory.</sub>

```bash
git branch
git branch feature/login
git checkout feature/login
```

<sub>- Lists, creates, and switches branches.</sub>

```bash
git status
git add .
git commit -m "feat: add login UI"
```

<sub>- Shows status, stages, and commits changes.</sub>

```bash
git push origin feature/login
```

<sub>- Pushes a branch to GitHub.</sub>

```bash
git pull origin main
```

<sub>- Pulls the latest code from the main branch.</sub>

```bash
git checkout dev
git merge feature/login
```

<sub>- Switches branches and merges changes.</sub>

```bash
git restore file.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit-id>
```

<sub>- Undoes changes safely.</sub>

```bash
git branch -d feature/login
git push origin --delete feature/login
```

<sub>- Deletes local and remote branches.</sub>

```bash
git log
```

<sub>- Shows the full commit history.</sub>

```bash
git log --oneline
```

<sub>- Displays a summarized commit history.</sub>

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
