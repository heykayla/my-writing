# Git Commands

## Introduction

This cheat sheet lists all Git commands for users who are new to using Git or unfamiliar with many of the basic Git commands.

## Git Commands Cheat Sheet

### Commands to Navigate

Use the commands outlined in this section to navigate to different directories (folders) or files on your local computer.

| Command  | Definition                                                                                                                                                                                            |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `pwd`    | This command stands for _Print Working Directory_. You use this command to see your current file path.                                                                                                |
| `pwd -p` | This commands shows you the full file path you're currently in.                                                                                                                                       |
| `cd`     | This command stands for _Change Directory_. You use this command to enter a directory by entering `cd directory_name`. If you enter only `cd` or `cd ~`, you'll be directed back to your Home folder. |
| `cd ..`  | This command takes you to a directory above the one you're currently in.                                                                                                                              |
| `cd -`   | This command takes you to the directory you were in before.                                                                                                                                           |
| `ls`     | This command lists all the files in a directory.                                                                                                                                                      |
| `ls -a`  | This command lists all files and hidden files.                                                                                                                                                        |
| `ls -l`  | This command lists all directories in a directory.                                                                                                                                                    |

### Commands to Create

Use the commands in this section to create new files and directories.

| Command | Definition                                                                                                       |
| ------- | ---------------------------------------------------------------------------------------------------------------- |
| `touch` | This command creates a new and empty file by entering `touch filename.extension`. (e.g., `touch hello_world.md`) |
| `mkdir` | This command stands for _Make Directory_. You use this command to create a new and empty directory.              |

### Helpful Commands

The commands outlined in this section are helpful miscellaneous commands.

| Command      | Definition                                                                      |
| ------------ | ------------------------------------------------------------------------------- |
| `clear`      | This command clears the contents within the terminal.                           |
| `git mv`     | This command renames files by entering `git mv old_filename new_filename`.      |
| `git status` | This command displays the current state of your repository or and staging area. |

### Configuring Git

Use the commands in this section to setup and customize your [Git](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) enviroment on your local computer.

| Command                          | Definition                                                           |
| -------------------------------- | -------------------------------------------------------------------- |
| `git config --global user.name`  | This commands sets your Git username. (e.g., `git config -heykayla`) |
| `git config --global user.email` | This command sets your Git email address.                            |
