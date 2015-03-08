# Octopress 3.0

Blogging using [Octopress](https://github.com/octopress/octopress). It's an obsessively designed toolkit for writing and deploying [Jekyll](http://jekyllrb.com/) blogs.

## Steps to try yourself

```cmd
git clone https://github.com/samarpanda/hello_octopress_3.git

## install dependencies
bundle

## jekyll build and serve with watch enabled. Terminal output will get your the url to preview pages
jekyll serve -w --baseurl ""

```

## Steps to Deploy this blog

* I have configured the deployment using git `gh-pages` branch.  
* Set `baseurl` in `_config.yml` as per your github repo  
* Update `_deploy.yml` as per your settings  
* For more details refer [Octopress deploy](https://github.com/octopress/deploy)  
* Run below command to publish this site in github using `gh-pages` branch  
```cmd
octopress deploy
```


## Preview

Don't miss to checkout the [Demo](http://samarpanda.github.io/hello_octopress_3/)

P.S: This piece of work was influenced by [Harvey Thompson](http://www.610yesnolovely.org/2014/12/31/setting-up-a-free-blog.html)