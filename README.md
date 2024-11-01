# How Git Works
![Static Badge](https://img.shields.io/badge/git-grey?style=for-the-badge&logo=git)
![Static Badge](https://img.shields.io/badge/github-black?style=for-the-badge&logo=github)

If you're new to Git, this guide walks you through the essential resources to get started.

Follow the guide to help you get started and learn how Git works.

## Git commands on local machine
1. Start your project in your local machine cloning a GitHub repo or inizializing new repo:

    - git clone <"repo-url"> to cloning GitHub repo
    - git init <"repo-url"> to start new repo

2. Check git status and logs:

    - git status
    - git log --oneline
    - git diff <"main branch"> <"other branch"> to see the difference beetwen branches

3. Modify your project and update the git repo:

    - git add -A to adding all new files create in the projects or git add <"name of new file"> to add the new file
    - git commit -m <"message on new changing"> to save the modify and create a checkpoint
    - git commit -am to add new files and save

4. Create a new branch to add a new features to the project and when you create a new branch, it is on another timeline:

    - git branch to show the branches of the repo or git branch <"new branch"> to create new branch
    - git branch -m <"new name"> to rename actual branch
    - git branch -d <"branch name"> to delete branch

5. The git checkout command allows you to switch from one branch to another or restore working tree files:

    - git checkout <"id-commit"> we can take id-commit from git log to restore working tree
    - git checkout <"branch name"> or git switch <"branch name"> to switch to another branch
    - git checkout -b <"new branch name"> to create and switch on new branch

6. To merge changes made in another branch with the current branch:

    - git merge <"branch name">

7. Rebase is a way to move a branch to another place in the tree:

    - git rebase <"main branch">

8. Stash is useful when you've made changes in a branch, but you're not ready to commit them yet, but you'd like to move to another branch.

    - git stash save <"message">
    - git stash list to see stash area
    - git stash apply <"stash name"> applies the changes and leaves a copy in the stash area
    - git stash pop <"stash name"> applies changes and removes files from the stash area
    - git stash clear to delete all stash area

## Git commands on GitHub to remote repo

1. git push to merge current branch in local machine on remote repo or git push origin <"new branch"> to create new brach on remote repo
2. git pull is a git fetch + git merge from remote repo to local
3. git fetch read the difference beetwen remote repo and local. After fetch you can see the difference beetwen remote branch and local branch with git diff origin <"branch name">
