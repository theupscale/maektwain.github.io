---
layout: post
title:  "R-console input and evaluation-Week 1"
date:   2015-03-04 22:32:00
categories: r
author: Saransh Sharma
---

Once i have downloaded the R base package from CRAN , the shell will open and like any other shell you can input your commands but what commands? yeah pretty neat, because we havent learned anything
about the syntax of R but before that we need to see basics, 

###Entering Input

- This symbol is an assignment operator `<-`

So we can now enter few commands for assigning values like this 

- `msg <- "hello"`  Right way
- `msg <- `         Wrong way because it is incomplete
- commenting `msg <- ## Incomplete expression with comments` `## here used are the comment syntax`

###Evaluation 

{% highlight R %}
    x <- 5 ## nothing will print
    x ## auto printing
    [1] 5
    print (x) ## explicit printing
    [1] 5
    
{% endhighlight %}


###Notes

-The `[1]` indicates `x` is vector and `5` is the element
    

    