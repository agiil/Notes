---
layout: IT
title: Muu
permalink: Muu
published: true
sidebar: true
---

# Muu

/// Ikoonide moodustamine EA-le
https://materialdesignicons.com/
valida ikoon
pildistada (48 või 32 suurus)
värvi muutmiseks 6068

// Värvide valimine
https://www.materialui.co/colors (Chromes)

- -
Agiilsõnastik
    Käivita Git Bash
    muuda Sublime-iga faili index.html
    cd Desktop
    cd AGIILSONASTIK
    git add -A
    git commit -m “uued sõnad”
    git push
- -

## Freshbrew
- Repod ja kaustad:
  - GitHub: agiil/Freshbrew - publitseeritud blogi
  - Desktop/Freshbrew - GitHubi repo lokaalne koopia
  - Desktop/FreshbrewPREPARE - ettevalmistuskaust, kasutab Hugot
  - public - siia genereerib Hugo väljundfailid, need tuleb tõsta Desktop/Freshbrew-sse
- Töövoog:
  - Blogikande lisamine: lisada fail kausta content/post, faili päis kopeerida varasemast blogikandest
  - GitBash -> cd Desktop -> cd FreshbrewPREPARE
- Kofiguratsiooni kontrollimine: hugo config
  - Kontrollimine enne genereerimist: hugo check
  - Blogifailide genereerimine: hugo
    - genereeritakse kausta public
  - Vanade failide kustutamine Desktop/Freshbrew-st: teha git-ga:
    - git rm -r .
  - Failide kopeerimine Desktop/FreshbrewPREPARE/public-st kausta Desktop/Freshbrew: käsitsi
  - Stage-imine: git add -A
  - Commit-ne: git commit -m “Uus blogikanne”
  - Üleslaadimine: git push
 
