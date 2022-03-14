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

Open your local computer's terminal or use your text editor's built-in terminal to enter commands.

### Step 2: Open your repository

Perform the following steps to locate and open your cloned repository:

1. See your current local path on your computer by running the `pwd` command.
2. Run `ls` to see your cloned repository listed.
3. To go inside your cloned repository on your local computer, run `cd` followed by the name of the cloned repository.
4. Re-run `ls` to see a list of all your current files within your cloned repository. If it's a new repository, you should only see your README.md file.

### Step 3: Validate your Git configuration settings

Check if you have Git properly configured on your local computer by running the `git config -l` command. The output should list your Git username, email, along with other details.

```
Kaylas-Air:How-to-Guides kaylamorales$ git config -l
credential.helper=osxkeychain
user.name=heykayla
user.email=kannmorales@gmail.com
core.editor=vs code --wait
core.excludesfile=/Users/kaylamorales/.gitignore_global
color.ui=true
difftool.sourcetree.cmd=opendiff "$LOCAL" "$REMOTE"
difftool.sourcetree.path=
mergetool.sourcetree.cmd=/Users/kaylamorales/Applications/Sourcetree.app/Contents/Resources/opendiff-w.sh "$LOCAL" "$REMOTE" -ancestor "$BASE" -merge "$MERGED"
mergetool.sourcetree.trustexitcode=true
commit.template=/Users/kaylamorales/.stCommitMsg
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
```

### Step 4: Create a new file

To **create** a new file in your cloned repository on your local computer, run the `touch` command followed by the title of the file you're creating.

```
Kaylas-Air:How-to-Guides kaylamorales$ git touch hello_world.md
```

### Step 5: Stage your file

Upon creating the file and making changes to it (if applicable), it's time to stage it by running the `git add .` command.

```
Kaylas-Air:How-to-Guides kaylamorales$ git add .
```

You will not see an output after running the command.

### Step 6: Commit file

Next, you will need to save your file and its changes by running `git commit -m "<message>"`. Within the quotation marks, enter brief description about your file.

```
Kaylas-Air:How-to-Guides kaylamorales$ git commit -m "Initial commit"
```

Afterward, you should see a similar output:

```
[main a50f2b4] Initial commit.
 1 file changed, 104 insertions(+), 31 deletions(-)
 rewrite How-to-Guides/hello_world.md (87%)
```

### Step 6: Push the file to your remote repository

Now that you've committed your file, you can push (publish) your file to your main branch into your remote repository (GitHub.com) by running the `git push` command.

## See also

Include references and/or links to other related documentation, either internal to the project or external.
After a leading sentence on why/how they are valuable to readers of the current topic, multiple related can be displayed in a list:

- One list for a small number of items, which can contain internal and external references, or;
- Two lists, divided into internal and external and separated by another leading sentence, if there are a larger number of items.
