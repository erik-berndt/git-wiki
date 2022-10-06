[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Basic Commands Overview

- git init
- git add .
- git commit -m 'comment'
- git remote add origin <https//:path to/repository.git>

- git status
- git log 
  - git lg (custom alias created in [.config](https://github.com/pytherik/learning-git/wiki/Configuration))
  - git log --oneline
- git [branch](https://github.com/pytherik/learning-git/wiki/Branching) branch_name

### amend

$ git commit -m 'initial commit'  
$ git add forgotten_file  
$ git commit --amend