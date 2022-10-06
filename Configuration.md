[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Configuration

git config --global user.name "Your Name"
git config --global user.emil "Your Email"

show name and email

git config user.name
git config user.email

# .gitconfig


name = pytherik  
email = erikberndt@gmx.net  


[alias]  

       lg = log --topo-order --all --graph --date=local --pretty=format:'%C(green)%h%C(reset) %><(55,trunc)%s%C(red)%d%C(reset) 
       %C(blue[%an]%C(reset) %C(yellow)%ad%C(reset)%n' 

[color]  

        ui = auto  
[init]  

        defaultBranch = master

[pull]

        rebase = false

