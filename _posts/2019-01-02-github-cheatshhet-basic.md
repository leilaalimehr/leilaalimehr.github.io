---
title: Cheatsheet for Github   
description: Cheatsheet for Github
date: 2019-01-02
author: Leila Alimehr
published: false
tags: Github  Cheatsheet
categories: [blog]
comments: true
---

#  Git and Github  (Basics)
Git is a source control repository that allows team users to collaborate to manage their codes on a project.

## Contents
- [Creating new repository](#Creating-new-repository)
- [Clone a repository](#clone-a-repository)
- [Tracking changes](#tracking-changes)
- [Remote Github](#remote-github)
  - [Set repository Github](#Set-repository-Github)
  - [Check remote repository](#check-remote-repository)
  - [Push local Git](#push-local-git)
  - [Update local Git](#update-local-Git)
  - [Example](#example)
  
## Creating new repository
To get started:
- Create a folder
- Go inside folder
- Run `git init`  to initialize your project.  
```
mkdir folder0
cd folder0
git init
```

##  Clone a repository
Unlike Git that run locally on a computer, Github is a cloud Git-based repository platform built for code developers to maintain the code source.  

- Go inside folder where you want to  save the  repository
- Run  `git clone https://github.com/[name of folder]/[name of repository]`


```
git clone https://github.com/leilaalimehr/SQL
```

## Tracking changes
###Check the status of project
- Run  `git status`

### Track a file
- Run  `git add [names of file]` or  `git add .` to add everything.
### Make a commit
- Run  `git commit -m "Write your commit"`

```
git status
nano file0.txt
myfirst file
^X

git add file0.txt
git commit -m "Write your commit"
git status
```

### Track all file and subfolder
- Run  `git add -A`
### Track folder
- Run  `git add foldername/`
### Remove file
- Run  `git rm Filesname`

### Compare the current stat with saved ones
- Run  `git diff`

### Branching
Be default the git adds all files and folders under master branch, user can add isolated branches that allows you move back and forth between them.  

- Create new brach `git checkout -b [name of brach]`
- Back to the master `git checkout master`
- Delete the branch `git checkout -d [name of branch]`
- Push to repository `git push origin [name of branch] `

## Remote Github
- Go to Github and create new repository

### Set repository Github
Set that repository’s url as the origin repo:
- Run  `git remote add origin https://github.com/[name of folder]/[name of repository].git`

### Check remote repository 
Check remote repository Github
- Run  `git remote -v`

### Push local Git 
Push local Git to a Github repository
- Run  `git push origin master`

### Update local Git
Update the local Git to a Github repository
- Run  `git pull origin master` to get the most recent changes that you or others have merged on GitHub.

```
git remote add origin https://github.com/leilaalimehr/justfortest
git remote -v

cd justfortest
git init

nano file0.txt
myfirst file
^X

git push origin master
git add file0.txt
git commit -m "Write your commit"
git status
git pull origin master
```

More useful link:<br>
-[[Swcarpentry GitHub]](http://swcarpentry.github.io/git-novice/): http://swcarpentry.github.io/git-novice/

**[⬆ back to top](#contents)**

### License
Copyright (c) 2019 Leila Alimehr
