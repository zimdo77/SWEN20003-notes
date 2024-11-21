# Reminder: Abstract classes
![[Screenshot 2024-09-04 at 22.36.02.png]]
# Interfaces
Interfaces represent a  "Can do" relationship. Interface names are usually called <...>able.
![[Screenshot 2024-09-04 at 22.36.58.png]]
# Defining interfaces
![[Screenshot 2024-09-04 at 22.39.27.png]]
# Implementing interfaces
![[Screenshot 2024-09-04 at 22.40.09.png]]
# Default methods
![[Screenshot 2024-09-04 at 22.46.29.png]]
This is to ensure that when a new method is added to the interface, all the classes that implement this interface won't "break down".
# Example
![[Screenshot 2024-09-04 at 22.48.22.png]]
![[Screenshot 2024-09-04 at 22.48.34.png]]
# Extending interfaces
![[Screenshot 2024-09-04 at 22.48.56.png]]
# Sorting
How can classes have sorting methods? i.e., String.sort() or Array.sort()
They implement the Comparable interface:
![[Screenshot 2024-09-04 at 22.51.34.png]]
## Comparable interface: use `compareTo()` method
![[Screenshot 2024-09-04 at 22.51.54.png]]
![[Screenshot 2024-09-04 at 22.53.02.png]]
# Next level abstraction (extends AND implements)
- Classes can only inherit one class, but can implement multiple interfaces
- Interfaces can extend a parent class
# Polymorphism
![[Screenshot 2024-09-04 at 22.57.10.png]]
Essentially, you can instantiate an object and have its reference as the interface that its class implements.
# Interface vs Inheritance
![[Screenshot 2024-09-04 at 23.00.15.png]]


