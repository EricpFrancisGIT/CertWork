## Git Hidden Folder

there is a hidden folder called `.git` which tells you that your project is a git repo

if we wanted to create a git repo in a new project, we create the fodler and then initialize that repo using `git init`

```
mkdir/workspace/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add Readme.md
#makes changes to readme.md
git commit -m "add readme file"
```

## Cloning

We can clone 3 ways: HTTPS, SSH, Github CLI

Since we are using Github Codespaces, we will create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## HTTPS 

```sh
git clone https://github.com/Eric-Github-Cloud-Journey/2ndAttempt.git
cd 2ndAttempt
```
## Commits

When we want to commit code we can write git commit  which will open up the commit edit message in the editor of choice 

```sh
git commit
```
Set the global editor
```sh
git config -- global core.editor emacs
```

Make a commit and commit message without opening an editor

```sh
git commit -m "add another 2 exclamation marks"
```
## Branches

## Remotes

## Stashing

## Merging

## Add 

When we want to stage changes that will be included in the commit, we can use the . to add all possible files.

```sh
git add Readme.md
git add .
```
## Reset

Reset allows you to move Staged changes to be unstaged.
This is useful when you want to revert all files not to be committted

```sh
git add.
git reset
```

> git reset will revert a git add.

## Status

Git status shows you what files will or will not be commited.

```sh
git status
```
## Gitconfig file
the gitconfig file is what stores your global configurations for git such as email, name, editor and more.

Showing the contents of the gitconfig file

```sh
git config --list
```

when you first install Git on a machined you are supposed to set up your name and email

```sh
git config --global user.name "John.Doe"
git config --global user.email johndoe@example.com
git status
```
