# GIT

## GIT Commands

```bash
# Print info about current repo
git status

# Create new git repo in current directory
git init

# Stage untracked or modified files
git add <file location>

# Commit all staged changes to the local repo
git commit -m "<commit message>"

# Add an upstream origin
git remote add origin <https://url/to/git/repo.git>

# Change the name of your current branch
git branch -M main

# Push changes to your local repository to the upstream repository. This command is also specifying the upstream branch name
git push -u origin main

# GIT Merge Conflict Demo
```

## GIT File states
1. Untracked files
   - File has been created but git is not controlling it
2. Unstaged files
   - Files that belong to the version history and have been modified in the current working tree
3. Staged files
   - Files that are staged are slated to be commited
4. Commited files
   - Commited files have been added to the local version history

# GIT Merge Conflict Demo

# test
