# chalearning-2018
Recipe for the summer 2018 edition of Machine Learning chalet

## Ingredients

- your favorite R distribution
- your favorite IDE
- 1 pinch of an internet connection

## Steps
1. Install the required packages at the R command line  
```
install.packages("blogdown")
install.packages("rmarkdown")
```
2. Try [this markdown demo](http://markdown-it.github.io) to familiarize yourself with markdown 
3. Save [this file](http://www.math.mcgill.ca/yyang/regression/RMarkdown/example.Rmd) as "file/path/test.Rmd"
4. Render that file as an html document with the following R command  
``` rmarkdown::render(input = "file/path/test.Rmd", output_format = "html_document") ```
5. Open the newly created "file/path/test.html" HTML file with your browser, and compare it to the corresponding test.Rmd source code  
6. At the R command line, run the following chunk to install the most up-to-date Hugo library  
``` blogdown::install_hugo() ```
7. Create a new local repository where you want your website to be contained (for example, under path "your/repo/path")
8. In your R session, set your working directory to your new repo, either explicitly (``` setwd("your/repo/path")``` at the R command line) or by creating a RStudio project in the folder
9. At the R command line, run the following chunk to create your website from [this template](http://www.github.com/yihui/hugo-lithium)  
``` blogdown::new_site(dir = ".", theme = "yihui/hugo-lithium") ```
10. At the R command line, run the following chunk to visualize your website from your local browser  
``` blogdown::serve_site() ```
11. Save the [following file](http://raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/images/dastat-logo.JPG) as static/images/dastat-logo.JPG
12. Save the [following file](http://raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/config/config.toml) as config.toml
13. Preview your website again and notice the logo and header changes  
``` blogdown::serve_site() ```
13. At the R command line, run the following chunk to create your first article  
```blogdown::new_post(title = "My first post")```
14. Go check the new post in content/post. Notice the post is a .md file  
15. At the R command line, run the following chunk to create your second article. This time, it will be a rmarkdown article   
```blogdown::new_post(title = "My second post", ext = ".Rmd")```
16. Now save [this file](http://www.math.mcgill.ca/yyang/regression/RMarkdown/example.Rmd) as "content/post/2018-08-25-my-third-post.Rmd"
17. Save [this other file](http://www.math.mcgill.ca/yyang/regression/RMarkdown/example.Rmd) as "content/post/2018-08-25-my-fourth-post.Rmd"
18. In "content/post/2018-08-25-my-fourth-post.Rmd", replace the yaml header by this header  
``` 

---
title: My fourth post
author: My Name
date: "`r format(Sys.time(), '%Y-%m-%d')`"
slug: my-fourth-post
categories: ["AI", "Machine Learning"]
tags: ["hype", "buzzword", "witchcraft", "black magic"]
---

```
19. Look at these websites that were made with blogdown :  
- https://roh.engineering/post/
- https://maraaverick.rbind.io/
- https://crimebythenumbers.com/
- https://alison.rbind.io/
- https://yihui.name/
