[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Merging

- we merge branches *not* commits
- HEAD is on the receiving branch (switch to where you merge into)

The fast **forward merge** is the simplest merge. It merges the another branch to let  
the master branch catch up with the progress made.  
**Only works when master stays unmodified.**

`$ (branch) git switch master`  
`$ (master) git merge branch`
