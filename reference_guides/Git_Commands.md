# Git Commands Reference Guide

## Overview

This reference guide lists basic Git commands for novice users of Git.

## Git Commands

### Navigate

Use the commands outlined in this section to navigate different directories (folders) or files on your local computer.

| Command               | Definition                                                                                                                                                                           |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `pwd`                 | This command stands for _Print Working Directory_. You use this command to see your current file path.                                                                               |
| `pwd -p`              | This command shows you the full file path you're currently in.                                                                                                                       |
| `cd <directory_name>` | This command stands for _Change Directory_. You use this command to enter and open a directory. Also, if you enter only `cd` or `cd ~`, you'll be directed back to your Home folder. |
| `cd ..`               | This command takes you to a directory above the one you're currently in.                                                                                                             |
| `cd -`                | This command takes you to the directory you were in before.                                                                                                                          |
| `ls`                  | This command lists all the files in a directory.                                                                                                                                     |
| `ls -a`               | This command lists all files and hidden files in a directory.                                                                                                                        |
| `ls -l`               | This command lists all directories in a directory.                                                                                                                                   |

### Create

Use the commands outlined in this section to create new files and directories.

| Command                      | Definition                                                                                                                     |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `touch <filename.extension>` | This command creates a new and empty file. (e.g., `touch hello_world.md`)                                                      |
| `mkdir <directory_name>`     | This command stands for _Make Directory_. You use this command to create a new and empty directory. (e.g., `mkdir new_folder`) |

### Miscellaneous

The commands outlined in this section are helpful miscellaneous commands.

| Command                                | Definition                                            |
| -------------------------------------- | ----------------------------------------------------- |
| `clear`                                | This command clears the contents within the terminal. |
| `git mv <old_filename> <new_filename>` | This command renames files.                           |

### Configure Git

Use the commands outlined in this section to set up and customize your [Git](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) environment on your local computer for all repositories on your computer. (**NOTE:** Learn how to configure Git per repository by reading [Customizing Git - Git Configuration](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#_git_config).)

| Command                                      | Definition                                |
| -------------------------------------------- | ----------------------------------------- |
| `git config --global user.name "<username>"` | This command sets your Git username.      |
| `git config --global user.email "<email>"`   | This command sets your Git email address. |

### Basic Workflow

Use the commands outlined in this section to perform the [Git workflow](https://uidaholib.github.io/get-git/3workflow.html).

| Command                     | Definition                                                                                                                                                                                                                                    |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git clone`                 | This command clones a repository to your local computer by entering `git clone https://github.com/uidaholib/gitworkshop.git`. You can use either an HTTPS or SSH URL for cloning a repository.                                                |
| `git status`                | This command displays the current state of your repository and staging area.                                                                                                                                                                  |
| `git log`                   | This command lists all recent activities.                                                                                                                                                                                                     |
| `git add .`                 | This command stages your files after applying changes. The `git add .` command tells Git that you've made changes to a file and that you would like Git to track the file.                                                                    |
| `git commit -m "<message>"` | This command saves or takes a "snapshot" of the changes you've made to a file. You use this command after staging the file (`add .`). Within the quotation marks, you can enter a message that describes the changes you've made to the file. |
| `git push`                  | This command pushes the changes you've made to your local files in your cloned repository into your remote (GitHub.com) repository.                                                                                                           |
| `git push origin main`      | This command pushes changes from a different branch to the main branch.                                                                                                                                                                       |
| `git pull`                  | This command updates your repository by pulling updates from your remote repository and merging the updates with your local repository.                                                                                                       |
| `git fetch`                 | This command displays changes made in your remote repository; it does not merge any changes with your local repository.                                                                                                                       |

### Work with Remote Repositories

Use the commands outlined in this section to help you start working with remote repositories.
| Command | Definition |
|--|--|
| `git remote -v` | This command lists the URL of your remote repository in your terminal. The word _origin_ will appear at the start of your remote connection or remote repository's URL; origin is the default and convention for the remote repository. |
| `git init <directory>` | This command creates a new Git repository or can convert an existing local and unversioned directory into a Git repository. To convert a directory into a Git repository, make sure to open the directory using `cd` and enter `git init`. |
| `git branch --all` | This command lists all the branches within your repository. |
| `git checkout <branch_name>` | This command switches you to a different branch. |
| `git checkout -b <branch-name>` | This command creates a new branch and switches to it at the same time. |
| `git switch <branch_name>` | This command switches you to a different branch. (Git v2.23+) |
| `git switch -c <branch-name>` | This command creates a new branch and switches to it at the same time. (Git v2.23+) |
| `git branch -d -r origin/feature/<branch>` | This command deletes a local branch. |
| `git fetch add upstream <link>` | This command adds the upstream to your forked (copied) repository, allowing you to push changes to the original repository. When adding the upstream, make sure to use the HTTPS or SSH link (whichever one you chose for cloning the forked repository to your local computer). |
| `git fetch upstream main` | This command pulls any updates from the main branch of the forked repository to your local copy. |
