# git Command 
- `git ls-files` : see the file in staging area
# Remove
- `git rm <file>` : remove file
- `git rm --cached -r <file>` : remove from the stageing area
# 
# Rename or Moving fille
- `mv <file.txt> <main.js>` : rename file in git
    - You can't able to add the rename file
    - `git add file.txt`
    - `git add main.js` : now see in git status
- `OR`
  - git mv main.js file.js

# Ignoring Files
- Create file **`.gitignore`** add file name or path to it to `ignore`
- Gitignore tample
```
github.com/github/gitignore
```

