- Inheriting attributes
- Inheriting and Overriding methods

- **Inheritance**: a form of abstraction that permits "generalisation" of similar attributes/methods of classes; analogous to passing genetics on to your children.
- **Superclass**: "Parent" (base) class in the inheritance relationship; provides general information to its "child" class.
- **Subclass**: "Child" (derived) class in the inheritance relationship; inherits common attributes and methods from the "parent class".

Main idea:
![Screenshot 2024-08-25 at 11.11.38](attachments/Screenshot%202024-08-25%20at%2011.11.38.png)
# Inheriting attributes and methods
For example, without implementing inheritance:
![Screenshot 2024-08-25 at 11.15.07](attachments/Screenshot%202024-08-25%20at%2011.15.07.png)
![Screenshot 2024-08-25 at 11.15.22](attachments/Screenshot%202024-08-25%20at%2011.15.22.png)

Now, after implementing inheritance:

![Screenshot 2024-08-25 at 11.15.49](attachments/Screenshot%202024-08-25%20at%2011.15.49.png)
![Screenshot 2024-08-25 at 11.16.12](attachments/Screenshot%202024-08-25%20at%2011.16.12.png)
# Defining Inheritance
![Screenshot 2024-08-25 at 11.17.48](attachments/Screenshot%202024-08-25%20at%2011.17.48.png)
# Creating objects
![Screenshot 2024-08-25 at 11.19.10](attachments/Screenshot%202024-08-25%20at%2011.19.10.png)

FIRST TWO WAYS ARE VALID. NOT THE THIRD ONE.
# Initialising with constructors
Keyword `super` can be used to call the constructor of the superclass. e.g.,
![Screenshot 2024-08-25 at 11.25.26](attachments/Screenshot%202024-08-25%20at%2011.25.26.png)

- only be used within the subclass constructor
- must be the first statement within the subclass constructor (if used)
- parameter types to super constructor call must match that of the constructor call in the base class.
![Screenshot 2024-08-25 at 12.01.42](attachments/Screenshot%202024-08-25%20at%2012.01.42.png)
# Inheriting and Overriding methods
## Implementing method inheritance
![Screenshot 2024-08-25 at 12.48.52](attachments/Screenshot%202024-08-25%20at%2012.48.52.png)
![Screenshot 2024-08-25 at 12.49.03](attachments/Screenshot%202024-08-25%20at%2012.49.03.png)
## Testing method inheritance
![Screenshot 2024-08-25 at 12.49.31](attachments/Screenshot%202024-08-25%20at%2012.49.31.png)

![Screenshot 2024-08-25 at 12.49.49](attachments/Screenshot%202024-08-25%20at%2012.49.49.png)

![Screenshot 2024-08-25 at 12.51.12](attachments/Screenshot%202024-08-25%20at%2012.51.12.png)
![Screenshot 2024-08-25 at 12.51.31](attachments/Screenshot%202024-08-25%20at%2012.51.31.png)
## Definitions
- **Overriding**: declaring a method that exists in a superclass again in the subclass, with the same signature. Methods can only be overriden by subclasses.
- **Overloading**: declaring multiple methods with the same name but different signatures (parameters). Superclass methods can be overloaded in subclasses.
- Both **overriding** and **overloading** are examples of **polymorphism**.
## Why override?
![Screenshot 2024-08-25 at 12.58.58](attachments/Screenshot%202024-08-25%20at%2012.58.58.png)
# Extension through overriding
## Put common part in parent, specific part in child
Keyword `super` refers to the attributes and methods of the parent object; just like `this` is a reference to itself.
![Screenshot 2024-08-25 at 19.41.17](attachments/Screenshot%202024-08-25%20at%2019.41.17.png)
![Screenshot 2024-08-25 at 19.41.33](attachments/Screenshot%202024-08-25%20at%2019.41.33.png)
![Screenshot 2024-08-25 at 19.41.47](attachments/Screenshot%202024-08-25%20at%2019.41.47.png)
## Improve encapsulation: person using class doesn't need to explicitly call `.isValidMove()`
![Screenshot 2024-08-25 at 19.47.34](attachments/Screenshot%202024-08-25%20at%2019.47.34.png)
![Screenshot 2024-08-25 at 19.47.53](attachments/Screenshot%202024-08-25%20at%2019.47.53.png)
![Screenshot 2024-08-25 at 19.48.07](attachments/Screenshot%202024-08-25%20at%2019.48.07.png)
# NOTE ON METHOD OVERRIDING
![Screenshot 2024-08-25 at 20.07.22](attachments/Screenshot%202024-08-25%20at%2020.07.22.png)
# NOTE: Methods of the superclass CANNOT access public attributes of a subclass. Only the other way around - indirectly - through overriding.
