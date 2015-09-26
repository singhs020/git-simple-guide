GIT ---Simple Guide
===================


This reference guide summarizes commonly used Git command line instructions for quick reference

----------

 
#### **Download GIT !**

> http://git-scm.com

-----------
####  **Basic Configuration**
```
 git config --global user.name "[name]"
```
>- **sets author for commit messages**

```
git config --global user.email "[email address]"
```
>- **sets email for commit messages**

```
git config --global color.ui auto
```
>- **enables helpful colorization in command prompt**

----------
#### **Creating Repositories**
```
git init
```
>- **creates a new local repository**

------

#### **Cloning a Repository**

```
git clone [url]
```
>- **Downloads the project with its history**

-----

#### **Making Changes**
```
git status
```
>- **status of your working directory**

```
git add [file]
```
>- **adds the file to staging area**

```
git add .
```
>- **add all files to staging area**

```
git commit -m "[message]"
```
>- **records snapshot in version history**

```
git reset [file]
```
>- **unstage the file but preserves its changes**

-----
#### **Branching**

```
git branch
```
>- **list all local branches in current repository**

```
git branch -r
```
>- **list all remote branches in current repository**

```
git branch [branch name]
```
>- **creates a new local branch**

```
git checkout -b [branch name]
```
>- **creates and checkout new local branch**

```
git branch -d [branch name]
```
>- **deletes a local branch**

-----

#### **Working With Remote**

```
git remote update origin
```
>- **updates history of remote branches**

```
git pull
```
>- **fetch all the changes from remote and merge them in local branch**

```
git push -u origin [branch name]
```
>- **creates a new branch in remote and sets the tracking with local branch**

```
git push origin --delete [branch name]
```
>- **deletes a remote branch**

```
git push origin [branch name]
```
>- **pushes local changes to remote branch**

-----
#### **Merging & Rebasing **

```
git merge [branch name]
```
>- **merge changes from the specified branch into current branch**

```
git mergetool
```
>- **initialize merge tool in case of conflicts**

```
git rebase [branch name]
```
>- **rebase current branch on the specified branch**

-----
#### **GUI Commands**

```
git gui
```
>- **opens the basic gui for git**

```
gitk
```
>- **shows history tree for current branch**

```
gitk --all
```
>- **shows history tree for whole repository**
