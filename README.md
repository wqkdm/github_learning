# GitHub Learning

A small repository for practising Git with SCSS, CSS, and JavaScript files.

## Clone the repository

1. Install Git and make sure `git --version` works in your terminal.
2. Open a terminal in the folder where you want to keep the project.
3. Run:

   ```powershell
   git clone https://github.com/wqkdm/github_learning.git
   cd github_learning
   ```

4. Open the `github_learning` folder in VS Code (`code .` if the `code` command is available).
5. Check your checkout:

   ```powershell
   git status
   git branch --show-current
   ```

A fresh clone checks out `main`. If GitHub asks you to authenticate, sign in with an account that has access to this repository.

## Start work on a branch

Create a branch for your task from the latest `main`:

```powershell
git switch main
git pull --ff-only origin main
git switch -c your-name/task-name
```

If your teammate has already pushed a branch you need, fetch it and switch to it instead:

```powershell
git fetch origin
git switch --track origin/branch-name
```

Commit your work locally, then push your branch:

```powershell
git add -- path/to/file
git commit -m "Describe your change"
git push -u origin your-name/task-name
```

Replace the example branch and file names with your own. Coordinate with the team before merging a branch into `main`.
