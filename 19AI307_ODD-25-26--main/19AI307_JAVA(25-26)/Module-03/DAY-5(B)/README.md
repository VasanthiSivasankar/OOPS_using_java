# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to find the square root of a number using Double wrapper class.

## AIM:
To write a Java program that reads a number in string format, converts it into a double, and prints its square root using the `Math.sqrt()` function.

## ALGORITHM :
1. Start the program.
2. Create a `Scanner` object to read input from the user.
3. Read a string value representing a number.
4. Convert the string to a `Double` using `Double.parseDouble()`.
5. Use `Math.sqrt()` to compute the square root of the number.
6. Display the result in the required format.
7. End the program.

## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: VASANTHI SIVASANKAR
RegisterNumber:  212223040234
*/
```

## SOURCE CODE:
```
import java.util.*;

public class Main
{
    public static void main(String[] args)
    {
        Scanner s = new Scanner(System.in);
        String str = s.next();
        
        Double num = Double.parseDouble(str);
        System.out.println("Square root of "+num+" is: "+(Math.sqrt(num)));
    }
}
```

## OUTPUT:
<img width="708" height="332" alt="image" src="https://github.com/user-attachments/assets/896a9f26-bd3e-4436-9f6d-09e46af83956" />

## RESULT:
The program successfully reads a numeric string, converts it to a double value, computes its square root, and displays the result.
