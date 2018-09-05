# Git right

## Best practices
- autoSquash + --fixup
-- git rebase <origin> <branch> --interactive --autosquash
-- git config --global alias.rbi "rebase --interactive" 
-- git config --global rebase.autosquash true 
-- git rbi <origin> <branch> 

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

## fatal: The current branch dev has no upstream branch.

Tired of:

```
~/git/git-intro  on  dev △  $ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev
```

then do: 

```
git config --global push.default true

```
## --fixup

```
git
```

## References
https://www.praqma.com/stories/git-autostash/
https://robots.thoughtbot.com/autosquashing-git-commits
