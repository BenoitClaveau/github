Mastering Git Workflow
=========================

Git is an open source program for tracking changes in text files. It was written by the author of the Linux operating system, and is the core technology that GitHub, the social and user interface, is built on top of.

##### Table of Contents
[Initializing the Repository](#repository)  
[Adding a file](#add)  
[Committing Changes](#commit)  
[Pushing to a Remote Repository](#push)  
[Pulling from the Remote Repository](#pull)  

##### Documentations
[Cheat Sheet](documents/github-git-cheat-sheet.pdf)  
[Git Reference](http://gitref.org/)  

<a name="repository"/>
## Initializing the Repository

A repository is the most basic element of GitHub. They're easiest to imagine as a project's folder. A repository contains all of the project files (including documentation), and stores each file's revision history. Repositories can have multiple collaborators and can be either public or private.

From the terminal, navigate to the root directory of your project and enter git init to generate a new Git repository.

```shell
mkdir [project-name]
cd [project-name]
git init
echo "me" >> contributors.txt
git a .
git commit -m "first commit"
git push origin master
```
From [GitHub Web Interface](https://help.github.com/articles/create-a-repo/)

- In the upper-right corner of any page, click +, and then click New repository
- Create a short name
- Choose between creating a public or private repository.

```
git clone [url]
```

<a name="add"/>
## Adding a File

We need to add some files to be version controlled. This can be accomplished by adding specific files by name using the git add command:

```shell
git add .
```

<a name="commit"/>
## Committing Changes

Once a change has been made, it is best practice to commit that change to the repository.  All commitments in Git require a commit message

```shell
git commit -am "this is my local commit I want to push to remote repository"
```

Warning: if you created new file, you need to add it to your local repository before committing.

<a name="push"/>
## Pushing to a Remote Repository

Pushing refers to sending your committed changes to a remote repository. For instance, if you change something locally, you'd want to then push those changes so that others may access them.

```shell
git push
```

<a name="pull"/>
## Pulling from the Remote Repository

Pull refers to when you are fetching in changes and merging them. For instance, if someone has edited the remote file you're both working on, you'll want to pull in those changes to your local copy so that it's up to date.

```shell
git pull
```

Once the local repository is updated, any conflicting files will be observed and conflicts must be resolved, after which point editing can begin as normal until the local repository needs to be pushed back to the remote repository once again, and the process repeats until development is complete!
