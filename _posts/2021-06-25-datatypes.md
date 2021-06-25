---
layout: author
author: okey
---
Page 29 - Primitive Data Types

Don't let the word "primitive" bamboozle you here. It is just the way that textbooks refer 
to the kind of information that pops up in your head whenever the word "data" is mentioned:
- the age of a student (int)
- the amount of money that is left in your bank account (double)
- the type of data that could be used to express Nigeria's population
- the type of data that you could use to answer a question like "You live in Lagos?" (boolean)

Now that we know what primitive data looks like, we need to ask our what data would look 
like when it is not primitive. To discover which data is not primitive, we need to look at classes 
and objects.

When we define a class in Java, we do so in the knowledge that we can always create an object 
out of the newly defined class. For example, if we define a class called Teacher, then we could 
always create an object of the Teacher class like this:

Teacher tagbo = new Teacher();

Now we have an object of the Teacher class, and we can use "tagbo" to refer to that object. 
What is not so obvious, however is that Teacher is now a new kind of data, and "tagbo" gives
us the means to refer to this particular Teacher object. We say that "tagbo" is a reference 
to a Teacher object.

Herein lies the difference between data that is primitive like the age of a teacher, and a 
reference to a Teacher object. A teacher's age is primitive data. A reference to a Teacher 
object is definitely not primitive data.
