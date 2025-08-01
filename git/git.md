=== GIT CHEAT SHEET ===
# SETUP
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git init
git clone <repo-url>

# BASIC WORKFLOW
git status
git add <file>      # Stage file
git add .           # Stage all changes
git commit -m "msg"
git push origin <branch>
git pull origin <branch>

# BRANCHING
git branch          # List branches
git branch <name>   # Create branch
git checkout <branch>
git checkout -b <new-branch>
git merge <branch>
git branch -d <branch>

# REMOTE
git remote -v       # List remotes
git remote add <name> <url>
git remote remove <name>
git push -u origin <branch>

# UNDO
git restore <file>  # Discard changes
git reset --hard    # WARNING: Destructive!
git commit --amend  # Fix last commit
git revert <commit>

# LOG & DIFF
git log             # Full history
git log --oneline   # Compact history
git diff            # Unstaged changes
git show <commit>

# STASH
git stash           # Save changes temporarily
git stash pop       # Restore last stash
git stash list      # View stashes
git stash drop      # Delete last stash

# TAGS
git tag             # List tags
git tag <tag-name>  # Create tag
git push --tags     # Push tags to remote

