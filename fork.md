Forking Repository
==================

A fork is a copy of a repository.
Forking a repository allows you to freely experiment with changes without affecting the original project.
A great example of using forks to propose changes is for bug fixes.
Make a fix and submit a pull request the project owner.

On GitHub

- Open a project.
- In the top-right corner of the page, click Fork.

# Clone your fork

To be able to work on the project, you will need to clone it to your computer.

```shell
git clone [url]
```

# Synchrnization

Synchronize your fork with the original repository.

- List your remote repository

```shell
git remote -v
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
```

- Add a remote upstream

```shell
git remote add upstream [original project url]
```

Now, you can keep your fork synced with the upstream repository

```shell
git fetch upstream
git merge upstream/master
```

