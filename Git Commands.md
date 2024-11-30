# Git Cheatsheet

- [Git Cheetsheet (GitHub Education)](https://education.github.com/git-cheat-sheet-education.pdf)

# Git Cheat Sheet

## Setup

### Configuring user information used across all local repositories

- `git config --global user.name "[firstname lastname]"`  
  Set a name that is identifiable for version history.

- `git config --global user.email "[valid-email]"`  
  Associate an email with history markers.

- `git config --global color.ui auto`  
  Enable command-line color for better readability.

## Setup and init

### Configuring user information, initializing, and cloning repositories

- `git init`  
  Initialize an existing directory as a Git repository.

- `git clone [url]`  
  Clone a repository from a URL.

## Stage and stapshot

### Working with snapshots and the Git staging area

- `git status`  
  Show modified files in the working directory.

- `git add [file]`  
  Stage a file for the next commit.

- `git reset [file]`  
  Unstage a file while keeping changes.

- `git diff`  
  View changes not staged.

- `git diff --staged`  
  View changes staged but not committed.

- `git commit -m "[descriptive message]"`  
  Commit staged content as a new snapshot.

## Branch  and merge

### Isolating work in branches and integrating changes

- `git branch`  
  List branches, with `*` indicating the active branch.

- `git branch [branch-name]`  
  Create a new branch at the current commit.

- `git checkout [branch-name]`  
  Switch to another branch.

- `git merge [branch]`  
  Merge a specified branch into the current one.

- `git log`  
  Show all commits in the current branch's history.

## Share  and update

### Updating and sharing repositories

- `git remote add [alias] [url]`  
  Add a remote repository alias.

- `git fetch [alias]`  
  Download branches from the remote.

- `git merge [alias]/[branch]`  
  Merge a remote branch into the current one.

- `git push [alias] [branch]`  
  Push local branch commits to the remote repository.

- `git pull`  
  Fetch and merge changes from the remote branch.

## Tracking path changes

### Versioning file deletions and path changes

- `git rm [file]`  
  Delete a file and stage the removal.

- `git mv [existing-path] [new-path]`  
  Move or rename a file and stage the change.

## Temporary commits

### Stashing changes

- `git stash`  
  Temporarily save changes to switch branches.

- `git stash list`  
  List stashed changes.

- `git stash pop`  
  Reapply stashed changes.

- `git stash drop`  
  Discard the most recent stash.

## Rewrite history

### Modifying commits and clearing history

- `git rebase [branch]`  
  Apply commits of the current branch onto another.

- `git reset --hard [commit]`  
  Reset the staging area and working directory to a specific commit.

## Inspect and compare

### Examining logs and differences

- `git log`  
  View commit history.

- `git log branchB..branchA`  
  Show commits in branchA not in branchB.

- `git diff branchB...branchA`  
  Show differences between branches.

- `git show [SHA]`  
  Display an object in human-readable format.

## Ignoring patterns

### Preventing unintended staging or commits

- Create a `.gitignore` file to define ignored files.
