# How to Add a Files to a GitHub Repository Using the Command Line

1. Go to your GitHub.com account and create a repository with a README.md file.
2. Copy your repository's HTTPS address.
3. Open your local computer's terminal and enter the following commands:
   - `git config -l` to check your Git configuration settings. You should see your GitHub username and email appear after running the command.
   - `git clone` and paste the HTTPS address to copy your repository from your GitHub.com account to your local computer.
   - `pwd` to see your current local path.
   - `ls` to see all your directories within your current local path. You should see your copied repository listed.
   - `cd` followed by the name of your copied repository to go inside it on your local computer.
   - `ls` to see a list of all your current files within your copied repository. You should only see your README.md file.
   - `touch` followed by the name of the file you'd like to create (e.g., `touch helloworld.md`).
4. Open your text editor.
5. Open the file you created.
6.
