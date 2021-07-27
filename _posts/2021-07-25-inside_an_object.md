---
layout: post
author: okey
---
Page 67 - Methods of the String class

First, a look at the two methods of the Student class:

```
public class Student {

  int age;
  
  void setAge(int newAge) {
    age = newAge; 
  }
  
  int getAge() {
    return age; 
  } 
  
  public static void main(String[] args) {
    Student uche = new Student(); 
    uche.setAge(14); 
    int info = uche.getAge();
    System.out.println(info);         // 14
  } 
}

```
In the main() method, we create an object of the Student class.
A reference to this object is stored in 'uche'. We can invoke Student 
methods on this object reference called 'uche'. When we do that, 
we can also say that we are calling the methods on 'uche'. 
Here is an example:

```
uche.setAge(14);

```
Here, we are invoking setAge(), a method of the Student class. We are calling this 
method on uche, an object reference. The setAge() method takes one argument. The type 
of this argument is int. The compiler will not accept your code if you fail to provide 
this argument or if you provide an argument of the wrong type. Also, the compiler will
reject your work if you provide the wrong number of arguments. Fortunately, the compiler 
will not reject our code here because we have provided one argument, as required. 
Furthermore, the argument that we provided (14) happens to be just the type of argument 
(int) that is required. 
