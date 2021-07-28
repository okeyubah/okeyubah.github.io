---
layout: post
author: okey
---

How to define a method Page 81
A Java method has a number of component parts, as demonstrated in our definition of the Student class:
**Name:** Every method requires a name, like getAge.
----------------------------------------------------
**Return type:** Every method must either must either return a value, 
--------------------------------------------------------------------
or state clearly that it does not return any value.

Confused? Let's take that line again. 

When you define a method, you need to tell the compiler whether 
your method returns any value. If your method does not return a value, then your are lucky: Your 
problems at this level can be used by using the word void, like this:

```
void setAge

```

The word 'void', above, tells the compiler that the method 'setAge' does not return any value.

And if your method returns a value? Then you need to tell the compiler what type of value your method returns, like this:

```
int getAge

```

The word 'int', above, tells the compiler that the method 'getAge' returns a value, and that the type of that value is int.

