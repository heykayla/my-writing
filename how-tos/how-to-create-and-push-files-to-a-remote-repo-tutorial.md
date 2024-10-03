# How to Create and Push New Files to a Remote Repository

## Overview

This guide explains how to create and push new files to a remote repository (GitHub.com) with the command line. 

## Before you begin

Before you begin pushing new files to a remote repository, ensure that you have:

- Git installed and configured on your local computer
- A repository cloned to your local computer
- A text editor downloaded on your local computer, such as VS Code or Atom

## Step 1 — Open your terminal

The terminal provides a command line where you can enter text commands.

To open the terminal on your Mac computer, do the following:
1. Open **Launchpad**.
2. In the top search bar, enter **Terminal**.
3. From the search result, select **Terminal**.  

To open the terminal on your Windows computer, do the following:
1. Right-click the Start button.
2. From the drop-down menu, select Terminal. 

## Step 2 — Open your cloned repository

Cloned repositories are copies of remote repositories that are created on your local computer, allowing you to work on files within the repository locally.

To locate and open your cloned repository from your terminal, do the following:

1. To see your current location path on your local computer, run the `pwd` command.
2. To see a list of directories and locate your cloned repository, run the `ls` command.
3. To open your cloned repository, run the `cd` command followed by the name of the cloned repository.

```
>:$ cd Cloned_Repo_Name
```

4. To validate that you have opened your cloned repository, re-run the `pwd` command.

## Step 3 — Check your Git configuration settings

The Git configuration settings control how Git behaves on your local computer.

To check your Git configuration settings on your local computer, run the `git config -l` command in your terminal. The output should list your Git username, email, and other details.

```
>:$ git config -l
credential.helper=osxkeychain
user.name=<Git_Username>
user.email=<Git_Email>
core.editor=vs code --wait
core.excludesfile=/Users/kaylamorales/.gitignore_global
color.ui=true
difftool.sourcetree.cmd=opendiff "$LOCAL" "$REMOTE"
difftool.sourcetree.path=
mergetool.sourcetree.cmd=/Users/<computername>/Applications/Sourcetree.app/Contents/Resources/opendiff-w.sh "$LOCAL" "$REMOTE" -ancestor "$BASE" -merge "$MERGED"
mergetool.sourcetree.trustexitcode=true
commit.template=/Users/<computername>/.stCommitMsg
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
```

> 🚩 **NOTE**:  Your outputs may differ from the output examples in this guide.

## Step 4 — Create a new file

To **create** a new file in your cloned repository, run the `touch` command followed by the filename you're giving it in your terminal.

```
>:$ git touch Filename.md
```

### Step 5 — Stage your file

Staging in Git is the process of preparing your file to be included in your next commit.

To stage the changes you made to the file, run the `git add .` command in your terminal.

```
>:$ git add .
```

**NOTE**: You will not see an output after running the command.

## Step 6 — Commit your file

Committing in Git is the process of saving your file from staging to the repository's history.

To commit your file, run the `git commit -m "<message>"` command in your terminal. Within the quotation marks, enter a brief description of your commit.

```
>:$ git commit -m "Commit_Message"
```

Afterward, you should see a similar output:

```
[main a50f2b4] Commit_Message.
 1 file changed, 104 insertions(+), 31 deletions(-)
 rewrite How-to-Guides/hello_world.md (87%)
```

## Step 7 — Push the file to your remote repository

Pushing in Git is the process of sending your file to your remote repository. 

To publish your changes to your remote repository, run the `git push` command in your terminal.

## See also

- [Signing up for a new GitHub account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account)
- [1.5 Getting Started - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [1.6 Getting Started - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
- [Create a repo](https://docs.github.com/en/get-started/quickstart/create-a-repo)
- [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)