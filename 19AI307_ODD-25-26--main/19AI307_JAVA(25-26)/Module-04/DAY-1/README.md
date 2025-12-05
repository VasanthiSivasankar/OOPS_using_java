# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
If an Integer object is set to null, and you attempt to call .toString() on it, what happens? How can you prevent your code from throwing an exception in such cases?

## AIM:
To write a Java program that demonstrates how a NullPointerException occurs when accessing methods on a null Integer object, and how to handle it using a try–catch block.

## ALGORITHM :
1. Start the program.
2. Create a Scanner object to read an integer input from the user.
3. Read an integer value input.
4. If the input is 0, assign null to the Integer object num; otherwise assign the input value.
5. Use a try block to call num.toString():
   - If num is not null, print its string representation.
   - If num is null, a NullPointerException will be thrown.
6. Catch the NullPointerException and print "Null Integer".
7. Close the scanner.
8. End the program.
   
## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: VASANTHI SIVASANKAR
RegisterNumber:  212223040234
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class NullPointerIntegerExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int input = sc.nextInt();
        Integer num = (input == 0) ? null : input;

        try {
            System.out.println(num.toString());
        } catch (NullPointerException e) {
            System.out.println("Null Integer");
        }

        sc.close();
    }
}
```

## OUTPUT:
<img width="506" height="373" alt="image" src="https://github.com/user-attachments/assets/f3dbb9dc-69e8-479b-b56a-5cf7833f724c" />

## RESULT:
The program successfully demonstrates how invoking a method on a null `Integer` object triggers a `NullPointerException`, and shows how the exception can be caught and handled gracefully by printing `"Null Integer"`.
