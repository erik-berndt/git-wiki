[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Branching

> HEAD is a pointer to the active branch (points on the latest commit by default).   
Commits are made (and shown) depending on where HEAD is pointing at.  
The HEAD file in .git references to the active branch (ref/heads/branch_name)  
and contains the latest commit-hash from that branch.  


List branches:  
``` 
$ git branch 
$ git branch -v         - info about last commit
```
Switch to branch:  
```
$ git switch <name> 
$ git checkout <name>
```   
list all remote branches of a cloned repo
```
$ git branch -r 
  origin/HEAD -> origin/main
  origin/fantasy
  origin/food
  origin/main
  origin/more-fantasy
  origin/morefood
  origin/movies
```

Switch to remote branch:  
```
$ git switch <name> 
$ git checkout <name>
```   
Detached-HEAD mode:
``` 
$ git switch origin/<name>
$ git checkout origin/<name>
```

once you switched branches you can toggle  
`$ git switch -`  
you cannot toggle back to Datached-HEAD mode   

Create new branch:  
`$ git branch <name>`


Create and switch directly: 
``` 
$ git switch -c <name>  
$ git checkout -b <name>  
```

Delete local branch:
```  
$ git branch -d <name>  
$ git branch -D <unmerged branch>  or -df
```  

Rename branch:
> To rename a branch you first must switch into it!  

`$ git branch -M <new-name>`  
