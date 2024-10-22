# Git Commands
## Installation:
```
sudo apt-get install git
```
```
git --version
```
## Configure Git:
### - For the current git repo
```
git config user.name "Shubham Verma"
```
```
git config user.email "example@domain.com"
```
### - For globally
```
git config --global user.name "Shubham Verma"
```
```
git config --global user.email "example@domain.com"
```
### - Set default editor and aliases
```
git config --global core.editor vim
```
```
git config --global alias.<your-alias-name> 'command-with-options'
```
## View Configuration:
```
git config --list
```
```
git config user.name
```
```
git config user.email
```
```
git config --get remote.origin.url
```
## Frequently Used Commands:
```
git fetch
```
```
git status
```
```
git init
```
```
git add <file_name>
```
### - same as: git add -A
```
git add .
```
```
git commit -m "message"
```
### - skip staging
```
git commit -a -m "message"
```
```
git commit --help
```
```
git commit --amend
```
## Checkout Files:
```
git checkout <commit-hash>
```
### - Dangerous commands (Below 2 commands):
```
git checkout -- <file-name>
```
### - Change all files to the previous commit
```
git checkout -f
```
## View Commits:
```
git log
```
### - n = 1, 2, 3, ...
```
git log -n
```
```
git log --oneline
```
```
git log --grep "keyword"
```
```
git log -p
```
### - n = 1, 2, 3, ...
```
git log -p -n
```
```
git log --stat
```
```
git log --pretty=oneline
```
```
git log --pretty=short
```
```
git log --pretty=full
```
### - h = hash, an = author name
```
git log --pretty=format:"%h - %an"
```
### - ae = author email (find all formatting on: git-scm.com)
```
git log --pretty=format:"%h - %ae"
```
```
git log --since=2.days
```
```
git log --since=2.weeks
```
```
git log --since=2.months
```
```
git log --since=2.years
```
```
git show <commit-id>
```
## Difference:
### - diff. b/w working area files v/s stage area files
```
git diff
```
### - diff. b/w stage area files v/s last commit files
```
git diff --staged
```
### - diff. b/w current-branch v/s branch-name
```
git diff <branch-name>
```
## Branches:
```
git branch
```
```
git branch --merged
```
```
git branch --no-merged
```
### - branches with last commit: hash-code and message
```
git branch -v
```
```
git branch <branch-name>
```
```
git checkout -b <new-branch-name>
```
### - commit before switching
```
git checkout <branch-name-to-move>
```
### - run from destination branch
```
git merge <branch-name>
```
```
git branch -d <merged-branch-name-to-delete>
```
```
git branch -D <unmerged-branch-name-to-delete>
```
## Tags:
```
git tag
```
```
git tag -a "tag-name" -m "message" <commit-id>
```
```
git show <tag-name>
```
```
git tag -d <tag-name>
```
## Renaming and Removing Files:
```
git rm <file-name>
```
```
git rm --cached <file-name>
```
```
git mv <old-file-name> <new-file-name>
```
## Remove Untracked Files:
### - dry-run
```
git clean -n
```
### - force removal
```
git clean -f
```
## Stashing:
```
git stash
```
```
git stash list
```
### - n = 0, 1, 2, 3, ...
```
git stash apply stash@{n}
```
```
git stash clear
```
## Reset (Before Commit):
### - same as: git restore --staged <file-name>
```
git reset <file-name>
```
### - for staging area (all files)
```
git reset .
```
### - for staging area and working directory both (all files)
```
git reset --hard
```
## Revert (After Commit):
```
git revert <wrong-commit-id>
```
## .gitignore:
```
vi .gitignore
```
### - after adding extensions or file names/directory in .gitignore file
```
git add .gitignore
```
## Stop Tracking Directory:
```
rm -rf .git
```
## Cloning:
```
git clone <url>
```
```
git clone <url> <custom-directory-name>
```
## Remote:
```
git remote
```
```
git remote -v
```
### - fetch commit history of the remote repo
```
git fetch origin
```
### - origin = remote-name (any-name), master = branch-name (any-name)
```
git push -u origin master
```
```
git push <remote-name> <branch-name>
```
```
git push origin <branch-name-in-local-repo>:<new-branch-name-in-remote-repo>
```
```
git push origin --all
```
### - pull = fetch + merge
```
git pull -u origin master
```
```
git remote add origin <remote-url>
```
### - origin (above command) can be replaced by any other name
```
git remote add <remote-name> <remote-url>
```
```
git push <remote-name> <new-remote-branch-name>
```
```
git push -d <remote-name> <branch-name>
```
### - Adding Multiple Remote URLs:
```
git remote set-url --add --push <remote-name> <remote-url-1>
```
```
git remote set-url --add --push <remote-name> <remote-url-2>
```











