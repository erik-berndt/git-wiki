[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Timetraveling and Undo

'Detached HEAD' state:

You can visit a former commit using  
```
$ git checkout commit-hash     - use commit hash to access
$ git checkout HEAD~1 [2..]    - move back in steps from current HEAD positon
```
HEAD is now pointing no longer to a branch but directly to a commit.  
To reattach HEAD use  
`$ git switch branch or master`  
or  
`$ git switch -`  


or you can create a new branch from here to continue in a different way.  

To undo unstaged changes in specific files or all files 
```
$ git checkout HEAD filename
$ git checkout HEAD *.txt
$ git checkout HEAD *
```
or just  
`$ git checkout -- filname / *.txt / *`  

### Restore

> A newer command that does the same as checkout HEAD **and more !**

```
$ git restore filename
$ git restore *.txt
$ git restore *
```
but also you can restore an earlier state  
`$ git restore --source HEAD~2 filename ...`  
which can be undone with the previous commands **until you stage!**  

to **unstage** one or more files use  
`$ git restore --staged filename ... `  
as shown in `$ git status`    

### Plain reset

Reset the repo to a specific commit  
`$ git reset <commit-hash> `  
later commits **are gone !** but the changes are still there!  
The changes are unstaged now and can be taken to a new branch to be committed there.  
 
### Hard reset

`$ git reset --hard <commit-hash>`  
later commits **and changes are gone!**  

### Revert

Creates a new commit which reverts the changes but keeps them in the unreverted commit.  
`$ git revert <commit-hash>`
