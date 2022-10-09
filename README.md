[![Build Status](https://travis-ci.com/rstudio/bookdown-demo.svg?branch=master)](https://travis-ci.com/rstudio/bookdown-demo)


#  best practice for bioinformatics

Some useful R tips.




# Location

- local: Yi station: /home/wangjl/data/rmarkdown_demo/bookdown-demo-main/
- github: https://github.com/DawnEve/R_best_practice
- url: https://dawneve.github.io/R_best_practice/  //? r.biomooc.com
- QQ group 生物信息与R语言: 187923577




# Other resource

- R 多元统计分析 https://yilewang.github.io/MSA/intro




# Bookdown

This is a book based on R Markdown and **bookdown** (https://github.com/rstudio/bookdown). Please see the page "[Get Started](https://bookdown.org/yihui/bookdown/get-started.html)" at https://bookdown.org/yihui/bookdown/ for how to compile this example into HTML. You may generate a copy of the book in `bookdown::pdf_book` format by calling `bookdown::render_book('index.Rmd', 'bookdown::pdf_book')`. More detailed instructions are available here https://bookdown.org/yihui/bookdown/build-the-book.html.

You can find the preview of this example at https://bookdown.org/yihui/bookdown-demo/.






## Build This Book

### How to Build and publish?

- push master with code;
- push gh-pages with html and figs.


```
dir: /home/wangjl/data/rmarkdown_demo/bookdown-demo-main/

1. 修改好后，增加版本号 index.Rmd 和 changeLog.txt 中一致
2. > build
3. push
$ git add .
$ git commit -m 'xxx'
$ git push origin master

3. $ mv docs docs2
```


```
1. $ git checkout gh-pages
2. replace docs/
$ rm -rf docs
$ mv docs2 docs

$ git add docs/
$ git commit -m '20220118'
$ git push origin gh-pages

$ git checkout master
> build # again
```

