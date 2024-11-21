- Introducing Java Packages
- Information Hiding
- Delegation through Association
- Wrapper Classes
# Java packages
- Classes and interfaces grouped together
- Allows reuse - can import into programs/classes
- Prevents naming conflicts
- Allows **access control**
- Another level of **encapsulation** - higher level than defining a class
## Creating packages
![Screenshot 2024-08-05 at 09.22.46](attachments/Screenshot%202024-08-05%20at%2009.22.46.png)
## Using packages
![Screenshot 2024-08-05 at 09.23.28](attachments/Screenshot%202024-08-05%20at%2009.23.28.png)
## The default package
![Screenshot 2024-08-05 at 09.28.22](attachments/Screenshot%202024-08-05%20at%2009.28.22.png)
# Information hiding
- The OO design paradigm allows information related to classes/objects (i.e. attributes and methods) to be grouped together - **Encapsulation** - [](L3%20-%20Classes%20and%20Objects%201.md#OO%20features)
- Actions on objects can be performed through methods of the class - **interface** to the class
- The OO design paradigm also supports **Information Hiding**, where some attributes and methods are hidden from the user.
- Information Hiding is aka **Visibility Control**.

- **Information Hiding**: ability to 'hide' the details of a class from the outside world
- **Access Control**: preventing an outside class from manipulation the properties of another class in undesired ways
## Visibility modifiers
![Screenshot 2024-08-05 at 09.35.04](attachments/Screenshot%202024-08-05%20at%2009.35.04.png)
![Screenshot 2024-08-05 at 09.35.19](attachments/Screenshot%202024-08-05%20at%2009.35.19.png)
### The `Circle` class with visibility modifiers
![Screenshot 2024-08-05 at 09.36.23](attachments/Screenshot%202024-08-05%20at%2009.36.23.png)
## Information hiding (cont.)
By using why **visibility modifiers** to control **visibility/access** of variables and methods:
- Data is safely sealed within the capsule of the class
- Prevents programmers from relying on details of class implementation
- Prevents accidental or wrong usage
- Keeps code elegant and clean - easier to maintain
- Enables to provide access to the object through a clean interface
## Mutability
- A **mutable class** is a class containing public mutator methods that change instance variables. Its objects are called **mutable objects**.
- An **immutable class** is a class that contains no methods (other than constructors) that change ANY instance variables. Its objects are called **immutable objects**.
### Example: the `Circle` class
- Mutable:
![Screenshot 2024-08-05 at 13.50.03](attachments/Screenshot%202024-08-05%20at%2013.50.03.png)
- Immutable:
![Screenshot 2024-08-05 at 13.50.43](attachments/Screenshot%202024-08-05%20at%2013.50.43.png)
**REMOVE 'SET' METHODS AND 'RESIZE' METHOD**
# Delegation through association
- A class can **delegate** its responsibilities to other classes.
- An object can **invoke methods** in other objects through **containership**.
- This relationship between classes is called **Association**

## Example: the `Circle` class
The design of this class can be improved because `centreX` and `centreY` are not specific to circles, but many other shapes too. So **encapsulation** can be improved.
![Screenshot 2024-08-05 at 13.58.42](attachments/Screenshot%202024-08-05%20at%2013.58.42.png)
So, create a `Point` class:
![Screenshot 2024-08-05 at 14.04.41](attachments/Screenshot%202024-08-05%20at%2014.04.41.png)
And use it within the `Circle` class:
![Screenshot 2024-08-05 at 14.05.41](attachments/Screenshot%202024-08-05%20at%2014.05.41.png)
# Wrapper classes
- Primitive data types like `int` and `double` only contain data, and they don't have attributes and methods (e.g. `parseInt()`)
- Java provides **wrapper classes** for primitives - allowing them to be "packaged"/"boxed" into objects and "pretend" that they are classes.

**Wrapper classes**: A class that gives extra functionality to primitives like `int`, and lets them behave like objects
![center|300](attachments/Screenshot%202024-08-05%20at%2014.14.45.png)
For example, the `Integer` class has methods like:
- Reverse: `Integer.reverse(10);`
- Rotate left: `Integer.rotateLeft(10, 2);`
- Signum: `Integer.signum(-10);`
- **Parsing**: `Integer.parseInt("10");`
## Parsing
**Parsing** is processing one data type into another. Every wrapper class has a parse function:
- `int i = Integer.parseInt("1");`
- `double d = Double.parseDouble("1");`
- `boolean b = Boolean.parseBoolean("TruE");`
## Automatic boxing/unboxing
- **Boxing/unboxing** is the processing of converting a primitive to/from its equivalent wrapper.
- This is done automatically through typecasting `(int)` or `(Integer)`
![center|300](attachments/Screenshot%202024-08-05%20at%2014.23.40.png)












