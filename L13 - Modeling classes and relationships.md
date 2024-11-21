Aim:
- Identify **classes** and **relationships**
- Represent classes and relationships in **UML**
- Develop simple **Class Diagrams**

![[Screenshot 2024-09-07 at 22.49.11.png]]
# Unified Modeling Language (UML)
UML is a graphical modeling language that can be used to represent object oriented analyisis, design and implementation.
# Classes in UML
 ![[Screenshot 2024-09-07 at 22.58.25.png]]
 ![[Screenshot 2024-09-07 at 22.58.39.png]]
 ![[Screenshot 2024-09-07 at 22.58.49.png]]
 ![[Screenshot 2024-09-07 at 22.59.02.png]]
# Class relationships in UML
4 common types of relationships:
- Association
- Generalisation (Inheritance)
- Realization (Interface)
- Dependency
## Association (delegation through association)
 - represents a **'has-a'** (containment) relationship between objects
 - allows objects to **delegate** tasks to other objects
 - shown by a **solid line**

E.g. Represent position of  the `GameObject` class using the `Position` class instead of coordinates using `int x, y;` or `double x, y;`

![[Screenshot 2024-09-07 at 23.09.31.png]]
### Properties of Association
#### Name and role
![[Screenshot 2024-09-07 at 23.21.29.png]]
#### Directionality
![[Screenshot 2024-09-07 at 23.23.00.png]]
#### Multiplicity
![[Screenshot 2024-09-07 at 23.23.51.png]]
![[Screenshot 2024-09-07 at 23.24.02.png]]
![[Screenshot 2024-09-07 at 23.24.24.png]]
#### Type: plain association (like above)
#### Type: self association
![[Screenshot 2024-09-07 at 23.25.38.png]]
#### Type: multiple associations
![[Screenshot 2024-09-07 at 23.26.00.png]]
#### Type: aggregation
![[Screenshot 2024-09-07 at 23.26.54.png]]
#### Type: composition
![[Screenshot 2024-09-07 at 23.28.29.png]]
## Generalisation (Inheritance)
 ![[Screenshot 2024-09-07 at 23.31.31.png]]

For abstract classes, italicise:
![[Screenshot 2024-09-07 at 23.32.11.png]]

An example...
![[Screenshot 2024-09-07 at 23.33.00.png]]
## Realization (Interface)

**NOTATION**: dotted line with empty arrow head

Say, from the example above:
- Only `Player` and `Enemy` can move
- `Guardian` and `Enemy` can attack each other
- `Enemy` can also attack `Player`
- Both `Character`s can also target the player

![[Screenshot 2024-09-07 at 23.35.10.png]]
## Dependency
![[Screenshot 2024-09-07 at 23.51.10.png]]
# Example...
![[Screenshot 2024-09-08 at 00.08.39.png]]
![[Screenshot 2024-09-08 at 00.08.49.png]]

