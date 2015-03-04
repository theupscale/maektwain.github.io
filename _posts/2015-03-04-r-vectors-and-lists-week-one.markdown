---
layout: post
title:  "R-Vectors and Lists-Week 1"
date:   2015-03-04 23:12:00
categories: r
author: Saransh Sharma
---

I wouldn't do much of writing here because when we do coding we simply do that, 

###Creating Vectors --How to create vectors in R

The `c()` function can be used to create vectors of objects

{% highlight R %}
    x <- c (0.5,0.6) ##numeric
    x <- c (TRUE,FALSE) ##logical
    x <- c (T,F) ##logical
    x <- c ("a", "saransh sharma", "any") ##character
    x <- c (9:29) ##integer
    x <- c (1+0i, 2+4i) ##complex
{% endhighlight %}

Use the `vector()` function

{% highlight R %}
    x <- vector ("numeric", length = 10)
    x
    [1] 0 0 0 0 0 0 0 0 0 0

{% endhighlight %}

###Mixing Onjects

{% highlight R %}
    y <- c (1.7, "a")  ## R will treat this as character because of the object high value in decimal comparison like 1.7 < "a" and here "a" is equal to 96 in decimal you can also compare in r console like this 
                       ## "a" < 1
                       ## it will return FALSE
    y <- c (TRUE, 2)   ## numeric
    y <- c ("a", TRUE) ##character
    

{% endhighlight %}

When different objects are mixed in a vector coercion occurs which makes he 