[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Basic Commands Overview
## git docs

[Git-Reference](https://git-scm.com/docs)  
[Git-Book](https://git-scm.com/book/en/v2)  

## Initialize local repository

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
$ git status                  # info about staged and unstaged changes
$ git log                     # info about commit history
$ git log --pretty --oneline  # nicer looking output 
```
To get a nicer looking output from *git log*
you can configure shortcuts for aliases in the [.git/config file.](https://github.com/pytherik/learning-git/wiki/Configuration)

## Create remote repository from terminal

For that you need github cli on your computer:  
[Installation Guide](https://computingforgeeks.com/how-to-install-github-cli-on-linux-and-windows/?expand_article=1)  

Authorization for local computer  
```
$ gh auth login
```
follow the cli menu  

Now prepare the project you want to create the repository from:  
```
$ mkdir new_Project
$ cd new_Project
$ git init
$ gh repo create new_Project --public --source=. --remote=origin
```
done  
[github cli getting started](https://cli.github.com/manual/gh_repo_create)


