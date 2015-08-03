---
title: "Initial notes on website/notebook structure"
author: ”Noam Ross”
date: 2015-08-03
notebook: 
...

 -  Each project has a `notebook/` folder somehwhere in its repository
 -  The notebooks folders are compiled to `*.md` from `*.Rmd` or `*.ipynb` on each push of the *project* using Circle-CI.
     +  Commits md files to a "notebook" branch
 -  The notebook repo compiles regularly or on an update (hook?)
     +  Downloads the latest version of the notebook branch of each project into a `_posts` category folder
     +  Compiles via jekyll