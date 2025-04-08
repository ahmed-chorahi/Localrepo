# Git Commands Reference Guide

## Repository Setup
```bash
# Initialize new repository
git init

# Clone repository
git clone https://github.com/username/repository.git
```

## Daily Commands
```bash
# Check status
git status

# Stage changes
git add .                    # All files
git add filename            # Single file

# Commit
git commit -m "message"

# Push changes
git push origin main
```

## Branch Operations
```bash
# View branches
git branch                  # Local
git branch -r              # Remote
git branch -a              # All

# Create & switch branch
git checkout -b new-branch

# Switch branches
git checkout branch-name

# Delete branch
git branch -d branch-name  # Safe
git branch -D branch-name  # Force
```

## Syncing
```bash
# Fetch updates
git fetch origin

# Pull changes
git pull origin main

# Update tracking
git fetch --prune
```

## History & Differences
```bash
# View history
git log
git log --oneline

# View changes
git diff
git diff --staged
```

## Undo Changes
```bash
# Unstage files
git reset filename

# Discard changes
git checkout -- filename

# Undo commit
git reset --soft HEAD~1    # Keep changes
git reset --hard HEAD~1    # Discard changes
```

## Remote Operations
```bash
# Add remote
git remote add origin URL

# Change remote URL
git remote set-url origin URL

# View remotes
git remote -v
```

## Stash Management
```bash
# Save changes
git stash

# List stashes
git stash list

# Apply stash
git stash apply

# Delete stash
git stash drop
```

## Merging
```bash
# Merge branch
git merge branch-name

# Cancel merge
git merge --abort
```

## Configuration
```bash
# Set credentials
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# Set default branch
git config --global init.defaultBranch main
```