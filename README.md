# 🧭 Git Collaboration Workflow Cheat Sheet

_A concise guide for effective teamwork using Git._

---

## 🚀 1. Setup

Clone the repository:
```bash
git clone https://github.com/org/project.git
cd project
```

Set your info (only once per machine):
```bash
git config user.name "Your Name"
git config user.email "your@email.com"
```

---

## 🌿 2. Branching Model

**Main branches**
- `main` → always stable, production-ready
- `develop` → (optional) integration branch

**Feature branches**
- `feature/<description>` → for new features or tasks  
- `bugfix/<description>` → for fixing issues  
- `hotfix/<description>` → urgent fixes on `main`

Create your own branch:
```bash
git checkout main
git pull origin main
git checkout -b feature/short-description
```

Example:  
`feature/login-ui` or `bugfix/fix-login-validation`

---

## 💻 3. Working on Code

Stage and commit your changes:
```bash
git add .
git commit -m "Add login form validation"
```

✅ Commit small, focused changes  
✅ Write clear, descriptive messages  

---

## 🔁 4. Sync with the Team

Keep your branch updated before pushing or merging:
```bash
git checkout main
git pull origin main
git checkout feature/short-description
git merge main
# or: git rebase main
```

If merge conflicts appear:
- Edit the marked files
- Choose what to keep
- Then:
  ```bash
  git add .
  git commit
  ```

---

## ☁️ 5. Push and Create a Pull Request (PR)

Push your branch to remote:
```bash
git push -u origin feature/short-description
```

Then open a **Pull Request** on GitHub/GitLab:
- ✅ Give a clear title and summary  
- 🧠 Request at least one review  
- 🚫 Don’t merge your own PR without approval  

After the PR is merged:
```bash
git checkout main
git pull origin main
git branch -d feature/short-description
```

---

## 🧩 6. Best Practices

✅ One branch per feature or bug  
✅ Small, atomic commits  
✅ Pull `main` often  
✅ Use meaningful names (`feature/signup-form`)  
✅ Don’t commit build files, secrets, or `.env`  

---

## 🧠 7. Useful Commands

| Command | Description |
|----------|-------------|
| `git status` | Show current changes |
| `git log --oneline --graph --all` | Visualize branch history |
| `git diff` | Show unstaged changes |
| `git stash` / `git stash pop` | Temporarily store work |
| `git fetch` | Get remote updates (no merge) |
| `git branch -a` | List all branches |
| `git remote -v` | Show remotes (origin, upstream, etc.) |

---

## 🧹 8. Optional Tools for Teams

🧾 **.gitignore** — ignore build outputs, dependencies, secrets  
✨ **Prettier / ESLint** — enforce consistent formatting  
⚙️ **GitHub Actions** — automate tests or deployment  
📋 **GitHub Projects / Issues** — organize tasks and sprints  

---

### 💡 Pro Tips
- Use `draft` PRs for work in progress  
- Review code with empathy and clarity  
- Keep `main` clean — only merge approved, tested code  

---

**Happy collaborating!** 💪  
_Commit often, commit well, and communicate clearly._