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

or you can create a new branch from here to continue in a different way.  

