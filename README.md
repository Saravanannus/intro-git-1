# Intro-Git1-module -3

# 1. Listing Branches

git branch: Lists all the branches in the current repository. The current branch is highlighted with an asterisk (*).

# 2. Creating a New Branch

git branch <branch_name>: Creates a new branch with the name <branch_name> but does not switch to it.

For example: git branch feature-x creates a branch named feature-x.

# 3. Switching to a Branch

git checkout <branch_name>: Switches to the specified branch.

Alternatively, you can use git switch <branch_name> (a newer command introduced in Git 2.23).

# 4. Creating and Switching to a New Branch

git checkout -b <branch_name>: Creates a new branch and immediately switches to it.

For example: git checkout -b feature-x creates and switches to the branch feature-x.

# 5. Deleting a Branch

git branch -d <branch_name>: Deletes the specified branch (if it has been merged).

git branch -D <branch_name>: Forces the deletion of the specified branch (even if it hasn’t been merged).

# 6. Renaming a Branch

git branch -m <new_name>: Renames the current branch to <new_name>.

git branch -m <old_name> <new_name>: Renames a specific branch from <old_name> to <new_name>.
