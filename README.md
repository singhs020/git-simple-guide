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

-----------
#### **Generating ssh key using ssh-keygen**

````
ssh-keygen -t rsa
````

>- **execute command above, It will prompt for file location ~/.ssh/id_rsa. Press Enter & fill passphrase**

````
cat ~/.ssh/id_rsa.pub
````

>- **display public key to consume futher**

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
#### **Merging & Rebasing**

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

-----
#### **Tags**

```
git tag
```
>- **list all the available tags**

```
git tag -l "v1.0.*"
```
>- **search for the tags(allow us to use wildcard characters)**

```
git tag -a v1.x -m "tagging message"
```
>- **creates an annoated tag**

```
git tag v1.x
```
>- **creates a lightweight tag**

```
git show v1.x
```
>- **shows a tag**

```
git tag v1.x <commit>
git tag -a v1.x <commit>
```
>- **allows us to add tag later**

-----------
#### Useful Tips & Tricks

>- **Delete all merged local branches**
```
git branch --merged | egrep -v "(^\*|master|dev)" | xargs git branch -d
```
-----------
#### **Docs & CheatSheet**
>- https://git-scm.com/doc
>- https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf
>- https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow
>- https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows
>- http://nvie.com/posts/a-successful-git-branching-model/
>- https://guides.github.com/introduction/flow/index.html
