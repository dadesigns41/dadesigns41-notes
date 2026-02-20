Use Git checkpoints
Codex can modify your codebase, so consider creating Git checkpoints before and after each task so you can easily revert changes if needed.
🧭 1. You Haven’t Committed Yet (Uncommitted Changes)

If you made changes but did NOT commit:

🔹 Discard specific file changes
git restore filename
🔹 Discard ALL uncommitted changes
git restore .

If you also added files (staged):

git restore --staged .
git restore .
🧱 2. You Already Made a Commit (Local Only)

If you made a commit and want to go back one checkpoint:

🔹 Keep the changes but undo commit
git reset --soft HEAD~1
🔹 Undo commit and discard changes completely
git reset --hard HEAD~1

That moves your branch pointer back one commit.

🕰 3. You Want to Go Back to a Specific Checkpoint

First, see history:

git log --oneline

Example output:

a1b2c3d Add docker config
d4e5f6g Update nginx
h7i8j9k Initial commit

To go back to d4e5f6g:

git reset --hard d4e5f6g

Boom. Full rollback.

🚨 4. You Already Pushed and Need to Revert Safely

If changes were pushed and you don’t want to rewrite history:

Use:

git revert <commit-hash>

That creates a NEW commit that undoes the old one.

This is safer for shared branches.
