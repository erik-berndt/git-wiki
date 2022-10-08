[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Branching

> HEAD is a pointer to the active branch (points on the latest commit by default).   
Commits are made (and shown) depending on where HEAD is pointing at.  
The HEAD file in .git references to the active branch (ref/heads/branch_name)  
and contains the latest commit-hash from that branch.  


List branches:  
`$ git branch [-v] [info last commit]` 

Create new branch:  
`$ git branch new_branch`

Switch to branch:  
`$ git switch branch_name` *(formerly git checkout branch_name)*   
once you switched branches you can toggle  
`$ git switch -`
 

Create and switch directly:  
`$ git switch -c new_branch`  

or  
`$ git checkout -b new_branch`  


Delete local branch:  
`$ git branch -d branch_name`  

> use `-D` or `-df` for *unmerged* branches  

Rename branch:
> To rename a branch you first must switch into it!  

`$ git branch -M new_name`  
