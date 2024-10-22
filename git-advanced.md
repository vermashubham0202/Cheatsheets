# Advanced Git Commands
## Cherry-pick (Apply commits from another branch):
This command is handy when you want to apply a specific commit from one branch to another.
```
git cherry-pick <commit-hash>
```
## Rebase (Reapply commits on top of another base):
Useful for keeping your history clean and avoiding unnecessary merge commits.
### - Interactive rebase (allows squashing or editing commits)
```
git rebase -i <commit-hash>
```
### - Rebase current branch onto another branch
```
git rebase <branch-name>
```
## Squash Commits (Combine multiple commits into one):
While using rebase interactively, you can squash multiple commits into a single one.
### - n = number of previous commits to include
```
git rebase -i HEAD~n
```
## Bisect (Finding the commit that introduced a bug):
This command helps to find the specific commit that introduced a bug.
```
git bisect start
```
### - Mark current commit as bad
```
git bisect bad
```
### - Mark a known good commit
```
git bisect good <commit-hash>
```
### - Stop the bisect process
```
git bisect reset
```
## Git Blame (View who modified each line):
Helpful for tracking down changes in a specific line of code.
```
git blame <file-name>
```
## Git Archive (Create a ZIP or tarball of the repository):
Useful when you want to package the repository for deployment or sharing.
```
git archive --format=zip HEAD > archive.zip
```
## Git Restore (Undo changes in the working directory):
This is a more modern replacement for `git checkout` when restoring files.
### - Restore file to last commit
```
git restore <file-name>
```
### - Restore to staging area
```
git restore --staged <file-name>
```
## Reset to a specific commit without deleting local changes:
If you want to move to a specific commit but retain your current changes, you can use:
```
git reset --soft <commit-hash>
```
## Reflog (View local reference logs for debugging):
Git stores a history of updates to the tip of branches, which can help recover lost commits.
```
git reflog
```
## Submodule Management:
If your project uses Git submodules (external repositories within the main project), the following commands are essential:
### - Add a new submodule
```
git submodule add <repo-url> <path>
```
### - Initialize and clone all submodules
```
git submodule update --init --recursive
```
### - Remove a submodule
```
git submodule deinit <submodule-path>
```
```
git rm <submodule-path>
```
```
rm -rf .git/modules/<submodule-path>
```
## Tagging a Release:
While you have the basic tag commands, here's an extended flow for creating annotated tags for releases:
### - Create a lightweight tag
```
git tag <tag-name>
```
### - Create an annotated tag
```
git tag -a <tag-name> -m "Release message"
```
## Working with Upstream Repositories:
If you're working with a forked repository, this can be useful for syncing changes from the original repository.
### - Add upstream repository
```
git remote add upstream <url>
```
### - Fetch upstream changes
```
git fetch upstream
```
### - Merge upstream changes into the local branch
```
git merge upstream/master
```
## Prune Remote Branches:
Clean up remote-tracking branches that no longer exist on the remote.
```
git fetch -p
```
