---
layout: post
author: okey
title: "How to define a method"
---
 
A Java method is made up of a number of component parts, as demonstrated in our definition of the Student class:
- Name: Every method requires a name, like getAge.
- Return type: Every method must either return a value, 

or state clearly that it does not return any value.

Confused? Let's take that line again. 
When you define a method, you need to tell the compiler whether 
your method returns any value. If your method does not return any value, then your job is lighter: 
Just use the word 'void', as shown below:

```
void setAge

```

Now the compiler knows that 'setAge' is a method that does not return any value.

And if your method returns a value? Then you need to tell the compiler what type of value is 
returned by your method. Below is how to do that:

```
int getAge

```

Now the compiler knows that 'getAge' is a method that returns a value, and that the type of value returned by 'getAge' is int.
