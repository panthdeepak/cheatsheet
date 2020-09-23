# 1. To track all remote branches, execute the following before `git pull --all`
```git branch -r | grep -v '\->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done```
