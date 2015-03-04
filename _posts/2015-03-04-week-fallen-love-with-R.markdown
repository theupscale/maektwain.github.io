---
layout: post
title:  "The love with R-Matrices Week One"
date:   2015-03-04 22:02:00
categories: r
author: Saransh Sharma
---

Matrices are vectors with dimension attributes , the dimension attribute is itself an integer vector of length 2 (nrow,ncol). Yeah right 
it is that matrices we are talking about which we use in mathematics and its quite super easy in R 

{% highlight R %}
    m <- matrix (nrow=2, ncol=3)
    m
          [,1]  [,2] [,3]
    [1,]    NA    NA   NA
    [2,]    NA    NA   NA
    
    dim(m)
    [1] 2 3
    
    attributes(m)
    $dim
    [1] 2 3
{% endhighlight %}

### Matrices are constructed column wise so entries would start from upper-left corner to down to columns

{% highlight R %}
    m <- matrix(1:6, nrow=2, ncol=3)
    m 
            [,1] [,2] [,3]
    [1,]       1    3    5
    [2,]       2    4    6

{% endhighlight %}

###How to create matrices directly from vectors

{% highlight R %}
    m <- 1:10
    m 
    [1] 1 2 3 4 5 6 7 8 9 10
    dim (m) <- c(2,5)
    m
        [,1] [,2] [,3] [,4] [,5]
    [1,]   1    3    5    7    9
    [2,]   2    4    6    8   10
{% endhighlight %}

###c-binding and r-binding 
Column binding and Row binding

{% highlight R %}
    x <- 1:3
    y <- 10:12
    cbind(x,y)
    
            x  y
    [1,]    1  10
    [2,]    2  11
    [3,]    3  12
    ##similarly rbinding
    
    x <- 1:3
    y <- 10:12
    rbind(x,y)
    
        [,1]  [,2]  [,3]
    x      1     2     3
    y     10    11    12
{% endhighlight %}


###Notes

