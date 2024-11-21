# Singleton pattern
Ensure there is only one instance of the class

![center|300](Screenshot%202024-09-20%20at%2013.39.51.png)

![Screenshot 2024-09-20 at 13.41.07](Screenshot%202024-09-20%20at%2013.41.07.png)
![Screenshot 2024-09-20 at 13.53.10](Screenshot%202024-09-20%20at%2013.53.10.png)
Constructor is private!
If instance is not created, make a new one. Otherwise, return the current one
# Factory method pattern
You SHOULDN'T create objects in a class that uses the object because...
- ...it commits the class to a particular object
- ...you cannot change the instantiation without changing the class
The Factory method defines a separate operation for creating an object. So it creates an object by calling a factory method
![Screenshot 2024-09-20 at 15.40.54](Screenshot%202024-09-20%20at%2015.40.54.png)

![center|400](Screenshot%202024-09-20%20at%2015.41.16.png)

Example:
![Screenshot 2024-09-20 at 15.41.49](Screenshot%202024-09-20%20at%2015.41.49.png)
![Screenshot 2024-09-20 at 15.42.04](Screenshot%202024-09-20%20at%2015.42.04.png)
![Screenshot 2024-09-20 at 15.42.21](Screenshot%202024-09-20%20at%2015.42.21.png)
## Aim: to generalize object creation
- DELEGATES object creation to subclasses 
- ABSTRACTS object creation by using a factory method
- ENCAPSULATES objects by allowing subclasses to determine what they need
# Template method pattern & strategy pattern
 - Main goal of these 2 patterns: separate a generic algorithm from a detailed design.
 - Template method pattern uses **INHERITANCE**
 - Strategy pattern uses **DELEGATION**
# Template method pattern
## Without template method pattern...
![Screenshot 2024-09-20 at 23.36.34](Screenshot%202024-09-20%20at%2023.36.34.png)
![Screenshot 2024-09-20 at 23.36.54](Screenshot%202024-09-20%20at%2023.36.54.png)
... and what if we wanted to do this for double, float, etc.? We would have to make a class for bubble sorting an int, another class for bubble sorting a double, etc.
## With template method pattern
![Screenshot 2024-09-20 at 23.38.27](Screenshot%202024-09-20%20at%2023.38.27.png)
![Screenshot 2024-09-20 at 23.38.47](Screenshot%202024-09-20%20at%2023.38.47.png)
... then do another child class for `DoubleBubbleSorter`

**NOTE:** calling the `sort()` method in the child class calls the `doSort()` method in the parent class (the main implementation of the algorithm), which then calls `outOfOrder()` and `swap()` that is overridden in the child class.

![Screenshot 2024-09-20 at 23.41.49](Screenshot%202024-09-20%20at%2023.41.49.png)
## Aim of template method pattern: 
Define a skeleton of an algorithm as an abstract class, allowing its subclasses to provide concrete behavior
# Strategy pattern
- Using inheritance like in the template method pattern means that there is a strong dependency to the base class. E.g. although `outOfOrder()` and `swap()` are generic methods, they cannot be re-used because they inherit the `AbstractBubbleSorter` class - hence, if there was another algorithm that also uses `outOfOrder()` and `swap()`, we would have to rewrite these methods for that algorithm.
- The strategy pattern is an alternative method which seeks to mitigate this
## Strategy pattern example
You can create an instance of `BubbleSorterS` by passing a handle into its constructor: which could be `IntSortHandle`, `DoubleSortHandle`, etc. - which works because they all implement the `SortHandle` interface.
![Screenshot 2024-09-22 at 13.28.01](Screenshot%202024-09-22%20at%2013.28.01.png)
![Screenshot 2024-09-22 at 13.28.38](Screenshot%202024-09-22%20at%2013.28.38.png)
![Screenshot 2024-09-22 at 13.28.49](Screenshot%202024-09-22%20at%2013.28.49.png)
![Screenshot 2024-09-22 at 13.29.02](Screenshot%202024-09-22%20at%2013.29.02.png)
![Screenshot 2024-09-22 at 13.29.15](Screenshot%202024-09-22%20at%2013.29.15.png)
And now if another algorithm wants to use `SortHandle`, they just need to store an instance of `SortHandle` (delegation):
![Screenshot 2024-09-22 at 13.40.19](Screenshot%202024-09-22%20at%2013.40.19.png)
![Screenshot 2024-09-22 at 13.40.31](Screenshot%202024-09-22%20at%2013.40.31.png)
![Screenshot 2024-09-22 at 13.41.38](Screenshot%202024-09-22%20at%2013.41.38.png)
# Observer pattern
- There are situations where many objects (observers) depend on the state of one object (subject)
- An object managing a one-to-many dependency between objects is inflexible as 1) it tightly couples the subject to particular dependent objects, and 2) these tightly coupled objects are hard to implement, test, and maintain
- Using the observer pattern decouples the subject and observers using a publish-subscribe style communication pattern
![Screenshot 2024-09-22 at 16.27.16](Screenshot%202024-09-22%20at%2016.27.16.png)
![Screenshot 2024-09-22 at 16.27.25](Screenshot%202024-09-22%20at%2016.27.25.png)![Screenshot 2024-09-22 at 16.28.17](Screenshot%202024-09-22%20at%2016.28.17.png)
## Observer pattern example
![Screenshot 2024-09-22 at 16.28.34](Screenshot%202024-09-22%20at%2016.28.34.png)
![Screenshot 2024-09-22 at 16.28.57](Screenshot%202024-09-22%20at%2016.28.57.png)
![Screenshot 2024-09-22 at 16.29.12](Screenshot%202024-09-22%20at%2016.29.12.png)
