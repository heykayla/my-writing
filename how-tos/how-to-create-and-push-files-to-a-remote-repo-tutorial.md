# How to Create and Push Files to a Remote Repository

## Overview

In this how-to, you’ll create and push new files to a remote repository (GitHub.com) with the command line. This how-to is intended for experts of GitHub. 

## Before you begin

Before you begin, you must ensure you meet the following prerequisites:

- Have a GitHub account.
- Have Git installed and configured on your local computer.
- Have a repository created and cloned to your local computer.
- Have a text editor downloaded on your local computer. For example, VS Code or Atom.

## Step-by-step guide

### Step 1: Open your terminal

To run commands, open your local computer's terminal or the text editor's built-in terminal.

### Step 2: Open your cloned repository

Perform the following steps to locate and open your cloned repository:

1. Run the `pwd` command to see your current local path on your computer.
2. Run `ls` to see your cloned repository listed.
3. Run `cd` followed by the name of the cloned repository to open your cloned repository.

```
>:$ cd <cloned_repo_name>
```

4. Re-run `pwd` to validate that you have opened your cloned repository.

### Step 3: Validate your Git configuration settings

To check your Git configuration settings on your local computer, run the `git config -l` command. The output should list your Git username, email, and other details.

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

> 🚩 **NOTE**:  Your output may not exactly replicate the examples in this how-to.

### Step 4: Create a new file

To **create** a new file in your cloned repository, run the `touch` command followed by the filename you're giving it.

```
>:$ git touch hello_world.md
```

### Step 5: Stage your file

After you create a file and make changes to it, it's time to stage it by running the `git add .` command.

```
>:$ git add .
```

You will not see an output after running the command.

### Step 6: Commit your file

To commit your file, run `git commit -m "<message>"`. Within the quotation marks, enter a brief description of your commit.

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

Now that you've committed your file, run `git push` to publish your changes to your remote repository.

## See also

- [Signing up for a new GitHub account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account)
- [1.5 Getting Started - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [1.6 Getting Started - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)
- [Create a repo](https://docs.github.com/en/get-started/quickstart/create-a-repo)
- [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
