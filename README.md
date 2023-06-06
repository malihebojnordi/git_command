# git_command
I am talking about git's command

## git config
You are using git for the first time or have a new git installation. This command sets your identity with your name and email address.
```
git config –global user.name “Your name”

```
```
git config –global user.email “Your email”

```

## git version
Used to check the Git version
```
git version

```

## How to init on git or gitlab
is the first command you use to start a new project in Git. This command will create a new empty repository into which you can then store your source code.
```
git init

```
You can also include the name of the repository in the git init command
```
git init <your repository name>

```
## git clone

The git clone command is used to copy an existing repository.
You use git clone when you need a copy of an existing repository. The git clone command first uses the git init command, then it will check all its contents.
```
git clone <your project URL>

```
## git add

The git add command adds all new code files or edited files to the repository. This command provides various options for adding files and folders.

The following command adds a specific file to the stage area.
```
git add your_file_name

```
The following command adds all edited and new files to the stage area.
```
 git add *

 ```

## Adding file when you want to push on github

```
git add . 

```

## committing on git

This is an essential command in Git. In fact, the git commit command will add the changes to the local repository.
```
git commit -m "writing text"

```
## git status

git status is used to check the status of files and you can identify which files need attention. This command can be executed at any time.
You can use it between the Git add and Git commits commands to see the status.
```
git status

```
## git branch

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
## git checkout

This command is used to switch between branches. It is one of the most powerful git commands and can be used as a multipurpose tool.

1. Go to another branch:
```
git checkout <branch_name>
```
2. You can create a new branch and switch to it:
```
git checkout -b <your_new_branch_name>
```

## git remote

This command acts like a border around the tank. If you need to communicate with the world outside the repository, you should use the git remote command. This command connects the local repository to the remote one.

```
 git remote add <shortname> <url>
```

### How to pull or get code from git

The git pull command downloads the content (not the metadata) and immediately updates the local repository with the latest content.

```
git pull origin
```
or
```
git pull <remote_url>
```

### How to push on git
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

###  git fetch

This command downloads all information about commits, references, etc. so you can review them before applying these changes to your local repository.

```
git fetch
```
### git stash

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

 ### git log

 With the help of the git log command, you can see all the previous commits starting from the last commit.

 ```
 git log
 ```
 