[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Basic Commands Overview

Initialize local repository

First make sure you're not in an existing repository  
`$ git status`  

```
$ git init <repo>
$ git cd <repo>
```
after creating the first file e.g. README.md
```
$ git add <file> or
$ git add .
$ git commit -m 'comment'
```
Now you're on the master-branch.


- git status
- git log 
  - git lg (custom alias created in [.config](https://github.com/pytherik/learning-git/wiki/Configuration))
  - git log --oneline
- git [branch](https://github.com/pytherik/learning-git/wiki/Branching) branch_name

