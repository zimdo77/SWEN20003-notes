# Enumerated types
![Screenshot 2024-10-23 at 17.19.28](Screenshot%202024-10-23%20at%2017.19.28.png)![Screenshot 2024-10-23 at 17.18.54](Screenshot%202024-10-23%20at%2017.18.54.png)
![Screenshot 2024-10-23 at 17.19.57](Screenshot%202024-10-23%20at%2017.19.57.png)![Screenshot 2024-10-23 at 17.20.33](Screenshot%202024-10-23%20at%2017.20.33.png)![Screenshot 2024-10-23 at 17.20.56](Screenshot%202024-10-23%20at%2017.20.56.png)![Screenshot 2024-10-23 at 17.21.29](Screenshot%202024-10-23%20at%2017.21.29.png)
![Screenshot 2024-10-23 at 17.21.49](Screenshot%202024-10-23%20at%2017.21.49.png)
NOTE: when sorting the `ranks` list, it is put in order of how it was declared in the enum class

![Screenshot 2024-10-23 at 17.22.05](Screenshot%202024-10-23%20at%2017.22.05.png)
# Variadic parameters (Varargs)
![Screenshot 2024-10-24 at 00.08.04](Screenshot%202024-10-24%20at%2000.08.04.png)
## how do they work
Essentially the method's argument has the form `datatype... args` where all the input arguments are converted to an array `args` of data type `datatype`.
## example 1: concatenate method
![Screenshot 2024-10-24 at 00.14.49](Screenshot%202024-10-24%20at%2000.14.49.png)
## example 2: average method
![Screenshot 2024-10-24 at 00.15.07](Screenshot%202024-10-24%20at%2000.15.07.png)
## The main method can be treated as a variadic method if we use `...` instead of `[]`.
```java
public class VariadicExample {
	public static void main (String... args) {
		// Enter code here
	}
}
```
# Functional interfaces
![Screenshot 2024-10-24 at 11.50.40](Screenshot%202024-10-24%20at%2011.50.40.png)
Their main uses are for **LAMBDA EXPRESSIONS** or **METHOD REFERENCES**, but they can also be useful on their own because define a clear contract with a single abstract method:
- callback mechanism in event-driven programming: a single action to perform upon an event.
- strategy patterns: implement strategies that can be swapped easily
- stream API

![Screenshot 2024-10-24 at 11.55.31](Screenshot%202024-10-24%20at%2011.55.31.png)

![Screenshot 2024-10-24 at 11.56.02](Screenshot%202024-10-24%20at%2011.56.02.png)
# Lambda expressions (instances of functional interfaces)
![Screenshot 2024-10-24 at 16.14.42](Screenshot%202024-10-24%20at%2016.14.42.png)
![Screenshot 2024-10-24 at 16.34.39](Screenshot%202024-10-24%20at%2016.34.39.png)

![Screenshot 2024-10-24 at 16.15.13](Screenshot%202024-10-24%20at%2016.15.13.png)
NOTE: `p` is used as an object that implements `Predicate<Integer>`, so that's why `p.test()` can be called.

![Screenshot 2024-10-24 at 16.15.33](Screenshot%202024-10-24%20at%2016.15.33.png)
NOTE: `u1` and `u2` are used as objects that implement `Unary<Integer>`, so that's why `u1.apply()` and `u2.apply()` can be called.
## lambda expressions: combining predicates
![Screenshot 2024-10-24 at 16.39.18](Screenshot%202024-10-24%20at%2016.39.18.png)
## lambda expressions: another example
![Screenshot 2024-10-24 at 16.40.18](Screenshot%202024-10-24%20at%2016.40.18.png)
![Screenshot 2024-10-24 at 16.40.43](Screenshot%202024-10-24%20at%2016.40.43.png)
# Anonymous classes vs lambdas
![Screenshot 2024-10-24 at 17.29.48](Screenshot%202024-10-24%20at%2017.29.48.png)
# Method references
![Screenshot 2024-10-25 at 11.17.21](Screenshot%202024-10-25%20at%2011.17.21.png)

![Screenshot 2024-10-25 at 11.18.17](Screenshot%202024-10-25%20at%2011.18.17.png)
## method references example
![Screenshot 2024-10-25 at 11.19.23](Screenshot%202024-10-25%20at%2011.19.23.png)
![Screenshot 2024-10-25 at 11.19.56](Screenshot%202024-10-25%20at%2011.19.56.png)
# Streams
![Screenshot 2024-10-25 at 13.02.32](Screenshot%202024-10-25%20at%2013.02.32.png)
![Screenshot 2024-10-25 at 13.04.22](Screenshot%202024-10-25%20at%2013.04.22.png)

## streams example 1
Write a function that takes a list of Strings, and returns a list that only contains the Strings with at lease 5 characters, starting with "C". And all the elements in the new list should all be in upper case.

Without streams:

![Screenshot 2024-10-25 at 13.05.02](Screenshot%202024-10-25%20at%2013.05.02.png)

With streams:

![Screenshot 2024-10-25 at 13.06.00](Screenshot%202024-10-25%20at%2013.06.00.png)
NOTE: remember to `collect` at the end
## streams example 2
Implement a stream pipeline that takes a list of People, and generates a String consisting of a comma separated list. The list should contain the names (in upper case) of all the people who are between the ages of 18 and 40.
![Screenshot 2024-10-25 at 13.07.49](Screenshot%202024-10-25%20at%2013.07.49.png)

 
