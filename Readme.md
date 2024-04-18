# Git Commands #

## git init -
initialize a new Git repository in the current directory or in a specified directory. When you run git init, Git creates a new subdirectory named .git within the current directory. This directory contains all of the necessary files for your repository, including the repository's metadata and configuration.

## git remote add origin https://github.com/suneelreddy12/FSDGIT -
The git remote add origin command is used to add a remote repository to your local Git repository. In this command, "origin" is just a conventional name for the remote repository, but you can choose any name you like.

## git branch -
git branch command is used to list, create, or delete branches in a Git repository. When used without any arguments, it lists all the branches in your repository and highlights the currently active branch.
-git branch <branch_name> -> creates new branch with specified name.
-git branch -d <branch_name> -> this command deletes the specified branch. If the branch has unmerged changes (commits that are not in the branch you're currently on), Git will refuse to delete it unless you use the -D option, which forces the deletion.
-git branch -M <new_branch_name> -> The git branch -M <branch_name> command is used to rename an existing branch to the specified <branch_name>. The -M option is shorthand for -m --move, which indicates that you want to move or rename the branch.

## git add . -
The git add . command is used to add all changes in the current directory and its subdirectories to the staging area in Git. The dot (.) represents the current directory.

-It stages all changes to files in the current directory and its subdirectories.
-This includes new files, modified files, and deleted files.
-After running git add ., the changes are ready to be included in the next commit. It's important to note that git add . stages all changes, so you should review the changes using git status before committing to ensure you're including the correct modifications. If you only want to add specific files, you can use git add <file> to add individual files or git add <directory> to add all files within a specific directory.


