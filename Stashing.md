[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Stashing

*to stash: verstecken, bunkern*

Git stash lets you switch branches without committing the changes  
of the current branch.  
Uncommitted changes will come with you unless the brach you're switching to  
has own changes.  
Back on the branch you were coming from just pop stashed changes to get them back.

```
$ (branch) git stash
$ (branch) git switch master
$ (master) do something
$ (master) git switch branch
$ (branch) git stash pop
```

`git stash apply` lets you apply stashed changes to multiple branches without removing  
them from the stash.  
Conflicts must be resolved similarly to [merging](https://github.com/pytherik/learning-git/wiki/Merging).  

Multiple stashes are allowed.
```
$ (rainbow*) git stash list
stash@{0}: WIP on rainbow: 398b643 change fg color    - hash (398..) and description (change..) refer to commit
stash@{1}: WIP on rainbow: 398b643 change fg color
stash@{2}: WIP on rainbow: 398b643 change fg color

$ (rainbow*) git stash apply stash@{1}        - stash is kept in list
$ (rainbow*) git stash pop stash@{1}          - stash removed from list
$ (rainbow*) git stash drop stash@{1}         - remove without or after applying
$ (rainbow*) git stash clear                  - clear stash
```


