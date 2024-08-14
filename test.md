# To Config your github account :

git config --global user.email "you@example.com" 

git config --global user.name "github_username" 

# for the first time cloning repo to local 
$ git clone 

need to change dir/folder to cloned repo 

$ git pull -> only after cloning. everytime if there is some changes on remote repo, then git pull will works. 

# Git Status check
$ git status -> to check the status of the repo.

# Git Add
$ git add . To add ALL changes made to stage.

$ git add <path/filename> -> to add specific changes made to stage. 

# Commit the file that you’ve staged in your local repository
$ git commit -m "Change on README.md" -> To commit changes to local repository 

# Push the changes in your local repository to GitHub!
$ git push -> to transfer all commits from local repository to remote repository 

# Branches
$ git branch -> list all branches in local repository 

$ git branch <branch-name> -> to create new branch 

# Switching Branch
$ git checkout <branch-name> -> to change branch 

$ git checkout -b <branch-name> -> to create new branch and switch to that new branch 

# Git Reset
$ git reset --hard

This discards all changes in your working directory and staging area, making your repository match the latest commit.

git reset --hard <commit> <commit>: This can be a specific commit hash, a branch name, HEAD~1 (the previous commit), or simply HEAD to reset to the latest commit.

If you don't specify a commit, git reset --hard will reset to HEAD, meaning it will discard all uncommitted changes in the working directory and staging area and keep the branch at the latest commit.
