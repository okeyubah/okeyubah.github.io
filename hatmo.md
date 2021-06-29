---
layout: post
author: okey
---
Page 64: More about Java Classes and Objects

An object is usually derived from a class. This implies that you start by defining a class,
and then you create an object out of that class. Here is an example:

Because it has more than three thousand students, and admits a couple of hundreds every year,
a university has accepted a plan by its IT department to define a Student class. The Vice 
Chancellor has now been convinced that, once the Student class has been defined, a Student 
object will created out of that class to represent each individual. This means that out of
one class you define, you can create thousands of objects. Below is our first attempt to define
the Student class:

class Student { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;int age;<br> }

At this stage, our Student class has just one member, age. The type of age is int. This kind of member 
is also called an instance variable. This means that each time a new instance (a new object) of 
the Student class is created, that object will contain a piece of data called age.

To improve upon our Student class, we will ensure that it has two new members: setAge() and getAge().
These two members are not the same kind as age, an instance variable. Instead, they are called 
methods: they help us to manipulate the value contained in our only instance variable, age. This is 
what our new definition of the Student class looks like:
