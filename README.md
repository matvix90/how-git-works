# howGitWorks

## Git Commands on local machine
- Start your project in your local machine cloning a GitHub repo or inizializing new repo:

    1. git clone <"repo-url"> to cloning GitHub repo
    2. git init <"repo-url"> to start new repo

- Check git status and logs:

    1. git status
    2. git log --oneline
    3. git diff <"main branch"> <"other branch"> to see the difference beetwen branches

- Modify your project and update the git repo:

    1. git add -A to adding all new files create in the projects or git add <"name of new file"> to add the new file
    2. git commit -m <"message on new changing"> to save the modify and create a checkpoint
    3. git commit -am to add new files and save

- Create a new branch to add a new features to the project and when you create a new branch, it is on another timeline:

    1. git branch to show the branches of the repo or git branch <"new branch"> to create new branch
    2. git branch -m <"new name"> to rename actual branch
    3. git branch -d <"branch name"> to delete branch

- The git checkout command allows you to switch from one branch to another or restore working tree files:

    1. git checkout <"id-commit"> we can take id-commit from git log to restore working tree
    2. git checkout <"branch name"> to switch
    3. git checkout -b <"new branch name"> to create and switch on new branch