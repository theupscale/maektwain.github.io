---
layout: post
title:  "R-Data Types and other details-Week 1"
date:   2015-03-04 22:55:00
categories: r
author: Saransh Sharma
---

As we have enough basic knowledge about R now like any other programming language R has suite of data objects we will be dealing with vectors
because it is lot like arrays the

###Objects
R has five atomic classes of objects

- character
- numeric(real numbers)
- integer
- complex
- logical(true/false)

The most basic object is vector 

- A vector only contain objects of same class
- BUT one exception is a list, which is represented as a vector but can contain objects of different classes
- Empty vectors can be created with `vector()`

###Numbers

- Numbers in r are treated as numeric objects
- If you want an integer , explicitly specify L suffix
- `1` will return you only numeric one, but `1L` will return you integer
- Special number called `Inf` which represents infinity eg  `1/0; Inf` 
- `NaN` represents an undefined value "null" `NaN` is also a missing number we will later on study.

###Attributes 
R objects can have attributes

- names,dimnames
- dimensions (eg matrices)
- class
- length
- other user-defined attributes/metadata

Attributes of an object can be accessed using `attributes()` function

###Examples

In the next blog!