## Changing a Commit Message After a Merge

### Scenario 1: Commit NOT Pushed Yet (Safe + Simple)

If you have **not pushed** the commit to the remote:

```bash
git commit --amend
```

This opens your editor so you can modify the commit message.

Or skip the editor:

```bash
git commit --amend -m "chore(infra): merge origin/main into main"
```

Then push normally:

```bash
git push origin main
```

---

### Scenario 2: Commit Already Pushed (History Rewrite)

If the commit has already been pushed to GitHub:

```bash
git commit --amend -m "better commit message"
git push --force
```

⚠️ Important:
- This rewrites history.
- Only force push if you're the only one working on the branch.
- Safe for personal infrastructure repos.
- Risky on shared production branches.

---

## Why This Works

- `--amend` rewrites the most recent commit.
- Rewriting a commit changes its hash.
- If it was already pushed, the remote history no longer matches.
- `--force` tells Git to overwrite the remote branch with your updated history.

---

## Advanced (Editing Older Commits)

To edit a commit further back in history:

```bash
git rebase -i HEAD~3
```

This opens interactive rebase mode where you can:
- Reword commit messages
- Squash commits
- Reorder commits
- Drop commits

Use carefully on shared branches.

---

## Professional Workflow Rule

- If it's already pushed and others may depend on it → avoid rewriting history.
- If it's a personal branch → rewriting is usually fine.
- Merge commits are rarely worth amending unless there's a strong reason.
