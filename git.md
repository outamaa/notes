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

## Remote

### Add remote

```shell
$ git remote add <remotename> <url>
```

### Fetch and merge upstream

```shell
$ git fetch upstream
$ git checkout <branch>
$ git merge upstream/<branch>
```

### Cherry picking

#### Cherry pick merge from another branch

For cherry picking merge commits, you need to specify which parent of
the merge will be used. This can be specified with `-m`

``` shell
# Get the parent commits

$ git show <merge commit sha>
commit <merge commit sha>
Merge: <parent 1 sha> <parent 2 sha>
# ...


```

## Settings

### Global settings

``` shell
git config --global user.name "Ville Outamaa"
git config --global user.email my@email.com
git config --global core.editor emacs
# etc
```
