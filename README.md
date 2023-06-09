# git_command
I am talking about git's command

## 1. git config

You are using git for the first time or have a new git installation. This command sets your identity with your name and email address.
```
git config –global user.name “Your name”

```
```
git config –global user.email “Your email”

```

## 2. git version

Used to check the Git version
```
git version

```

## 3. git init

is the first command you use to start a new project in Git. This command will create a new empty repository into which you can then store your source code.
```
git init

```
You can also include the name of the repository in the git init command
```
git init <your repository name>

```
## 4. git clone

The git clone command is used to copy an existing repository.
You use git clone when you need a copy of an existing repository. The git clone command first uses the git init command, then it will check all its contents.
```
git clone <your project URL>

```
## 5. git add

The git add command adds all new code files or edited files to the repository. This command provides various options for adding files and folders.

The following command adds a specific file to the stage area.
```
git add your_file_name

```
The following command adds all edited and new files to the stage area.
```
 git add *

 ```

## 6. git add

```
git add . 

```

## 7. committing on git

This is an essential command in Git. In fact, the git commit command will add the changes to the local repository.
```
git commit -m "writing text"

```
## 8. git status

git status is used to check the status of files and you can identify which files need attention. This command can be executed at any time.
You can use it between the Git add and Git commits commands to see the status.
```
git status

```
## 9. git branch

You can manage branches effectively with the git branch command. There are various Git branch options and switches.


1. List all branches
```
git branch
```

2. Create a new branch
```
git branch <branch_name>
```
3. Delete a branch

```
 git branch -d <branch_name>
```
## 10. git checkout

This command is used to switch between branches. It is one of the most powerful git commands and can be used as a multipurpose tool.

1. Go to another branch:
```
git checkout <branch_name>
```
2. You can create a new branch and switch to it:
```
git checkout -b <your_new_branch_name>
```

## 11. git remote

This command acts like a border around the tank. If you need to communicate with the world outside the repository, you should use the git remote command. This command connects the local repository to the remote one.

```
 git remote add <shortname> <url>
```

### 12. git pull

The git pull command downloads the content (not the metadata) and immediately updates the local repository with the latest content.

```
git pull origin
```
or
```
git pull <remote_url>
```

### 13. git push
After connecting to the remote repository (using the git remote command), it's time to push the changes to the repository
```
git push origin
```
or
```
git push -u <short_name> <your_branch_name>
```

The Git source and upstream must be set up before using the git push command.
```
git push –set-upstream <short_name> <branch_name>
```

### 14. git fetch

This command downloads all information about commits, references, etc. so you can review them before applying these changes to your local repository.

```
git fetch
```
### 15. git stash

This command saves edited files temporarily. stash means to save. In Git, everything that is not committed is saved.

```
git stash
```

The following command lists all stashes:

```
git stash list
```
It simply applies a stash to the branch:

```
git stash apply
 ```

 ### 16. git log

 With the help of the git log command, you can see all the previous commits starting from the last commit.

 ```
git log
 ```
 By default it shows all commits of the current branch but you can use it to see all commits of entire branches with all options.


 ```
git log –all
 ```

### 17. git shortlog

The git shortlog command shows a summary of the git log command.

```
git shortlog
```

### 18. git show

Compared to the git log command, the git show command shows details about a specific commit.
```
git show <your_commit_hash>
```

### 19. git rm

Sometimes you need to remove multiple files, here the Git rm command is used.
This command can remove tracked files from index and working directory.

```
git rm <your_file_name>
```


### 20. git merge

The git merge command helps to merge changes from two branches into a single branch.

```
git merge <branch_name>
```
### 21. git rebase

Git Rebase is similar to the git merge command. Merges two branches into a single Branch with one exception. A git rebase command overwrites the commit history.

If you have multiple private branches, you should use the git rebase command to merge them into one Branch. This creates a linear commit history.
```
git rebase <base>
```

### 22. git bisect

The git bisect command helps to find bad commits.


A. Start git bisect :

```
git bisect start
```


B. Notify git bisect about a good commit.

```
git bisect good a123
```

C. Notify git bisect about a bad commit.

```
git bisect bad z123
```

### 23. git cherry-pick

Git cherry-pick is a good and powerful command that allows you to pick any commit from any branch and apply it to any other Branch.

``` git cherry-pick <commit-hash>
```

### 24. git archive

The git archive command combines multiple files into a single file. It's like a zip tool, meaning you can unzip files and access each file individually.

```
git archive –format zip HEAD > archive-HEAD.zip
```


### 25. git pull –rebase

Most of the time, your should rebase (not merge) when using git pull.

```
git pull –rebase
```

### 26. git blame

Use the git blame command to check the contents of each file line by line. This command helps to identify who made changes to a file.

```
git blame <your_file_name>
```

### 27. git tag

Git tags are helpful & you can use them for release management. You can think of the Tag as an immutable branch. Its importance is much greater during public release. The Git Tag command is used to create a new tag.

```
git tag -a v1.0.0
```


### 28. git verify-commit

The git verify-commit command checks the GPG signature of commits. GPG or "GNU Privacy Guard"

```
git verify-commit <commit>
```


### 29. git verify-tag

You can verify the tag with this command.

```
git verify-tag <tag>
```


### 30. git diff

Most of the time, you should compare two git files or branches before committing or pushing. The helpful command git diff is used for this.

A. Comparing the working directory with the local repository:

```
git diff HEAD <filename>
```


B. Comparison of two branches:

```
git diff <source branch> <target branch>
```

### 31. git citool

Git Citool is a graphical alternative to Git Commit.

```
git citool
```

### 32. git mv

The Git mv command is used to rename a Git file. It has two arguments; Source and destination file names.

```
git mv <old-file-name> <new-file-name>
```


### 33. git clean

You can work with untracked files using the git clean command. With this command, you can remove all untracked files from the working directory. To work with tracked files, you must use the git reset command.

```
git clean
```

### 34. git help

You can use the git help command to get more information and help for each command.

```
git help <git_command>
```

### 35. git whatchanged

The Git whatchanged command does the same thing as Git log but in raw format.

```
git whatchanged
```
