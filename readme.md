---
title: Subclassing and Interfaces
type: Homework
duration: "1:00"
creator:
    name: Charlie Drews
    city: NYC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Subclassing, Abstract Classes, and Interfaces

> ***Note:*** _You can discuss with classmates, but everyone must submit their own answers_

## Exercise

#### Requirements

- Fork this repo, then add your answers direcly to this **readme.md** file
  - After forking, you can clone, edit the readme in the text editor of your choice, and push back to Github...
  - Or, you can edit the readme [right from the browser](https://help.github.com/articles/editing-files-in-your-repository/)
- After adding your answers, submit a **pull request**

#### Questions

1. What is the difference between *member variables* (also called *instance variables*) and *class variables* (w/ keyword `static`)? Which can be accessed without creating an instance of the class?

	Answer: A class variable can be accessed without creating an instance of the class because it is shared by all instances.

2. Does it make sense to write  *getter* and *setter* methods for a `public` member variable? What about `private` variables?

	Answer: Writing getter and setter methods is better for private variables as it allows you to access private variables, for public member variables, you can already access them.

3. What are some benefits of making member variables `private`?

	Answer: Making a member variable private is beneficial because it security in your code from other developers making changes that you would not ordinarily authorize.

4. If class A extends class B, which is the super class and which is the sub class? Which would you call parent, and which would you call child?

	Answer: Class B would be the Parent aka the super class... Class A would be the Child aka the sub class... assuming I'm reading that correctily "public class A extends class B"

5. What does it mean for a class to *inherit* methods and/or variables from its parent class?

	Answer: inheriting means that you do not need to explicitly write all the methods from a parent class in its child class, rather you could call it using various methods but the "super" function works well.

6. Consider the following code, where class Refrigerator extends class Appliance, and `getTemperature()` is a method in Refrigertor, but NOT in Appliance:
  ```
  Appliance myAppliance = new Refrigerator();
  double temperature = myAppliance.getTemperature();
  ```
  Why will this call to `getTemperature()` cause an error? How will *casting* help solve this issue?

  **I am not sure about this one, I will talk to the TA about it this evening.

7. In a normal class (also called a *concrete* class), do you need to *implement* all of the methods, or can your simply *declare* some? What about in an `abstract` class
	
	Answer: concrete methods require a method with a block for its relevant code.. Abstract methods are only declared without blocks, either in an abstract class, or as members of an interface. 

8. What about an `interface`? Can you implement any methods in an interface? Can you declare methods in an interface?

	Answer: An "interface" allows you to implement and declare methods.

9. Can you create an instance of an `abstract` class? Also, look up the Java keyword `final` and see if you can explain why a class CANNOT be both `abstract` and `final`.

	Answer: You can not create an instance of an abstract class. Although subclasses of an abstract class can. Final classes can't have subclasses, if a class were to be final and abstract, it would not be allowed to fully implement an abstract class.

10. What happens when a method *overrides* another method? If a parent and child class have methods with the same name, when you call that method on an instance of the child class, which implementation of the method will be executed?

	Answer: The child class will override the parent class implementing the childs method.

11. What is the relationship between `List`, `LinkedList`, and `ArrayList`? Why do we call a method *polymorphic* if it takes an input of type `List` rather than an input of type `LinkedList` or `Arraylist`, and why is that useful?
	
	Answer: We call a method polymorphic when it takes an input of type List rather than an input of the other types because it is the parent class referring to a child class object. List, LinkedList, and ArrayList are theoricially parent/superclass, child/subclass of each other. 

#### Deliverable

This file, with your answers added

## Additional Resources

Refer to the [Classes lesson](https://github.com/ga-adi-nyc/Course-Materials/tree/master/lessons/java-essentials/classes-lesson), the [Subclassing lesson](https://github.com/ga-adi-nyc/Course-Materials/tree/master/lessons/java-essentials/subclasses-lesson), and the [Interfaces & Abstract Classes lesson](https://github.com/ga-adi-nyc/Course-Materials/tree/master/lessons/java-essentials/interfaces-and-abstract-classes-lesson).

Feel free to google these concepts as well. There are plenty of Java tutorial websites and StackOverflow posts that can help you. But be sure to write up your answers in your own words - copying and pasting some text does NOT help you actually learn!
