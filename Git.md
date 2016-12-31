---
layout: IT
title: Git
permalink: Git
published: true
sidebar: true
---

# Git

- GitHub lokaalse repo loomine
  - mine kataloogi, kuhu alla lokaalne repo luua
  `git clone <GitHubi repo URL>`
- mis faile on muudetud?
  - `git status`
- commit-i ettevalmistamine 
  - failide lisamine (staging): `git add <failinimi>`
  - lisa kõik muudetud failid: `git add --all`
  - stage manually deleted files (better to use `git rm)`: `git add -u`
- commit-i tegemine
  - `git commit -m <kirjeldus>`
- lokaalse repo värskendamine: `git pull`
  - lokaalsete muudatuste üleslaadimine (eeldab push-õigust): `git push [origin]`
- harude kuvamine
  - kõik: (jooksev haru tärniga): `git branch`
    - kuvab nii lokaalsed kui ka eemal (remote) jälgitavad (tracking) harud: `git branch -a`
- haru kustutamine
  - `git branch -d <haru>`
- haru vahetamine
  - `git checkout <haru>`
- kustuta kaust (`-r` rekursiivne)
  - `git rm -r <kaust>`

## Git Bash

- kataloogi loomine: `mkdir <kataloog>`
- faili ümberpaigutamine: `mv <file> <kataloog>`
- faili ümbernimetamine: `mv <old> <new>`

- paste Git Bashis: `<Fn><Insert>` (Lenovo)

## Failide rekursiivne loendamine jooksvas kataloogis

- `find . -type f | wc -l`

### Parooliküsimise vältimine

- `git config --global credential.helper wincred`

### Kirjandus

- Git interaktiivne spikker: http://ndpsoftware.com/git-cheatsheet.html#loc=workspace; 
- Gitflow parem diagramm: http://www.patrickzahnd.ch/ 
- 2FA GitHubis: http://blog.swilliams.me/words/2015/04/01/two-factor-authentication-for-github/ 
- https://www.quora.com/How-does-Git-merge-work 
- https://betterexplained.com/articles/aha-moments-when-learning-git/ 




