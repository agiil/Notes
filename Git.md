---
layout: IT
title: Git
permalink: Git
published: true
sidebar: true
---

<p><a href='https://github.com/agiil/Notes/edit/master/Git.md'><span class='material-icons'>edit</span></a></p>

# Git
{:.no_toc}

* TOC
{:toc}

<a href='https://github.com/agiil/Notes'>Edit</a>

## GitHubi lokaalne repo

__lokaalse repo loomine__ 1) mine kataloogi, kuhu alla lokaalne repo luua 2)  `git clone <GitHubi repo URL>`

__mis faile on muudetud?__ `git status`

__commit-i ettevalmistamine__ 1) failide lisamine (_staging_): `git add <failinimi>`; 2) lisa kõik muudetud failid: `git add --all`; 3)  stage manually deleted files (better to use `git rm)`: `git add -u`

__commit-i tegemine__ `git commit -m <kirjeldus>`

__lokaalse repo värskendamine__ `git pull`

__lokaalsete muudatuste üleslaadimine__ (eeldab push-õigust): `git push [origin]`

__lokaalsete muudatuste hülgamine__ `git reset --hard`

__haru loomine__ `git branch <haru>`

__harude kuvamine__ kõik: (jooksev haru tärniga): `git branch`; kuvab nii lokaalsed kui ka eemal (remote) jälgitavad (tracking) harud: `git branch -a`

__haru kustutamine__ `git branch -d <haru>`

__haru vahetamine__ `git checkout <haru>`

__kustuta kaust__ (`-r` rekursiivne) `git rm -r <kaust>`

## Git Bash

__kataloogi loomine__ `mkdir <kataloog>`

__faili ümberpaigutamine__ `mv <file> <kataloog>`

__faili ümbernimetamine__ `mv <old> <new>`

__skripti täitmine__ `./Puhasta.sh`

__paste Git Bashis__ `<Fn><Insert>` (Lenovo)

## Loendamine

__failide loendamine jooksvas kaustas failitüübi järgi__ `ls -lR *.md | wc -l`

__failide rekursiivne loendamine jooksvas kataloogis__ `find . -type f | wc -l`

__kaustade arv (rekursiivne)__ `find DHX-Adapter -type d | wc -l`

__LOC count__ `shopt -s globstar`, seejärel `wc -l **/*.java`

__muudatuste statistika__ `git diff --stat <commit>`

## Parooliküsimise vältimine

`git config --global credential.helper wincred`

## Kirjandus

- [Git Reference](http://gitref.org/index.html) by GitHub team
- [Git interaktiivne spikker](http://ndpsoftware.com/git-cheatsheet.html#loc=workspace)
- [Gitflow parem diagramm](http://www.patrickzahnd.ch/)
- [2FA GitHubis](http://blog.swilliams.me/words/2015/04/01/two-factor-authentication-for-github/) 
- [Kuidas mestimine töötab?](https://www.quora.com/How-does-Git-merge-work)
- [aha-moments-when-learning-git](https://betterexplained.com/articles/aha-moments-when-learning-git/) 




