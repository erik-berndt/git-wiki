[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Configuration

git config --global user.name "Your Name"
git config --global user.emil "Your Email"

show name and email

git config user.name
git config user.email

# .gitconfig 

`1 # Das ist Gits benutzerspezifische Konfigurationsdatei.
 2 [user]
 3 # Bitte passen Sie die folgenden Zeilen an und kommentieren     Sie diese aus:
 4 name = pytherik
 5 email = erikberndt@gmx.net 
 6
 7 [alias]
 8 lg = log --topo-order --all --graph --date=local --pretty=fo    rmat:'%C(green)%h%C(reset) %><(55,trunc)%s%C(red)%d%C(reset)     %C(blue) 
   [%an]%C(reset) %C(yellow)%ad%C(reset)%n'
 9 [color]
10   ui = auto
11 [init]
12   defaultBranch = master 
13 [pull] 
14   rebase = false`
