---
layout: topic
title: Java classes
chapter: seven
pageno: 43
---

When you start writing Java code, the first thing you need to do is define a class. Thereafter, you can then create objects that belong to your new class. After you have created an object, you can use that object to accomplish some tasks. Confused?

Not to worry! We will only be looking at how to define classes at this stage. To define a class, you write code that starts with the word "class", followed by the name of the class, for example class Teacher. Next, you will provide your new class with a pair of curly braces "{}", as shown in this example: class Teacher {}.

Now you have a class called Teacher. Notice that the name of the class starts with a capital letter. The name of any class you define should also start with a capital letter.

Unfortunately, there is nothing within the curly braces, "{ }" of our new class. This means that our new class is empty. This also means that our new class is totally useless. To be of any use, our new class should have any number of "members". A member could be a piece of data, like the teacher's age. A member could also be a "method", lines of code that prescribe how to manipulate such data. A more useful definition of the Teacher class might look like this:

class Teacher {
      int age;
}

This new definition of the Teacher class contains a member called age. The type of this member is int. We know that this is the case because the word "age" is preceded by the word "int". Java is notoriously strict about the type of data you use in your programs, hence the need to put the word int in front of age. That way, everyone can see that the piece of data called age is of a particular type: int. In case you are still wondering, an int is a kind of number, the kind of number that can hold a person's age.

Java has other types of data, like "String", which we could use to hold the teacher's name. Thus, if we wanted the teacher's age to be replaced by their name, then our definition of the Teacher class would look like this:

class Teacher {
      String name;
}

Notice that the word int has now been replaced by another word, String. This is because age and name are not the same type of data. While age is an int, name is actually a String.
