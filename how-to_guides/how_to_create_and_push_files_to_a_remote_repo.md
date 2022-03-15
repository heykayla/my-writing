# How to Create and Push Files to a Remote Repository

## Overview

This how-to article covers instructions for creating and pushing new files to a remote repository using the command line.

## Before you start

Before you begin, make sure you meet these prerequisites:

- Have a GitHub account
- Have Git installed and configured on your local computer
- Have a repository created and cloned to your local computer
- Have a text editor downloaded on your local computer (e.g., VS Code, Atom, etc.)

## Step-by-step guide

### Step 1: Open your terminal

Open your local computer's terminal or use your text editor's built-in terminal to run commands.

### Step 2: Open your cloned repository

Perform the following steps to locate and open your cloned repository:

1. See your current local path on your computer by running the `pwd` command.
2. Run `ls` to see your cloned repository listed.
3. To go open your cloned repository, run `cd` followed by the name of the cloned repository.

```
>:$ cd <cloned_repo_name>
```

4. Re-run `pwd` to validate that you have opened your cloned repository.

### Step 3: Validate your Git configuration settings

Check your Git configuration settings on your local computer by running the `git config -l` command. The output should list your Git username, email, along with other details.

```
>:$ git config -l
credential.helper=osxkeychain
user.name=<gitusername>
user.email=<gitemail>
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

> 🚩 **NOTE**: Your output may not exactly replicate the example shown above.

### Step 4: Create a new file

To **create** a new file in your cloned repository, run the `touch` command followed by the filename you're giving it.

```
>:$ git touch hello_world.md
```

### Step 5: Stage your file

Upon creating the file and making changes (if applicable), it's time to stage it by running the `git add .` command.

```
>:$ git add .
```

You will not see an output after running the command.

### Step 6: Commit file

Next, save your file and its changes by running `git commit -m "<message>"`. Within the quotation marks, enter a brief description of your file.

```
>:$ git commit -m "Initial commit"
```

Afterward, you should see a similar output:

```
[main a50f2b4] Initial commit.
 1 file changed, 104 insertions(+), 31 deletions(-)
 rewrite How-to-Guides/hello_world.md (87%)
```

### Step 6: Push the file to your remote repository

Now that you've committed your file run `git push` to publish your changes to your remote repository (GitHub.com).

## See also

- [Signing up for a new GitHub account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account)
- [1.5 Getting Started - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [1.6 Getting Started - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
- [Create a repo](https://docs.github.com/en/get-started/quickstart/create-a-repo)
- [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
