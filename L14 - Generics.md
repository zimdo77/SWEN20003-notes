- Understand generic classes in Java
- Use generically typed classes
- Define generically typed objects
# `Comparable` interface
![Screenshot 2024-09-18 at 15.23.38](Screenshot%202024-09-18%20at%2015.23.38.png)
![Screenshot 2024-09-18 at 15.24.16](Screenshot%202024-09-18%20at%2015.24.16.png)
THE TYPE MUST BE STATED WHEN A CLASS IMPLEMENTS THIS INTERFACE
## Example of class implementing `Comparable` interface
![Screenshot 2024-09-18 at 15.29.35](Screenshot%202024-09-18%20at%2015.29.35.png)
If it were class `Book`, then the implemented method is `compareTo(Book book)`
## Why use generic types?
**NOTE:** by using generic types (e.g. generic `Comparable`), 1) this allows for code reuse for many types, and 2) Type-safe: you don't have to assert the correct type before comparing because it would have already raised a compile-time error.
![Screenshot 2024-09-18 at 15.48.39](Screenshot%202024-09-18%20at%2015.48.39.png)
![Screenshot 2024-09-18 at 15.49.06](Screenshot%202024-09-18%20at%2015.49.06.png)
# `<ArrayList>` class

- A **Generic** class
- Similar to a list in Python
- More functionality than an array: resize-able, no effort to add and remove elements
![Screenshot 2024-09-18 at 16.08.32](Screenshot%202024-09-18%20at%2016.08.32.png)

![Screenshot 2024-09-18 at 16.09.26](Screenshot%202024-09-18%20at%2016.09.26.png)
## Properties of `<ArrayList>`
### Pros
- iterated using 'for-each' loop
- Automatically handles resizing
- can: insert, remove, get, and modify (and many more) elements at any index
- Inherently able to `toString()`
### Cons
- Cannot be indexed using [ ]
- Although an ArrayList grows automatically, it doesn't shrink automatically, so it can consume more memory than needed. Use `trimToSize()` to release excess memory
- Cannot store primitive data types (int, float, etc. )
# Generic classes
**Definition**: A class that is defined with an arbitrary type for a field, parameter, or return type

Notes:
- The type parameter is included in angular brackets after the class name in the class definition heading: e.g. `public class Sample<T>`
- A type parameter can have any reference type (i.e. any class type)
- Traditionally use a single upper case letter like `T` or `U`.
## Example: single type
![Screenshot 2024-09-18 at 21.46.22](Screenshot%202024-09-18%20at%2021.46.22.png)
## Example: multiple types
![Screenshot 2024-09-18 at 21.48.35](Screenshot%202024-09-18%20at%2021.48.35.png)
![Screenshot 2024-09-18 at 21.49.10](Screenshot%202024-09-18%20at%2021.49.10.png)
# Bounded Type Parameters
You can add constraints for the types. Note: extends here means something different
![Screenshot 2024-09-18 at 21.50.24](Screenshot%202024-09-18%20at%2021.50.24.png)
# Generic methods
**Definition**: a method that accepts arguments, or returns objects of an arbitrary type
![Screenshot 2024-09-18 at 22.08.00](Screenshot%202024-09-18%20at%2022.08.00.png)
## Example
![Screenshot 2024-09-18 at 22.17.13](Screenshot%202024-09-18%20at%2022.17.13.png)
![Screenshot 2024-09-18 at 22.17.29](Screenshot%202024-09-18%20at%2022.17.29.png)
# WHAT CAN'T YOU DO
![Screenshot 2024-09-18 at 22.27.17](Screenshot%202024-09-18%20at%2022.27.17.png)