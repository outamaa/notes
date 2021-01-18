# Git tips and tricks

## Stashing

Stash tracked changes with `git stash`.

Also stash untracked files:
``` shell
git stash -u
```

Only stash some of the changes, git prompts interactively:

``` shell
git stash -p # --patch
```

Create new branch with stashed changes:

``` shell
git stash branch <branchname>
```
