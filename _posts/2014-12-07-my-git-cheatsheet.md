---
layout: post
title: GIT Cheatsheet
tags: [git, cheatsheet]
---

Just a list of some git commands that can be useful in daily work. A cheatsheet is only for my
private purposes and covers the commands that I'm using...

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





