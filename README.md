# chalearning-2018
Recipe for the summer 2018 edition of Machine Learning chalet

## Ingredients

- your favorite R distribution
- your favorite IDE
- 1 pinch of an internet connection

## Steps

1. At the R command line, run the following chunk to install the blogdown package  
``` install.packages("blogdown") ```
2. At the R command line, run the following chunk to install the Hugo library  
``` blogdown::install_hugo() ```
3. Create a new git repository (more details on git later) where you want your website to be contained. For example :  
![git-init-new-directory](http://www.raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/images/git-init-new-directory.JPG)  
![git-init-name](http://www.raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/images/git-init-name.JPG)  
4. At the R command line, run the following chunk to create your website from [this template](http://www.github.com/yihui/hugo-lithium)  
``` blogdown::new_site(theme = "yihui/hugo-lithium") ```
5. At the R command line, run the following chunk to visualize your website from your local browser  
``` blogdown::serve_site() ```
6. Save the [following file](https://www.raw.githubusercontent.com/jplecavalier/chalearning-2018/master/static/images/dastat-logo.JPG) as mywebsite/static/images/dastat-logo.PNG
7. Save the [following file](https://www.raw.githubusercontent.com/jplecavalier/chalearning-2018/master/recipe/config/config.toml) as mywebsite/config.toml
8. At the R command line, run the following chunk to create your first article  
```blogdown::new_post(title = "My first post")```
9. At the R command line, run the following chunk to create your second article. This time, it will be a rmarkdown article, rather than a markdown article only  
```blogdown::new_post(title = "My second post", ext = ".Rmd")```
10. LC drag n drop un article
11. JPL drag n drop un article
12. On toggle quelques items du .yaml de l'article
13. Exemple 1 de site fait avec blogdown
14. Exemple 2 de site fait avec blogdown