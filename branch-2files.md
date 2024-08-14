# 1. Git Branch

$ git branch -> list all branches in local repository

$ git branch <branch-name> -> to create new branch

$ git checkout <branch-name> -> to change branch

$ git checkout -b <branch-name> -> to create new branch and switch to that new branch

# 2. Renaming a Branch
git branch -m <new_name>: Renames the current branch to <new_name>.

git branch -m <old_name> <new_name>: Renames a specific branch from <old_name> to <new_name>

# After rename the branch how to update it from local repo to remote repo

Renaming a branch in your local Git repository and then updating it on the remote repository involves a few steps. 
Here's how you can do it:

# 1. Rename the Branch Locally
First, rename your branch in the local repository using the following command:

git branch -m old-branch-name new-branch-name
For example, to rename the branch feature-x to feature-y:

git branch -m feature-x feature-y

# 2. Delete the Old Branch on the Remote
Next, you need to delete the old branch from the remote repository. This step is necessary because renaming a branch locally does not automatically update the remote branch.

git push origin --delete old-branch-name
For example:

git push origin --delete feature-x

# 3. Push the New Branch to the Remote
Now, push the renamed branch to the remote repository:

git push origin new-branch-name
For example:

git push origin feature-y

# 4. Set the Upstream Branch
After pushing the new branch, you need to set the upstream tracking so that the local branch tracks the new remote branch:

git push --set-upstream origin new-branch-name

For example:

git push --set-upstream origin feature-y

# 5. Update References (Optional)
If other team members are using the old branch, you might want to notify them about the change. They will need to delete the old branch from their local repositories and check out the new one.

# Summary of Commands

git branch -m old-branch-name new-branch-name  # Rename the branch locally

git push origin --delete old-branch-name       # Delete the old branch from the remote

git push origin new-branch-name                # Push the new branch to the remote

git push --set-upstream origin new-branch-name # Set the upstream branch