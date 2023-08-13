[←back to content](https://github.com/pytherik/learning-git/wiki/Content)
# Diffing

Changes in current branch
```
shows changes of all edited files or [filename]

$ git diff [filename]                         # only unstaged !
$ git diff HEAD [filename]                    # staged and unstaged since HEAD (last commit) !
$ git diff --staged [filename]                # only staged !
           --cached [filename]
```
accross branches
```
$ git diff branch1..branch2 [filename]        # compare two branches
$ git diff branch2 branch1  [filename]        # order does matter !
```
across commits
```
$ git diff hash1 hash2                        # compare two commits by its log-hashes
$ git diff hash2 hash1                        # order does matter !
```



