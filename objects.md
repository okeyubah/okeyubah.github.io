---
layout: post
chapter: 2
pageno: 14
title: "More about Java objects"
---


An object is usually derived from a class. This implies that you start by defining a class,
and then you create an object out of that class. Here is an example:

Because it has more than three thousand students, and admits a couple of hundreds every year,
a university has accepted a plan by its IT department to define a Student class. The Vice 
Chancellor has now been convinced that, once the Student class has been defined, a Student 
object will be created out of that class to represent each individual student. This means that out of
one class you define, you can create thousands of objects. Below is our first attempt to define
the Student class:

```
class Student {
  int age;
}
```


At this stage, our Student class has just one member (age). The type of age is int. This kind of member 
is also called an instance variable. What this means is that each time a new instance (a new object) of 
the Student class is created, that instance will contain a piece of data called age.

To improve upon our Student class, we will ensure that it has two new members: setAge() and getAge().
These additions are not the same kind member as age. The two new members are called methods, while age is 
an instance variable. Methods are required to enable us manipulate data, such as may be contained in 
instance variables like age. This is what an improved definition of the Student class might look like:

```
class Student {
  int age;
  void setAge(int newAge) {
    age = newAge;
  }
  void getAge() {
    return age;
  }
}
```

Now we can create an object of the Student class like this:
```
public class Registrar {
  public static void main(String[] args) {
    Student uche = new Student();
    uche.setAge(15);
    uche.getAge();    //15
  }
  ```
}

There is a lot to unpack here, but we will be doing that in a future post. Suffice it 
to say that we have defined a class named Student. Inside another class named Registrar, we have created 
an object of the Student class. To access this newly created object, we use an object reference called uche. 
Using uche, we are able to access the two methods defined in the Student class. By using these 
two methods, setAge() and getAge(), we are able to access age, the only instance variable defined in
the Student class.
