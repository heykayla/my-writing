# Git Commands Cheat Sheet

## Introduction

This cheat sheet lists all Git commands for users who are new to using Git or unfamiliar with many of the basic Git commands.

## Git Commands

### Navigating

Use the commands outlined in this section to navigate to different directories (folders) or files on your local computer.

| Command               | Definition                                                                                                                                                                           |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `pwd`                 | This command stands for _Print Working Directory_. You use this command to see your current file path.                                                                               |
| `pwd -p`              | This commands shows you the full file path you're currently in.                                                                                                                      |
| `cd <directory_name>` | This command stands for _Change Directory_. You use this command to enter and open a directory. Also, if you enter only `cd` or `cd ~`, you'll be directed back to your Home folder. |
| `cd ..`               | This command takes you to a directory above the one you're currently in.                                                                                                             |
| `cd -`                | This command takes you to the directory you were in before.                                                                                                                          |
| `ls`                  | This command lists all the files in a directory.                                                                                                                                     |
| `ls -a`               | This command lists all files and hidden files in a directory.                                                                                                                        |
| `ls -l`               | This command lists all directories in a directory.                                                                                                                                   |

### Creating

Use the commands outlined in this section to create new files and directories.

| Command                      | Definition                                                                                                                     |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `touch <filename.extension>` | This command creates a new and empty file. (e.g., `touch hello_world.md`)                                                      |
| `mkdir <directory_name>`     | This command stands for _Make Directory_. You use this command to create a new and empty directory. (e.g., `mkdir new_folder`) |

### Miscellaneous

The commands outlined in this section are helpful miscellaneous commands.

| Command                               | Definition                                                                      |
| ------------------------------------- | ------------------------------------------------------------------------------- |
| `clear`                               | This command clears the contents within the terminal.                           |
| `git mv <old_filename <new_filename>` | This command renames files.                                                     |
| `git status`                          | This command displays the current state of your repository or and staging area. |

### Configurating Git

Use the commands outlined in this section to setup and customize your [Git](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) enviroment on your local computer.

| Command                            | Definition                                                           |
| ---------------------------------- | -------------------------------------------------------------------- |
| `git config --<global user.name>`  | This commands sets your Git username. (e.g., `git config -heykayla`) |
| `git config --<global user.email>` | This command sets your Git email address.                            |

### Basic Workflow

Use the commands outlined in this section to perform the basic [Git workflow](https://uidaholib.github.io/get-git/3workflow.html).

| Command                     | Definition                                                                                                                                                                                               |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git clone`                 | This command clones a repository to your local computer by entering `git clone https://github.com/uidaholib/gitworkshop.git`. You can use either an HTTPS or SSH URL for cloning a repository.           |
| `git status`                | This commands tells the current state of your repository.                                                                                                                                                |
| `git add .`                 | This command stages your files after applying changes. The `git add .` command tells Git that you've made changes to a file and that you would like Git to track the file.                               |
| `git commit -m "<message>"` | This command saves the changes you've made to a file. You use this command after staging the file. Within the quotation marks, you can enter a message that summarizes the changes you made to the file. |
