- Introducing Classes and Objects
- Defining Classes
- Using Classes

# Procedural vs Object oriented programming

The key difference is in abstraction. Procedural languages like C use functions. Object oriented languages like C++ and Java use abstract data types (ADT) - which contains data and functions that operate on data.

In Java, a class is an implementation on an ADT
# Classes
- Represents an entity (e.g. a student, a book, university subject, etc.) or even more abstract things (e.g. a list, a string, etc.) - things that have common properties.
- Fundamental unit of abstraction in OOP.
- Has **attributes** and **methods**.
- Defines a new data type.
# Object
- Instances of a class.
- Contains a state, e.g. a student has a student id, name, and other credentials.
- "X is of type A", "X is an object of the class A", "X is an instance of the class A" are all equivalent.  
# OO features
![Screenshot 2024-07-29 at 10.50.55](Screenshot%202024-07-29%20at%2010.50.55.png)![Screenshot 2024-07-29 at 10.51.08](Screenshot%202024-07-29%20at%2010.51.08.png)
![Screenshot 2024-07-29 at 10.51.30](Screenshot%202024-07-29%20at%2010.51.30.png)
# Defining a class
![Screenshot 2024-07-29 at 10.53.57](Screenshot%202024-07-29%20at%2010.53.57.png)
- A class should be Capital
## Adding attributes
![Screenshot 2024-07-29 at 10.56.40](Screenshot%202024-07-29%20at%2010.56.40.png)
## Adding methods
![Screenshot 2024-07-29 at 10.59.17](Screenshot%202024-07-29%20at%2010.59.17.png)
**NOTE:** Local variables are inside the method as opposed to instance variables which are outside the method declaration.

![Screenshot 2024-07-29 at 11.00.29](Screenshot%202024-07-29%20at%2011.00.29.png)
# Using a class
## Creating objects
![Screenshot 2024-07-29 at 11.14.28](Screenshot%202024-07-29%20at%2011.14.28.png)
Lines 5 and 6 are instantiating an object (creating an object of a class). Without instantiating (lines 5 and 6), `aCircle` and `bCircle` are null references (point to null). `new` is analogous to `malloc` in C.

## Assigning references of a class
![Screenshot 2024-07-29 at 11.16.53](Screenshot%202024-07-29%20at%2011.16.53.png)
Line 7 shows assigning references of a class. No need to deallocate memory for object Q, there is automatic garbage collection in Java. 
## Using instance variables and methods
![Screenshot 2024-07-31 at 15.22.37](Screenshot%202024-07-31%20at%2015.22.37.png)

## An example using `Circle` class:
![Screenshot 2024-07-31 at 15.23.21](Screenshot%202024-07-31%20at%2015.23.21.png)

# The `main` method
![Screenshot 2024-07-31 at 15.30.08](Screenshot%202024-07-31%20at%2015.30.08.png)



