---
layout: post
title:  "OOP Basics using Kotlin"
date:   2023-06-09 11:38:38 +0530
categories: jekyll update
tag: kotlin
---

![post cover](/assets/oop-part-1.jpeg){: width="250" }

Working with classes, constructors and visibility modifiers in Kotlin
<!--more-->

## Object Oriented Programming

It is a computer programming paradigm based on the concept of objects. Object contains state 
in the form of attributes or properties and actions in the form of method or functions.

In OOP, we representing real world objects into a model/object to derive solution for a particular problem.

### Example 

Let's talk about computer monitor. It comes out with variety of size, color, model which we can call it as attributes
or properties and on, off, restart capabilities which we can call it as methods or functions.

## Class

- It is a user defined data type
- class declartion consists of class name, header(constructor, constructor parameter) and body.
- class body contains properties and functions
- member function means function defined within a class
- memeber property means val/var that belong to a class
- Object is derived from instantiating a class
- var or val is used to hold state of the object
- var enable us to rebind reference to different object
- Mutability means an object can change its state

{% gist f75b54708c9b7c4daa18a34f2e15e144 %}

## Constructors

Special type of member function to instantiate a class.

{% gist 1c93823b0b07fe71973440778791eac4 %}

## Visibility Modifiers

1. public 
2. private
3. protected
4. internal 

Let's see how visibility modifiers applies to class members

> Properties, Functions that belong to a class are called as class members

### Public

- Class members are accessible to anyone outside the class provided that the class containing the members is public.
- To a class be public we need not declare it explicitly `public`

### Private

Members visible only to other members of the same class

{% gist 6b109a2674701772a1d509a7228d93f3 %}

### Protected

Same as private but the members visible to the subclass also.

{% gist b3c8ef6a387c372ec70985c97c07ac23 %}

### Internal

`internal` is accessible only inside the module in which the classes, functions and properties are declared

### Top level Function | Property | Class

Classes, Functions and Properties that are declared inside a package within a file with extension `.kt`
are said to be top level. 

Top level functions, property and classes that are declared `private` are accessible 
only within the file where they are declared.

{% gist 33a1acd7caa1b8ceb7e2ee931a69fbed %}

`protected` modifier doesn't apply to top level class, property and function.

## Packages

Enables resuability and grouping classess, functions and property.

{% gist 0b913eaa2681853558bbb742abe70328 %}
