# GitHub User Guides

In this guide you'll discover how use GitHub 

* Mastering Git Workflow
* Forkings projects
* Create your first GitHub page
* Managing Issues
* Writing Markdown files
* Being Social

# Mastering Git Workflow

Git is an open source program for tracking changes in text files. It was written by the author of the Linux operating system, and is the core technology that GitHub, the social and user interface, is built on top of.

## Create a repository

### What is repository

A repository is the most basic element of GitHub. They're easiest to imagine as a project's folder. A repository contains all of the project files (including documentation), and stores each file's revision history. Repositories can have multiple collaborators and can be either public or private.

```shell
mkdir [project-name]
cd [project-name]
git init
echo "me" >> contributors.txt
git a .
git commit -m "first commit"
git push origin master
```

[GitHub Web Interface](https://help.github.com/articles/create-a-repo/)

## Pull

Pull refers to when you are fetching in changes and merging them. For instance, if someone has edited the remote file you're both working on, you'll want to pull in those changes to your local copy so that it's up to date.

```shell
git pull
```

## Push

Pushing refers to sending your committed changes to a remote repository. For instance, if you change something locally, you'd want to then push those changes so that others may access them.

```shell
git commit -am "this is my local commit I want to push to remote repository"
git push
```

Warning: if you created new file, you need to add it to your local repository before the commit.

### New file

```shell
git add .
git commit -am "new file"
git push
```

# Writing Markdown files

[guide](https://guides.github.com/features/mastering-markdown/)

