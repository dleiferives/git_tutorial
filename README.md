# GIT Tutorial
## Tutorial for getting acquainted with Git/Github

## *"Git is to GitHub as videos are to YouTube"*
GitHub is just one place to house git-managed repositories and offers some very nice tools e.g., code comparisons, pull requests, easy collaboration, etc. GitLab is another tool similar to GitHub.

Download Git: https://git-scm.com/downloads

## Git Cheat Sheet:
`git status`    View status of current branch (e.g., modified/deleted/added files)

`git add`   Add file changes (modify/add/delete) to the **staging area**. Nothing in the **staging area** has been committed *yet* 

&emsp;&emsp;`-A`    Adds all modified files to the staging area

&emsp;&emsp;`--patch`   Allows you to split the modifications into separate commit hashes/messages 

`git commit`    Commit all files in the staging area. This effectively creates a local checkpoint/savepoint. Collaborators will **not** see these changes yet

&emsp;&emsp;`-m` Flag to add commit message. Commit messages should be descriptive and are required for all commits.

&emsp;&emsp;`-am`   Can use this in place of `git add -A` to quickly add all files and attach a commit message

`git push`  Will push all local commits to the remote branch (e.g., from local computer to GitHub)

&emsp;&emsp; `-f`   Force push. Will override any merge conflicts

`git clone` Clone git repository to the local directory

`git pull` Pull any changes made on the remote branch into local branch

`git branch` View all local branches

&emsp;&emsp; `-d` Delete specified branch

`git checkout`  Switch to another local branch. Will require that all currently modified files either be restored, stashed, or committed. Can also checkout to a previous commit hash

&emsp;&emsp; `-b` Create new branch if specified branch doesn't exist

`git rebase` Rebase current branch off specified branch. Useful to avoid merge commits

&emsp;&emsp; `-i` Interactive mode

`git merge` Merge specified branch into current branch (e.g., `git merge emergencyFix`)

`git restore` Restore specified files to their most recent commit

`git stash` Save current changes in a stash and revert changes to most recent commit. Stashes can be re-applied at later times and are saved in a stack-like data structure.

`git diff` View all differences made in specified files/branches
