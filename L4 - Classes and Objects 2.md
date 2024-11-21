- Getters, Setters, and Constructors
- Static Attributes and Methods
- Standard Methods in Java
# Getters and Setters
- To initialise/update or access instance variables, we have to define specific methods.
- It is better to use getters and setters than directly accessing instance variables (explained later)
- Setter (mutator) method: `aCircle.setX(10.0); // to initialise or update instance variable`
- Getter (accessor) method: `aCircle.getX(); // to access instance variable`

Example:
![Screenshot 2024-07-31 at 15.44.34](Screenshot%202024-07-31%20at%2015.44.34.png)


![Screenshot 2024-07-31 at 15.44.58](Screenshot%202024-07-31%20at%2015.44.58.png)
# Constructors
`Circle aCircle = new Circle(); ` <-- The right side calls a class' constructor
- A constructor is a method used to create and initialise an object.
- Constructors have the same name as the class
- Constructors have no return value
- A class can have one or more constructors - which is dependent on the number of parameters (method overloading)
## Defining constructors
![Screenshot 2024-07-31 at 16.05.13](Screenshot%202024-07-31%20at%2016.05.13.png)

![Screenshot 2024-07-31 at 16.06.15](Screenshot%202024-07-31%20at%2016.06.15.png)

![Screenshot 2024-07-31 at 16.06.34](Screenshot%202024-07-31%20at%2016.06.34.png)
## Method overloading (as seen above)
- This is the ability to define methods with the same name but different signatures (type or number of arguments).
- **Method overloading** is a type of **polymorphism** (ability to process objects differently depending on their data type or class). 
## `this` Keyword
![Screenshot 2024-07-31 at 16.12.12](Screenshot%202024-07-31%20at%2016.12.12.png)
# Static attributes and methods
## Static attributes
Instance variables: one copy per object
Static variables: one copy per class (shared between objects)
![Screenshot 2024-07-31 at 16.18.00](Screenshot%202024-07-31%20at%2016.18.00.png)
![Screenshot 2024-07-31 at 16.18.28](Screenshot%202024-07-31%20at%2016.18.28.png)
## Static method
- Static methods are accessed using the name of the **class**, not the **object**.
- Static methods can only call other static methods
- Static methods can only access static data
- Try not to make all methods and attributes static - this is procedural programming

![Screenshot 2024-07-31 at 16.22.54](Screenshot%202024-07-31%20at%2016.22.54.png)
![Screenshot 2024-07-31 at 16.21.49](Screenshot%202024-07-31%20at%2016.21.49.png)
## Static members
![Screenshot 2024-07-31 at 16.41.57](Screenshot%202024-07-31%20at%2016.41.57.png)
# Standard Java methods
## adding `equals` method to the `Circle` class
![Screenshot 2024-08-06 at 14.20.08](Screenshot%202024-08-06%20at%2014.20.08.png)
## adding `toString` method to the `Circle` class
![Screenshot 2024-08-06 at 14.20.22](Screenshot%202024-08-06%20at%2014.20.22.png)
## adding `copy` constructor to the `Circle` class
![Screenshot 2024-08-06 at 14.20.50](Screenshot%202024-08-06%20at%2014.20.50.png)
