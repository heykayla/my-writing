# Git Commands

## Overview

This reference article contains the following information for beginner Git users:

- Commands to navigate directories and files.

- Commands to create directories and files.

- Commands to configure Git.

- Commands for miscellenous actions.

- Commands set up and work a remote repository.

## Commands to navigate

You can use the following commands  to navigate directories (folders) or files on your local computer.

| Command | Description  |
|--|--|
| `cd ..` | Takes you to a directory above the one you're currently in. |
| `cd <directory_name>` | Allows you to enter and open a directory. If you enter only `cd` or `cd ~`, you'll be directed back to your **Home** folder. |
| `cd -` | Takes you to the directory you were in before. |
| `pwd` | Shows your current file path. |
| `pwd -p` | Shows the full file path you're currently in. |
| `ls` | Lists all the files in a directory. |
| `ls -a` | Lists all files and hidden files in a directory. |
| `ls -l` | Lists all directories in a directory. |

## Commands to create and rename files and directories 

You can use the following commands to create new files and directories on your local computer.

| Command | Description |
|--|--|
| `git mv <old_filename> <new_filename>` | Renames files. Example: `git mv hello_world.md hello_universe.md` |
| `mkdir <directory_name>` | Creates an empty directory. Example: `mkdir new_folder` |
| `touch <filename.extension>` | Creates an empty file. Example: `touch hello_world.md` |

## Commands to configure Git

You can use the following commands to configure a [Git](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) enviroment for your repositories on your local computer.

**Note**: To learn how to configure Git, see [Customizing Git - Git Configuration](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#_git_config).

| Command  | Description |
|--|--|
| `git config --global user.name "<username>"` | Sets your Git username. |
| `git config --global user.email "<email>"` | Sets your Git email address. |

## Commands to perform Git workflow actions

You can use the following commands to perform actions a part of the [Git workflow](https://uidaholib.github.io/get-git/3workflow.html).

|Command| Description |
|--|--|
| `git clone` | Clones a repository to your local computer. You can use either an HTTPS or SSH URL for cloning a repository. Example: it clone https://github.com/uidaholib/gitworkshop.git. |
| `git status` | Displays the current state of your repository and staging area. |
| `git log` | Lists all recent activities. |
| `git add .` | Stages your files after applying and saving changes. The `git add .` command tells Git that you've made changes to a file and that you would like Git to track the file. |
| `git commit -m "<message>"` | Saves or takes a "snapshot" of the changes you've made to a file. Use this command after staging the file (`add .`). Within the quotation marks, you can enter a message that describes the changes you're committing. |
| `git push` | Pushes the changes you've made in your local repository to your remote (GitHub.com) repository.
| `git push origin main` | Pushes changes from a different branch to the main branch. |
| `git pull` | Updates your local repository by pulling and merging updates from your remote repository. |
| `git fetch` | Displays changes made in your remote repository. It does not merge any changes with your local repository. |
| `git remote -v` | Lists the URL of your remote repository in your terminal. The word _origin_ will appear at the start of your remote connection or remote repository's URL. Origin is the default and convention for the remote repository. |
| `git init <directory>` | Creates a new Git repository or can convert an existing local and unversioned directory into a Git repository. To convert a directory into a Git repository, open the directory using `cd` and enter `git init`. |
| `git branch --all` | Lists all the branches within your repository. |
| `git checkout <branch_name>` | Switches you to a different branch. |
| `git checkout -b <branch-name>` | Creates a new branch and switches to it at the same time. |
| `git switch <branch_name>` | Switches you to a different branch. (Git v2.23+) |
| `git switch -c <branch-name>` | creates a new branch and switches to it at the same time. (Git v2.23+) |
| `git branch -d -r origin/feature/<branch>` | Deletes a local branch. |
| `git fetch add upstream <link>` | Adds the upstream to your forked (copied) repository, allowing you to push changes to the original repository. When adding the upstream, make sure to use the HTTPS or SSH link (whichever one you chose for cloning the forked repository to your local computer). |
| `git fetch upstream main` | Pulls any updates from the main branch of the forked repository to your local copy. |
