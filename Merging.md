[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Merging

- we merge branches *not* commits
- HEAD is on the receiving branch (switch to where you merge into)

The fast **forward merge** is the simplest merge. It merges the another branch to let  
the master branch catch up with the progress made.  
**Only works when master stays unmodified.**
```
$ (branch) git switch master  
$ (master) git merge branch
``` 

### Handle conflicts

```
<<<<<<<< HEAD
This is the code modified by HEAD:
some code  
some more code
========
This confliction code from the branch:
some other code
>>>>>>>> bug-fix (branch)
``` 
- open conflicting files
- edit file(s) to remove conflicts by deciding which content  
you want to keep
- remove conflict markers (<<<, ===, >>>>)
- git add changes and git commit
