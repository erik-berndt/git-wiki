[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Github basics

### Local Repositiries

1. Create repository on github - copy URL (HTTPS or SSH)

on your local machine:
```
$ git init <repository>
$ cd <repository>
$ touch README.md
$ git add README.md
$ git commit -m 'add README'
``` 
githubs new convention for master is main  
```
$ git branch -M main                 -optional, changes master to main  
$ git remote add origin <paste URL>
$ git push -u origin master/main
```
or  
2. Create repository on github - add README.md - copy URL (HTTPS or SSH)

on your local machine
```
$ git clone <paste URL>
$ cd <repository>
``` 
### SSH
if you have an ssh connection use the SSH-URL of the repository
```
$ git remote add origin git@github.com:username/repository-name.git
``` 
**Changin origin from HTTPS to SSH or vice versa**
```
$ git remote remove origin
$ git remote add origin SSH-URL or HTTPS-URL
```

**Changing or deleting the passphrase**

`$ ssh-keygen -p`
will ask for the location, in my case `~/.ssh/id_ed25519`  
You're now prompted for the old passphrase and the new passphrase.  
Leave blank for No Passphrase.  

### Push

Syntax
``` 
$ git push --set-upstream origin <branch>  or
$ git push -u origin <branch>
```
- git push -u
  - command, -u sets upstream for the branch you push    
(if set: use only `$ git push` for further uploads of that branch)  
- origin
  - conventional name for destination information (you can call it what you like
  - stored in `$ git remote -v` 
- branch 
  - select the branch you want to push (master or main or every other existing branch)  

