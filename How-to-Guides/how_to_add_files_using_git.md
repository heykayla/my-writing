# How to Create and Clone a GitHub Repository and Push New Files Using the Command Line

## Introduction

This how-to guide shares instructions on:

- Creating a new GitHub repository on your GitHub.com account
- Cloning your GitHub repository from your GitHub.com account to your local computer
- Creating a new file in your cloned repository on your local computer
- Pushing your new file from your local computer to your GitHub.com repository

To complete the steps, you will need to have Git installed on your computer and be using the command line on your local computer.

## Instructions

1. Go to your [GitHub.com](http://wwww.github.com) account and create a repository with a README.md file.
2. Copy your repository's HTTPS address.
   ![Copying repo's HTTPS address](https://github.com/heykayla/Technical-Writing-Portfolio/blob/main/Images/how_to_add_files_using_git/image3.png)
3. Open your local computer's terminal to enter commands.
4. To check your Git configuration settings, enter the `git config -l` command. You should see your GitHub username and email appear after running the command.
5. Clone your repository from you GitHub.com to your local computer by entering `git clone` followed by the HTTPS address.
6. See you current local path on your computer by entering the `pwd` command.
7. Enter `ls` to see all your directories within your current local path. You should see your cloned repository listed.
8. To go inside your cloned repository on your local computer, enter `cd` followed by the name of the cloned repository.
9. Enter `ls` to see a list of all your current files within your copied repository. You should only see your README.md file.
10. To create a new file, enter `touch` followed by the name of the file you'd like to create (e.g., `touch helloworld.md`).
11. Enter `git add .` to stage the file for a commit.
12. To push the file to your GitHub.com account, enter `git commit -m` followed by a message within quotation marks (e.g., `git commit -m "Initial file creation"`).
13. Run `git push` to publish the new file into your GitHub.com repository.
