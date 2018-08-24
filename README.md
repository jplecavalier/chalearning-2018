# chalearning-2018
Recipe for the summer 2018 edition of Machine Learning chalet

## Ingredients

- your favorite R distribution
- your favorite IDE
- 1 pinch of an internet connection

## Steps
1. Try [this markdown demo](http://markdown-it.github.io) to familiarize yourself with markdown 
2. Save [this file](http://math.mcgill.ca/yyang/regression/RMarkdown/example.Rmd) as "file/path/test.Rmd"
3. Render that file as an html document with the following R command
``` rmarkdown::render("file/path/test.Rmd", output_format = "html_document") ```
4. At the R command line, run the following chunk to install the blogdown package  
``` install.packages("blogdown") ```
5. At the R command line, run the following chunk to install the most up-to-date Hugo library  
``` blogdown::install_hugo() ```
6. Create a new local repository where you want your website to be contained (for example, under path "your/repo/path")
7. In your R session, set your working directory to your new repo, either explicitly (``` setwd("your/repo/path")``` at the R command line) or by creating a RStudio project in the folder
8. At the R command line, run the following chunk to create your website from [this template](http://www.github.com/yihui/hugo-lithium)  
``` blogdown::new_site(theme = "yihui/hugo-lithium") ```
9. At the R command line, run the following chunk to visualize your website from your local browser  
``` blogdown::serve_site() ```
10. Save the [following file](https://www.raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/images/dastat-logo.JPG) as static/images/dastat-logo.PNG
11. Save the [following file](https://www.raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/config/config.toml) as config.toml
12. At the R command line, run the following chunk to create your first article  
```blogdown::new_post(title = "My first post")```
13. Go check the new post in content/post. Notice the post is a .md file  
14. At the R command line, run the following chunk to create your second article. This time, it will be a rmarkdown article   
```blogdown::new_post(title = "My second post", ext = ".Rmd")```
15. Now save [this file](http://math.mcgill.ca/yyang/regression/RMarkdown/example.Rmd) as "content/post/2018-08-25-my-third-post.Rmd"
16. Save [this other file](http://math.mcgill.ca/yyang/regression/RMarkdown/example.Rmd) as "content/post/2018-08-25-my-fourth-post.Rmd"
17. In "content/post/2018-08-25-my-fourth-post.Rmd", replace the yaml header by this header  
``` 

---
title: My fourth post
author: My Name
date: "`r format(Sys.time(), '%d %B, %Y')`"
slug: my-second-post
categories: ["AI" "Machine Learning"]
tags: [ "hype" "buzzword" "witchcraft" "black magic"]
---

```
18. Look at these websites that were made with blogdown :  
- https://roh.engineering/post/
- https://maraaverick.rbind.io/
- https://crimebythenumbers.com/
- https://alison.rbind.io/
- https://yihui.name/
