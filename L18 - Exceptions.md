	# Types of errors
- Syntax: not legal code - identified by compiler
- Semantic: code runs but there is a logical error - identified through software testing
- Runtime: program crashes prematurely (e.g. array index out of bounds, perform operations on wrong data types) - identified through execution
# Preventing runtime errors
## Method 1: Defensive programming
Explicitly guard against invalid conditions![[Screenshot 2024-10-20 at 23.33.26.png]]
This is not ideal because:
- have to think of every edge case
- not good for long term (not scalable)
- poor abstraction
- not nice to read
## Method 2: Exceptions
Exceptions are error states caused by runtime error. 'Exceptions' is also a class to represent error objects.
![[Screenshot 2024-10-20 at 23.36.05.png]]
![[Screenshot 2024-10-20 at 23.37.05.png]]

NOTE: 'finally' should be used to close files that don't need to be open for example
# Chaining exceptions
![[Screenshot 2024-10-20 at 23.39.20.png]]

NOTE: Don't catch the super super class "Exception" - not ideal. If you have to, write something like "Something went wrong". But ideal to catch the specific exceptions
# Example
![[Screenshot 2024-10-20 at 23.46.24.png]]
# Generating exceptions (throw, throws)
![[Screenshot 2024-10-20 at 23.46.43.png]]
![[Screenshot 2024-10-21 at 10.28.32.png]]
# Custom/user-defined exceptions
![[Screenshot 2024-10-21 at 10.29.19.png]]
![[Screenshot 2024-10-21 at 10.29.30.png]]
![[Screenshot 2024-10-21 at 10.29.41.png]]
![[Screenshot 2024-10-21 at 13.23.50.png]]
NOTE: Be wary of catching `Exception` class.
# Checked vs Unchecked exception
![[Screenshot 2024-10-21 at 13.26.53.png]]![[Screenshot 2024-10-21 at 13.27.04.png]]
# Try With
![[Screenshot 2024-10-21 at 13.52.42.png]]
By doing try with (e.g. declaring `reader` as an argument in line 2), the `finally` block can access reader. If reader was declared within the `try` block, the `finally` block won't be able to access it. Or just declare reader before the `try` block.