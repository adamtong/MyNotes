# Git

## Key features
* Allows us to keep track of changes made to our code.
* Allows us to synchronize code among various people working on the same project.
* Allows us to work on code on a branch without affecting the main code base.
* Allows us to revert back to previous versions of our code if required.

## Basic commands

To clone a repository:
```bash
git clone <url>
```
To add a new file:
```bash
git add <filename>
```
Note that git does not track directories, so `git add <directory>` has no effect.

To add all files in a directory:
```bash
git add .
```
To commit changes:
```bash
git commit -m 'commit message'
```
To check local repository status:
```bash
git status
```
To check repository history:
```bash
git log
```
To push local commits to github:
```bash
git push origin main
```
where `origin` is the remote repository, and `main` is the name of a branch in the local repository to be pushed.

To pull updates from the remote repository to the local repository
```bash
git pull
```
To revert to a previous commit
```bash
git reset --hard <commit>
```
To undo the last commit
```bash
git reset HEAD~
```
To revert to the latest version on github
```bash
git reset --hard origin/main
```

## Branching

To create 