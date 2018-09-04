# Git best practices

## Know your git configuration

Configuration may come from these sources:

### List config for repository (from .git/config)
```
git config --local --list 
```
### List config for user (from ~/.gitconfig)
```
git config --global --list
```
### List config for user (from $GIT_INSTALL_DIR/gitconfig)
```
git config --system --list
```

## autostash
> When set to true, automatically create a temporary stash before the operation begins, and apply it after the operation ends. This means that you can run rebase on a dirty worktree. However, use with care: the final stash application after a successful rebase might result in non-trivial conflicts. Defaults to false.

Replaces:
```
git stash
git checkout <branch>
git stash pop
```

## autosquash

