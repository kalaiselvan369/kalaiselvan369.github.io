---
layout: post
title:  "OOP Basics using Kotlin"
date:   2023-06-09 10:38:38 +0530
categories: jekyll update
tag: kotlin
---

![post cover](/assets/oop-part-1.jpeg){: width="250" }

Working with classes, constructors and visibility modifiers in Kotlin
<!--more-->

## OOP Definition

It is a computer programming paradigm based on the concept of objects. Object contains data 
in the form of attributes or properties and actions in the form of method or functions.

We are representing real world objects into a model or object that software program can interpret.

### Example 

Let's take a computer monitor which has size, color, model number which we can call it as attributes
or properties and on, off, restart capabilities as methods or functions.

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

## Access Modifiers

1. public
2. private
3. protected
4. internal - it is accessible only inside the module in which the class/function/property is declared

### Top level function/property/classes

Top level functions, property and classes that are declared `private` are accessible 
only within the file where they are declared.

{% gist 33a1acd7caa1b8ceb7e2ee931a69fbed %}

## Packages

Enables resuability and grouping classess, functions and property.

{% gist 0b913eaa2681853558bbb742abe70328 %}
