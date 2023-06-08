---
layout: post
title:  "Kotlin Basics"
date:   2023-06-07 16:11:38 +0530
categories: jekyll update
tag: kotlin
---
![Kotlin Logo](/assets/kotlin-logo.png)

Kotlin Basics that all developer should learn before diving into intermediate and advanced topics.
<!--more-->

## Entry point

`main` function is the entry point to the Kotlin program. 

`main` function is automatically invoked when Kotlin program is executed

`main` function can contain a parameter or be empty

if `main` function contain's a parameter then the type of the parameter should be `Array<String>`

{% gist c1715cccf0bb1c34bffcf34e52d27a2b %}


## Using val and var

`val` means value. It can be initialized and it cannot be reassigned.

`var` mean variable and it is mutable

### Syntax

```kotlin

val identifier = initalization

var identifier = initalization
```

`identifier` refers to elements in a program

{% gist 1ec010e9f0563ffce6bffca2927778eb %}

