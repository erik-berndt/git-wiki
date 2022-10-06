[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Branching

> HEAD is a pointer to the active branch (points on the latest commit by default).   
Commits are made (and shown) depending on where HEAD is pointing at.

List branches:  
**$ git branch**

Create new branch:  
**$ git branch new_branch**

Switch to branch:  
**$ git switch branch_name** *(formerly git checkout branch_name)*  

Create and switch directly:  
**$ git switch -c new_branch**  

or  
**$ git checkout -b new_branch**  


Delete local branch:  
**$ git branch -d branch_name**  

or use **-D** for *unmerged* branches  




