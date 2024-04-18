# Git Commands #

## git init -
initialize a new Git repository in the current directory or in a specified directory. When you run git init, Git creates a new subdirectory named .git within the current directory. This directory contains all of the necessary files for your repository, including the repository's metadata and configuration.

## git remote add origin https://github.com/suneelreddy12/FSDGIT -
The git remote add origin command is used to add a remote repository to your local Git repository. In this command, "origin" is just a conventional name for the remote repository, but you can choose any name you like.

## git branch -
git branch command is used to list, create, or delete branches in a Git repository. When used without any arguments, it lists all the branches in your repository and highlights the currently active branch.
- git branch <branch_name> -> creates new branch with specified name.
- git branch -d <branch_name> -> this command deletes the specified branch. If the branch has unmerged changes (commits that are not in the branch you're currently on), Git will refuse to delete it unless you use the -D option, which forces the deletion.
- git branch -M <new_branch_name> -> The git branch -M <branch_name> command is used to rename an existing branch to the specified <branch_name>. The -M option is shorthand for -m --move, which indicates that you want to move or rename the branch.

## git add . -
The git add . command is used to add all changes in the current directory and its subdirectories to the staging area in Git. The dot (.) represents the current directory.

- It stages all changes to files in the current directory and its subdirectories.
- This includes new files, modified files, and deleted files.
- After running git add ., the changes are ready to be included in the next commit. It's important to note that git add . stages all changes, so you should review the changes using git status before committing to ensure you're including the correct modifications. If you only want to add specific files, you can use git add <file> to add individual files or git add <directory> to add all files within a specific directory.

## git commit -m "<commit-msg>" -
In the git commit command, the -m flag is used to specify the commit message directly in the command line, without opening a text editor. However, when providing the commit message using the -m flag, you should enclose the message within quotation marks.

## git pull -
When you run git pull without specifying any additional parameters, Git will attempt to fetch changes from the remote repository and merge them into your current branch.

1) Fetch: Git retrieves any new commits from the remote repository that you don't have in your local repository.
2) Merge: Git automatically merges the fetched commits into your current branch. If there are no conflicts, the merge will be completed automatically. However, if there are conflicts, Git will pause the process and allow you to resolve them manually before completing the merge.
If you're on the "master" branch and want to pull changes from the remote "master" branch, you can simply run: git pull origin master
This command tells Git to fetch changes from the "master" branch of the remote named "origin" and merge them into your current branch.

## git push -u origin master -
The git push -u origin master command is used to push the commits from your local "master" branch to the remote repository named "origin" and set up tracking so that future git pull or git push commands without specifying the branch and remote will automatically refer to this branch and remote.

Here's what each part of the command does:

1) git push: This command is used to push commits from your local repository to a remote repository.
1) -u: This flag stands for "upstream." When used with git push, it sets up tracking information so that your local branch is connected to a remote branch. After setting up tracking, future git pull or git push commands without specifying the branch and remote will automatically refer to this branch and remote.
3) origin: This is the name of the remote repository where you want to push your changes. In most cases, "origin" is the default name for the remote repository you cloned from, but you can have multiple remotes with different names.
4) master: This is the name of the branch you want to push to the remote repository. In this case, you're pushing changes from your local "master" branch to the "master" branch on the remote repository.