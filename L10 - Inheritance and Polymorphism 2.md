- Inheritance and information hiding
- The Object Class
- Abstract classes
# Inheritance and Information Hiding
## `private` methods cannot be overridden
In this case, say something defined as `Piece rook = new Rook()`, if you want to call `rook.isValidMove`, it won't override to the child method.
![Screenshot 2024-08-25 at 20.13.53](Screenshot%202024-08-25%20at%2020.13.53.png)
## Restricting inheritance
![Screenshot 2024-08-25 at 20.15.38](Screenshot%202024-08-25%20at%2020.15.38.png)
![Screenshot 2024-08-25 at 20.16.10](Screenshot%202024-08-25%20at%2020.16.10.png)
## Access control - can the child class use/call parent class' attributes/methods?
![Screenshot 2024-08-25 at 20.25.30](Screenshot%202024-08-25%20at%2020.25.30.png)![Screenshot 2024-08-25 at 20.25.45](Screenshot%202024-08-25%20at%2020.25.45.png)![Screenshot 2024-08-25 at 20.28.41](Screenshot%202024-08-25%20at%2020.28.41.png)
SO TRY TO MAKE ATTRIBUTES PRIVATE AND DEFINE METHODS TO GET/SET THEM![Screenshot 2024-08-25 at 20.57.46](Screenshot%202024-08-25%20at%2020.57.46.png)![Screenshot 2024-08-25 at 20.58.09](Screenshot%202024-08-25%20at%2020.58.09.png)
![Screenshot 2024-08-25 at 20.58.24](Screenshot%202024-08-25%20at%2020.58.24.png)
## Inheritance and Shadowing
![Screenshot 2024-08-25 at 21.05.09](Screenshot%202024-08-25%20at%2021.05.09.png)
## Privacy and visibility modifiers summary
![Screenshot 2024-08-25 at 21.06.21](Screenshot%202024-08-25%20at%2021.06.21.png)
![Screenshot 2024-08-25 at 21.06.36](Screenshot%202024-08-25%20at%2021.06.36.png)
# The `Object` Class
- Every class in Java extends `Object` class.
- `toString` and `equals` methods are part of the `Object` class. So when we were define these methods in our classes, they were overriding the method in the parent class `Object`.
![Screenshot 2024-08-26 at 17.16.02](Screenshot%202024-08-26%20at%2017.16.02.png)
# `getClass` and `instanceOf`
![Screenshot 2024-08-26 at 17.17.14](Screenshot%202024-08-26%20at%2017.17.14.png)
# Upcasting and Downcasting
![Screenshot 2024-08-26 at 17.17.46](Screenshot%202024-08-26%20at%2017.17.46.png)
# Polymorphism
![Screenshot 2024-08-26 at 17.18.38](Screenshot%202024-08-26%20at%2017.18.38.png)
# The Abstract Class
## Definition
Some classes aren't meant to be instantiated (using `new`) because they aren't completely defined. E.g., `
```
Piece p1 = new Piece();
p1.move()
```
This doesn't make sense, because `move()` is specific to a piece type (rook, bishop, etc.)
So they should be an abstract class.

- **Abstract Class**: a class that represents common attributes and methods of its subclasses, but that is missing some information specific to its subclasses; cannot be instantiated.
- **Concrete Class**: a class with well defined, specific implementations for all actions it can take.

E.g.,
![Screenshot 2024-08-26 at 17.25.40](Screenshot%202024-08-26%20at%2017.25.40.png)
## Abstract methods
![Screenshot 2024-08-26 at 17.26.19](Screenshot%202024-08-26%20at%2017.26.19.png)
NO IMPLEMENTATION - JUST DECLARING (end with semi-colon)
## Abstract vs Concrete
Abstract classes are identical, except:
- They may have abstract methods (not mandatory)
- Classes with abstract methods MUST be declared abstract
- Cannot be instantiated (using `new`)
- Represents an 'incomplete' concept, rather than a thing that is part of a problem
## Abstract Classes Example
![Screenshot 2024-08-26 at 17.34.50](Screenshot%202024-08-26%20at%2017.34.50.png)
![Screenshot 2024-08-26 at 17.34.59](Screenshot%202024-08-26%20at%2017.34.59.png)
![Screenshot 2024-08-26 at 17.35.08](Screenshot%202024-08-26%20at%2017.35.08.png)
![Screenshot 2024-08-26 at 17.35.16](Screenshot%202024-08-26%20at%2017.35.16.png)
# Types of Inheritance
![Screenshot 2024-08-26 at 17.36.46](Screenshot%202024-08-26%20at%2017.36.46.png)