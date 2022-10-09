[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Basic Commands Overview

Initialize local repository

First make sure you're not in an existing repository  
`$ git status`  

```
$ git init <repo>
$ cd <repo>
```
after creating the first file e.g. README.md
```
$ git add <file> or
$ git add .                - stage your changes
$ git commit -m 'comment'  - commit staged changes, comment required!
```
Now you're on the master-branch.  
You can now push it to a [Github repository.](https://github.com/pytherik/learning-git/wiki/Github-Basics)

```
$ git status         - info about staged and unstaged changes
$ git log            - info about commit history
```
To get a nicer looking output from *git log*
you can configure shortcuts for aliases in the [.git/config file.](https://github.com/pytherik/learning-git/wiki/Configuration)
