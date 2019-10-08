# Git Workflow Functions

```bash
~: cd my-git-repo

# create a new branch "new-branch" and also
# sibling worktree "my-git-repo~new-branch"

~/my-git-repo (master): gwo new-branch

# list all worktrees

~/my-git-repo~new-branch (new-branch): gwl
~/my-git-repo b8d8b03 [master]
~/my-git-repo~new-branch ae985a [new-branch]

# switch back to master

~/my-git-repo~new-branch (new-branch): gwo master

# delete "new-branch" branch and the worktree

~/my-git-repo (master): gwd new-branch
```
