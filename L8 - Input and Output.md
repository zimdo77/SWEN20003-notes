# Input: Command line arguments
Definition: data provided to a program when it is executed - acessible through the `args` variable:
``` java
public static void main(String[] args)
```
- `args` is an array of Strings that store command line arguments.
- For multiword Strings, remember to use quotes.
- Access args by indexing, e.g. `System.out.println(args[2]);`
# Input: Scanner

Import library
``` java
import java.util.Scanner
```

Only create 1 Scanner per program.
System.in is an object representing the standard input stream i.e command line/terminal.
```java
Scanner scanner = new Scanner(System.in);       
```

Scanner methods:

- read a single line of text until a "return" or newline character (\\n)
```java
String s = scanner.nextLine();
```

- read a single value that matches the method name (`boolean`, `int`, etc.)
```java
boolean b = scanner.nextBoolean();
int i = scanner.nextInt();
double d = scanner.nextDouble()
```

- return `true` if there is input to be read
```java
scanner.hasNext();
```

- return `true` if the next "token" matches XXX
```java
scanner.hasNextXXX();
```
# Input: Reading files 
## Reading files using BufferedReader
 ![[Screenshot 2024-08-18 at 22.28.16.png]]
 ![[Screenshot 2024-08-18 at 22.28.39.png]]
 ![[Screenshot 2024-08-18 at 22.29.15.png]]
 ![[Screenshot 2024-08-18 at 22.29.24.png]]
 ![[Screenshot 2024-08-18 at 22.29.37.png]]
## Reading files using Scanner
![[Screenshot 2024-08-18 at 22.31.55.png]]
## Reading files: BufferedReader vs Scanner
- BufferedReader is more efficient than Scanner. 
- Scanner is preferable for smaller files.
- Scanner can parse text as well as read it.
# Output: Writing files
![[Screenshot 2024-08-18 at 22.45.13.png]]
![[Screenshot 2024-08-18 at 22.45.51.png]]
![[Screenshot 2024-08-18 at 22.46.08.png]]
![[Screenshot 2024-08-18 at 22.46.24.png]]
![[Screenshot 2024-08-18 at 22.46.36.png]]