# Creating Git Repository

\# 1. On GitHub (done via browser):

\# - Create new repository with the exact same name as your local folder: https://github.com/new

\# - Do NOT initialize with README or .gitignore or license (those fields should be set to `Off`)

\# - Generate a Personal Access Token (PAT) with only `repo` permissions (under `scope`) for authentication


&nbsp;
&nbsp;

\# 2. In PowerShell, inside your local project folder:

```
cd path\\to\\your\\project            # Navigate to your project directory
git init                          # Initialize a new local Git repository
```


\# - Set your Git identity globally (only needed once or if not set before)

```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```


\# Push commits to GitHub, set `'origin/main'` as the upstream branch

```
git add .                         # Stage all files for commit
git commit -m "Initial commit"`  # Commit staged files with a message
git branch -M main                # Rename default branch to 'main' (if needed)
git remote add origin https://github.com/CarmelBaris/YourRepoName.git # Add GitHub repo as remote named 'origin'
git push --set-upstream origin main
```

\# - When prompted for password, enter your GitHub Personal Access Token (PAT)

\# - And that's it! 

