# Git Command
- Version control System is a tools that help to tack changes in code
- git is a version control system
# Github
- Websit that allows developers to stor and manage therir code using Git.
#
# Configuring git
- `SYSTEM` : All users
- `GLOBAL` : All repositories of the current user
- `LOCAL`  : The current repository
```
git config --global user.name "<My Name>"
git config --global user.email "<someone@email.com>"
git config --list
```
`git config --global -e` : to edit global config file

# Clone & Status
- Clone - Cloning a repository on our local machine
  ```
  git clone <-some link->
  ```
- Status - displays the state of the code
  ```
  git status # -s for short 
  ```
# Git Status Track
- untracked : new files that git doesn't yet track
- modified  : changed
- staged    : file is ready to be committed
- unmodified : unchanged

# Add & Commit

- `add` - adds new or changed files in your working directory to the Git staging area.
  ```
  git add <-file anme->
  ```
- `commit` = it is the record of change
  ```
  git commit -m "some message"
  
  git commit -a -m "some message" # to commit without add {-am}
  ```
# Push 

- `push` - upload local repo content to remote repo
  ```
  git push origin main
  ```
#
# Init Command 

- `init` - used to create a new git repo
  ```
  git init
  git remote add origin <-link-> # (<remote repo>)
  git remote -v (to verify remote)
  git branch    (to check branch)
  git branch-M main (to rename branch)
  git push -u origin main  # to set -u origin main to set as origin main
  ```
#
# Branch Commands
- `git branch` : to check branch
- `git brandh -M main` : to rename branch
- `git checkout <-branch name->` : to navigate
- `git checkout-b <-new branch name->` : to crate new branch
- `git brach-d <- Branch name ->` : to delete branch
  
# Merging Code
- Way 1
  `git diff <-branch name->` : to comare commits, branches, files & more
  `git merge <-branch name->` : to merge 2 branches
- Way 2
  `Create a PR`
  
# Pull Request
It lets you tell other about change you've pushed to a branc in a repository on GitHub.

# Pull Command 
`git pull origin main`
used to fetch and download content from a remote repo and immediately update the local repo to match that content.

# Resolving Merge Conflicts
an event that takes place when Git is unable to automatically resolve differences in code between two commits.
#
# Undoing changes
- Case 1 : staged changes
  `git log`
  ```
  git reset <-file name->
  git reset
  ```
- Case 2 : commited changes (for one commit)
  ```
  git reset HEAD~1
  ```
- Case 3 : commited changes(for many commits)
  ```
  git reset <-commit hash->
  git reset --hard <-commit hash->
  ```
  #
  # Fork
  A fork is a new repoitory that shares code and visibility settings with the original "upstream" reposioty.<br>
  for is a reough copy
   
