---
title: "Git"
date: 2023-05-10T08:16:07+02:00
draft: false
author: Thomas Panzeri
---

## Basic Commands

* `git init` - initializes a new Git repository
* `git clone [url]` - clones a remote repository to your local machine
* `git status` - displays the current status of the repository
* `git add [file]` - adds a file to the staging area
* `git add .` - adds all modified files to the staging area
* `git commit -m "[message]"` - commits changes to the local repository with a descriptive message
* `git push` - pushes changes from the local repository to the remote repository
* `git pull` - pulls changes from the remote repository to the local repository

## Branching

* `git branch` - lists all branches in the repository
* `git branch [branch name]` - creates a new branch
* `git checkout [branch name]` - switches to the specified branch
* `git merge [branch name]` - merges the specified branch into the current branch

## Reverting Changes

* `git reset [file]` - unstages a file
* `git reset --hard` - discards all changes since the last commit
* `git revert [commit]` - creates a new commit that reverses the changes made in the specified commit

## Viewing Changes

* `git log` - displays the commit history
* `git diff [file]` - shows the differences between the file in the working directory and the most recent commit
