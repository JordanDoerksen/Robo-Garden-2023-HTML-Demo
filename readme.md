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

| Command                             | Action                                                                                           |
| ----------------------------------- | ------------------------------------------------------------------------------------------------ |
| `git status`                        | What is the state of my current working tree? (The current state of all files in the local repo) |
| `git add <file>`                    | Stage this file(or files)                                                                        |
| `git commit -m "my commit message"` | Commit changes to the local version history                                                      |
| `git push`                          | syncs local changes up to the upstream origin (e.g. github)                                      |
| `git pull`                          | sync remote changes down to your local development environment                                   |
| `git checkout -b branch-name`       | Create a new branch locally and give it a name                                                   |
| `git stash`                         | Sets modifications aside to be reapplied later                                                   |
| `git stash pop`                     | apply stashed changes to current working tree                                                    |
| `git branch`                        | List local branches                                                                              |
| `git branch -r`                     | List remote branches                                                                             |
| `git switch main`                   | Switch to target branch (in this example the `main` branch)                                      |

## How to merge branches
1. Switch to the branch you want to merge your changes into `git switch main`
   > If I made changes in a branch called `bug-fix` and want those changes in `main` I need to be in the main branch
2. Check upstream of the target branch for unmerged changes `git fetch`
3. Get upstream changes `git pull`
4. Merge the branch into current branch `git merge the-name-of-the-other-branch`