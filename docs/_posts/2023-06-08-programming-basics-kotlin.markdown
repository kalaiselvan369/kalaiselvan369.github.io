---
layout: post
title:  "Programming Basics using Kotlin"
date:   2023-06-08 17:11:38 +0530
categories: jekyll update
tag: kotlin
---

![post cover](/assets/post-1-cover.png){: width="250" }

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


## Data types

Each data has a type. Kotlin has predefined data types such as

1. Numbers  - Int, Float, Literal Constants
2. Characters
3. Strings
4. Booleans
5. Arrays
6. Unsigned Integer types - No negative value

### Integer types

1. Byte  ---> 8 bit values between -128 to 127
2. Short --> 16 bit values between -32768 to 32767
3. Int   ------> 32 bit values between -2<sup>31</sup> to 2<sup>31</sup> -1
4. Long  ---> 64 bit

{% gist 464f0fb96c408566de90488032c480f1 %}

### Floating point type

1. Float - single precision - 6 to 7 decimal points
2. Double - double precision - 15 to 16 decimal points

### Literal Constants

1. Decimal - 126
2. Long - 12490L
3. Hexadecimal - 0x0F
4. Binary - 0b00001011

{% gist aaae2004363965f1342741bf32a65970 %}

### Characters

Characters are represented by the type `Char`

Special characters start from an escaping backslash

1. `\t` – tab

2. `\b` – backspace

3. `\n` – new line (LF)

4. `\r` – carriage return (CR)

5. `\'` – single quotation mark

6. `\"` – double quotation mark

7. `\\` – backslash

8. `\$` – dollar sign

> Adding Int to a Char yields another Char

{% gist 464ce8ca09c3f3279ee081327a91b5b1 %}

### Boolean

1. `&&` (AND) logical `AND` or conjunction 
2. `||` (OR) logical `OR` or disjunction
3. `!` (NOT) logical `NOT` or negation

## Assignment Operators

{% gist 7e8536f87b32acb6cd0e73ea8c6153ca %}

## Increment and Decrement Operators

For post increment, i++

> first produce the result, then do the increment.
 
1. Store the initial value of `i` to a temporary storage `i0`.
2. Assign the result of `i0.inc()` to `i`.
3. Return `i0` as the result of the expression. That is why `j` value is 0

For pre increment, ++k

> first do the increment, then return the resulting value.

1. Assign the result of `k.inc()` to `l`.
2. Return the new value of `l` as a result of the expression.

{% gist 3d95a7eee899a579b046b2332ff36a9b %}

## Ranges

1. Using for loop with `in` keyword
2. Using Ranges with help of `..`, `until`, `downTo`, `step`
3. Looping Char `a`..`z`
4. Find Char in String using `in` keyword

{% gist 194582f654458e197b4158cd3563160d %}

## Using `in` keyword

`in` can be used for iteration in for loops and to check membership.

{% gist 3651e403aae9437b8b0f0b70e7e79d1f %}

## Expression 

Expression yields result

Example for expression: if-else as an expression

## Statement

Statement create side effect and doesn't produce result

Example for statement: for loop

{% gist 0c198d2a1702069912653377672f2262 %}


