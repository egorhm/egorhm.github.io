---
layout: post
title: GIT Cheatsheet
tags: [git, cheatsheet]
---

Just a list of some git commands that can be useful in daily work. Very often it can be rather hard
to remember all this commands and where this cheatsheet can be helpful. It covers only those
commands and combinations that i consider usefull for me and defenitly there more amd more commands
that someone else may consider irreplaceable.

<!--more-->

### Staging and Remote

View staged differences

    git diff --staged

Unstage changes
    
    git reset HEAD <file>

Blow away all changes since last commit

    git checkout -- <file>

__Don't do the following commands after `push`!__

Forgot something on commit. Reset last commit into staging. Move to commit before HEAD (HEAD^).

    git reset --soft HEAD^

Undo last commit and all the changes. Roolback several commit (e.g. 2 : `HEAD^^`).

    git reset --hard HEAD^

### Branching

List all remote branches

    git branch -r

Get all the information on all the branches local/remote and etc.

    git remote show origin

Delete the remote branch. __Only__ remote and you'll need to delete local branch manually.

    git push origin :branch_name

Delete local branch.

    git branch -[d|D] branch_name



