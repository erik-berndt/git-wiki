[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Add and Commit

Add single files:  
`$git add filename1 filename2 ...`  

Add all:  
`$git add .`  

Commit:  
`$ git commit -m 'comment'`  

Write comment in editor:  
`$ git commit`

Add all and commit:  
`$ git commit -a -m 'comment'`  

### amend

```
$ git commit -m 'initial commit'  
$ git add forgotten_file  
$ git commit --amend
$ git commit -m 'new comment for last commit' --amend
```
