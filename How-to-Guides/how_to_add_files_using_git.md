# How to Add a Files to a GitHub Repository Using the Command Line

1. Go to your GitHub.com account and create a repository with a README.md file.
2. Copy your repository's HTTPS address.
   ![Copying HTTPS address](https://github.com/heykayla/Technical-Writing-Portfolio/blob/main/Images/how_to_add_files_using_git/image3.png)
3. Open your local computer's terminal.
4. Enter `git config -l` to check your Git configuration settings. You should see your GitHub username and email appear after running the command.
5. Enter `git clone` and paste the HTTPS address to clone your repository from your GitHub.com account to your local computer.
6. Enter `pwd` to see your current local path.
7. Enter `ls` to see all your directories in your current local path. You should see your cloned repository listed.
8. Enter `cd` followed by the name of your cloned repository to go inside your repository on your local computer.
9. Re-enter `ls` to see a list of all your current files within your repository. You should only see your README.md file.
10. Enter `touch` followed by the name of the file you'd like to create (e.g., `touch helloworld.md`).
11. Manually look for and open the file you created
