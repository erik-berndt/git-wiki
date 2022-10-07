[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Configuration

git config --global user.name "Your Name"
git config --global user.emil "Your Email"

show name and email

git config user.name
git config user.email

# .gitconfig

```
name = pytherik
email = erikberndt@gmx.net

[alias]
    lg = "log --color --graph --pretty=format:'%Cred%h%Creset %Cgreen(%cr) %C(bold blue)<%an>%Creset -%C(yellow)%d%Creset %s' --abbrev-commit"

[color]
    ui = auto
[init]
    defaultBranch = master
[pull]
    rebase = false

```