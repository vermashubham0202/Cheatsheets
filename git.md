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
```
git log -n    # n = 1, 2, 3, ...
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
```
git log -p -n   # n = 1, 2, 3, ...
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
### h = hash, an = author name
```
git log --pretty=format:"%h - %an"
```
### ae = author email (find all formatting on: git-scm.com)
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

















