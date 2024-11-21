- Choose appropriate data structures storing, retrieving and manipulating objects (data)  
- Use the Java Collections Framework  
- Use the Java Maps Framework
# Collections and Maps
![Screenshot 2024-09-18 at 22.40.26](attachments/Screenshot%202024-09-18%20at%2022.40.26.png)
# `ArrayList` class
## `ArrayList` for storing
![Screenshot 2024-09-18 at 22.50.54](attachments/Screenshot%202024-09-18%20at%2022.50.54.png)![Screenshot 2024-09-18 at 22.51.03](attachments/Screenshot%202024-09-18%20at%2022.51.03.png)

To store different types of objects, assuming they inherit the same base class:
![Screenshot 2024-09-18 at 23.09.48](attachments/Screenshot%202024-09-18%20at%2023.09.48.png)![Screenshot 2024-09-18 at 23.10.09](attachments/Screenshot%202024-09-18%20at%2023.10.09.png)
NOTE: cannot do `shapes.add(new Shape())` if `Shape` is an abstract class
![Screenshot 2024-09-19 at 10.22.49](attachments/Screenshot%202024-09-19%20at%2010.22.49.png)
## `ArrayList` for sorting
### Simple case: use `Comparable` interface
![Screenshot 2024-09-19 at 10.23.24](attachments/Screenshot%202024-09-19%20at%2010.23.24.png)
![Screenshot 2024-09-19 at 10.23.35](attachments/Screenshot%202024-09-19%20at%2010.23.35.png)
**NOTE:** `Collections.sort(circles)` isn't required to be assigned to the circles ArrayList, because the method automatically does that.
![Screenshot 2024-09-19 at 10.24.47](attachments/Screenshot%202024-09-19%20at%2010.24.47.png)
### Multiple ways to sort objects: use `Comparator` interface
E.g. want to sort by name AND by rating - multiple options

First, create separate classes that implement `Comparator`
![Screenshot 2024-09-19 at 10.52.33](attachments/Screenshot%202024-09-19%20at%2010.52.33.png)
Then, do `Collections.sort(...)` with the respective Comparator classes as an argument.
NOTE: The first sort method (with only 1 parameter) on line 5 uses the `compareTo()` method of the `Comparable` interface, whereas the next two sort methods uses the `compare()` method of the `Comparator` interface.
![Screenshot 2024-09-19 at 10.53.29](attachments/Screenshot%202024-09-19%20at%2010.53.29.png)![Screenshot 2024-09-19 at 10.54.18](attachments/Screenshot%202024-09-19%20at%2010.54.18.png)
### `Comparable` vs `Comparator`
![Screenshot 2024-09-19 at 10.56.31](attachments/Screenshot%202024-09-19%20at%2010.56.31.png)
### A shortcut for having multiple ways to sort objects: Anonymous Inner Class
This way, we don't have to create a new class for each comparator
![Screenshot 2024-09-19 at 10.58.19](attachments/Screenshot%202024-09-19%20at%2010.58.19.png)
![Screenshot 2024-09-19 at 10.58.39](attachments/Screenshot%202024-09-19%20at%2010.58.39.png)
# Collections
![Screenshot 2024-09-19 at 11.02.49](attachments/Screenshot%202024-09-19%20at%2011.02.49.png)
## Hierarchy
![Screenshot 2024-09-19 at 11.00.06](attachments/Screenshot%202024-09-19%20at%2011.00.06.png)
## Common operations
![Screenshot 2024-09-19 at 11.01.32](attachments/Screenshot%202024-09-19%20at%2011.01.32.png)
## Most useful
![Screenshot 2024-09-19 at 11.02.01](attachments/Screenshot%202024-09-19%20at%2011.02.01.png)
# Maps
![Screenshot 2024-09-19 at 11.02.20](attachments/Screenshot%202024-09-19%20at%2011.02.20.png)
## Hierarchy
![Screenshot 2024-09-19 at 11.03.33](attachments/Screenshot%202024-09-19%20at%2011.03.33.png)
## Common operations
![Screenshot 2024-09-19 at 11.03.53](attachments/Screenshot%202024-09-19%20at%2011.03.53.png)
## Using `HashMap`

![Screenshot 2024-09-19 at 11.05.34](attachments/Screenshot%202024-09-19%20at%2011.05.34.png)
