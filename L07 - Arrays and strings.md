# Arrays
Definition: A sequence of elements of the same type arranged in order in memory
## Array declaration
![Screenshot 2024-08-12 at 20.07.41](attachments/Screenshot%202024-08-12%20at%2020.07.41.png)
## Array initialisation and assignment
Many ways to initialise
![Screenshot 2024-08-12 at 20.11.53](attachments/Screenshot%202024-08-12%20at%2020.11.53.png)
In the third block, both `intArray_1` and `intArray_2` are references to the same array
## Multidimensional arrays
![Screenshot 2024-08-12 at 20.16.53](attachments/Screenshot%202024-08-12%20at%2020.16.53.png)
## Arrays of objects
![Screenshot 2024-08-12 at 20.18.07](attachments/Screenshot%202024-08-12%20at%2020.18.07.png)
![Screenshot 2024-08-12 at 20.18.55](attachments/Screenshot%202024-08-12%20at%2020.18.55.png)
## Array methods
- Indexing
```
int[] intArray = new int[10];
int x = intArray[NUMBER];                     // NUMBER is anything from 0 to 9
```
- Length
```
int len = intArray.length;                    // length is an attribute
```
- Equality
```
import java.util.Arrays;

int[] n1 = {3, 1, 2};
int[] n2 = {3, 1, 2};

println(Arrays.equals(n1, n2));               // outputs true
```
- Resizing (arrays are fixed length; resizing creates a new array)
```
int[] intArray = new int[5];
intArray = new int[intArray.length + 3];
```
- Sorting (ascending)
```
Arrays.sort(n1);
```
- Printing
```
System.out.println(Arrays.toString(n1));
```
OUTPUT: `[3, 1, 2]`
## For each loop (for loop in Python)
![Screenshot 2024-08-12 at 20.27.44](attachments/Screenshot%202024-08-12%20at%2020.27.44.png)
# Strings
Is a class and data type made up of a sequence of characters
## String methods
- Length: `s.length()`
- Upper (or lower) case: `s.toUpperCase()`
- Split: `s.split(" ")`
- Check substring presence: `s.contains("Hell")`
- Find substring location: `s.indexOf("Hell")`
- Substring: `s.substring(2, 7)`
## Strings are immutable
Every String operation returns a new String, so remember to reassign. E.g. `s = s.toUpperCase()`
## Check for equality
![Screenshot 2024-08-14 at 00.11.00](attachments/Screenshot%202024-08-14%20at%2000.11.00.png)
