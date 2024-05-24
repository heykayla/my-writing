# How to Create and Push Files to a Remote Repository

## Overview

In this how-to, you’ll use the command line to create and push new files to a remote repository (GitHub.com). 

This how-to is intended for intermediate to expert users of GitHub.

## Before you begin

Before you begin this how-to, you must have the following:

- Git installed and configured on your local computer
- A repository created and cloned to your local computer
- A text editor downloaded on your local computer, such as VS Code or Atom

## Step-by-step guide

### Step 1 — Open your terminal

To run commands, open your local computer's terminal or the text editor's built-in terminal.

### Step 2 — Open your cloned repository

In your terminal, do the following to locate and open your cloned repository:

1. To see your current location path on your local computer, run the `pwd` command.
2. To see a list of directories and locate your cloned repository, run the `ls` command.
3. To open your cloned repository, run the `cd` command followed by the name of the cloned repository.

```
>:$ cd Cloned_Repo_Name
```

4. To validate that you have opened your cloned repository, re-run the `pwd` command.

### Step 3 — Check your Git configuration settings

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

> 🚩 **NOTE**:  Your outputs may differ from the output examples in this how-to.

### Step 4 — Create a new file

To **create** a new file in your cloned repository, run the `touch` command followed by the filename you're giving it in your terminal.

```
>:$ git touch Filename.md
```

### Step 5 — Stage your file

After you create and edit the file, run the `git add .` command in your terminal to stage your changes.

```
>:$ git add .
```

**NOTE**: You will not see an output after running the command.

### Step 6 — Commit your file

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

### Step 7 — Push the file to your remote repository

To publish your changes to your remote repository, run the `git push` command in your terminal.

## See also

- [Signing up for a new GitHub account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account)
- [1.5 Getting Started - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [1.6 Getting Started - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
- [Create a repo](https://docs.github.com/en/get-started/quickstart/create-a-repo)
- [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)