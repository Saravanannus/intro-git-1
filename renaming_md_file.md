# How to rename the .md file after upload the file from local repository to remote repository 

Renaming a .md file (or any file) in a Git repository after it has been uploaded to a remote repository involves several steps. You'll need to rename the file locally, commit the change, and then push the updated commit to the remote repository.

Here’s how you can do it:

# 1. Rename the File Locally
Use the git mv command to rename the file within your local repository. This command handles the renaming and stages the change for you.

git mv old_name.md new_name.md

# For example:

git mv README.md README_NEW.md

# 2. Commit the Change
After renaming the file, you need to commit the change to your local repository.

git commit -m "Renamed README.md to README_NEW.md"

# 3. Push the Change to the Remote Repository
Finally, push the commit with the renamed file to the remote repository.

git push origin main

Replace main with the name of your branch if you're not working on the main branch.