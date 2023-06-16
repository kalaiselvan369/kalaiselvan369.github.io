---
layout: post
title:  "Nice Features of Kotlin Part -1 "
date:   2023-06-09 11:38:38 +0530
categories: jekyll update
tag: kotlin
---

![post cover](/assets/kotlin-nice-feature-1.jpeg){: width="250" }

Named & Default arguments, Data classes, Safe calls, String template and more...
<!--more-->

## Named and Default Arguments

1. Default arguments simplify functions with longer arguments. 
2. Named arguments improves code redability

{% gist c80a6a9c94604ef0fa807499804de973 %}


## String template

Programmatic way to generate a string

{% gist b39568f901cb235fbb1e4865551084e3 %}


## Operator Overloading

Custom implementations for the predefined set of operators on types.

### Unary Operators

`+a` means a.unaryPlus()

`-a` means a.unaryMinus()

`!a` means a.not()

### Increment & Decrement Operators

`a++` means a.inc()

`a--` means a.dec()

### Arithmetic Operators

`a + b` means a.plus(b)

`a - b` means a.minus(b)

`a * b` means a.times(b)

`a % b` means a.rem(b)

`a..b` means a.rangeTo(b)

`a % b` means a.div(b)

### Indexed Access Operators

`a[i]` means a.get(i)

### Invoke Operator

`a()` means a.invoke()

`a(i)` means a.invoke(i)

{% gist 75a0d383adde93e8deba31a6988f9bf7 %}


## Extension Function

Extension functions add additional member functions to the existing class without altering the class.
Extension functions can access only the public members of the receiver type

{% gist e9c5949586c9ebf91db1719ff61775a8 %}


## Using `when` as statement and expression

It is conditional expression with multiple branches.

{% gist 80796594f5a21f50ebaa6b31593e4431 %}


## Using `enums`

1. Class with fixed number of instances.
2. Semicolon should be added at the last enum instance when we additionally include class members.

{% gist 9c9092fec8d4f41630a40b40dea323f0 %}


## Dealing with `null`

To avoid null pointer exception in code, we can use some checks

1. Safe call  `?.`
2. Elvis `?:`
3. Non-null assertion `!!` (Use only if mandatory)

{% gist 4fc3e728dfbd657c5a54d5a37c509578 %}

## Data class

1. Class to hold data
2. Class Constructor should contain at-least one parameter 
3. Compiler only uses the properties defined inside the primary constructor for the automatically generated functions.
4. Automatically generated functions are `equals()`, `hashCode()`, `toString()`, `componentN()`
5. `copy()` is special automatically generated functions which allow to access properties declared in the body as well.

{% gist 4b05c87d173222c76ca7f6174c5bae2e %}
