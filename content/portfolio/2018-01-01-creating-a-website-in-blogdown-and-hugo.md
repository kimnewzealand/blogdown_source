---
title: Creating a website in Hugo creative portfolio theme
slug: creating-a-website-in-blogdown-and-hugo
categories: ["Post"]
tags: ["R","blogdown"]
---

*30 January 2018*  
  
There are a many tutorials and the great bookdown [blogdown: Creating Websites with R Markdown](https://bookdown.org/yihui/blogdown/) with detailed steps on how to create a website using blogdown and Hugo. 

I used the fantastic [tutorial](https://tclavelle.github.io/blog/blogdown_github/) by Tyler Clavelle to create this blog. This website uses the [blogdown](https://github.com/rstudio/blogdown) R package and static site generator Hugo. I chose to use the Hugo creative portfolio theme, with side bar and tiles layout. I use Windows and GitHub repo to deploy the website.

This is a brief summary of my tips, discovered through trial error and many github pushes:

+ In order to change the style colours you need to specify the full style = "style.sea.css", not just style= "sea" in the config.toml file

+ Once you have installed your theme, do not change any of the theme folder files. You can override these with updates or new files in your blog_down source directory. This is because of Hugo's [lookup order](https://gohugo.io/templates/lookup-order/). 

+ I was looking for a way to separate the projects and posts into content sections. In an attempt to do this, I created params.navlinks for post in the config file but this theme does not seem to work with list.html in any layout folder. There was an issue raised in [github](https://github.com/kishaningithub/hugo-creative-portfolio-theme/issues/35) however the creator answered that the theme is designed to publish only to the portfolio. 

+ After a bit of research on text editors, I am using Atom text editor to edit multiple R markdown and html files in the blogdown_source folder.

+ I have also transitioned from command line Git Bash to using a git client GitKraken and yes I am now [happy with git](http://happygitwithr.com/). I am using GitKraken to stage, commit and push files to the kimnewzealand.github.io repo.
