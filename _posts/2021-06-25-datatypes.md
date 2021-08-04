---
layout: author
author: okey
Primitive Data Types
---

Don't let the word "primitive" bamboozle you here. It is just the way that textbooks refer 
to the kind of classification that pops up in your head whenever the word "data" is mentioned:
- the age of a student (int)
- the amount of money that is left in your bank account (double)
- the type of data that could be used to express Nigeria's population (long)
- the type of data that says type 'm' if you are male, 'f' if you are female (char)
- Your answer when asked, "You live in Lagos - true or false?" (boolean)

Now that we know what primitive data looks like, we need to ask ourselves what data would look 
like if it is not primitive. To discover which data is not primitive, we need to look at classes 
and objects.

When we define a class in Java, we do so in the knowledge that we can always create an object 
out of the newly defined class. For example, if we define a class called Teacher, then we could 
always create an object of the Teacher class like this:

Teacher tagbo = new Teacher();

Now we have an object of the Teacher class, and we can use "tagbo" to refer to that object. 
What is not so obvious, however is that Teacher is now a new kind of data, and "tagbo" gives
us the means to refer to this particular Teacher object. We say that "tagbo" is a reference 
to a Teacher object.

Herein lies the difference between a data type that is primitive, and one that is not: 
the age of a teacher is of type int, a primitive data type; "tagbo", used above to refer to a 
Teacher object is a data type, but not a primitive data type. It is a reference to a Teacher 
object.

Please note that a reference to a Teacher object is barely the tip of the iceberg because Java has 
already defined many, many classes that we can use in our code. A major example of such classes is 
the String class, as demonstrated in the following usage:

String sule = new String("Sule Maikirga");

System.out.println(sule);    // prints Sule Maikirga

Now, if you ask us, "Is sule a primitive data type?" we will say "No!"
And if you ask us, "What type of data is sule?" we will say "A reference to a String object."
