---
layout: post
title:  "First Post!"
date:   2015-01-19 23:27:44
category: blog
tags: R
---
Here is something silly:

{% highlight r %}
Buffalo <- function(){
  word <- match.call()[[1]]
  sentence <- rep(as.character(word), 8)
  indices <- !(1:8 %in% c(1, 3, 7))
  sentence[indices] <- tolower(sentence[indices])
  return(paste0(paste(sentence, collapse=' '), '.'))
}
Buffalo()
# [1] "Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo."
{% endhighlight %}

Inspired by the relevant [wiki page][buffalo x8].

Making this site with the help of [Jekyll][jekyll]. I'm excited to see what I can do with it.

[buffalo x8]:  http://en.wikipedia.org/wiki/Buffalo_buffalo_Buffalo_buffalo_buffalo_buffalo_Buffalo_buffalo
[jekyll]:      http://jekyllrb.com
