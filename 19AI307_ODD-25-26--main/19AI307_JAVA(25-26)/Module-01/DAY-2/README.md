# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A pirate ship has a code lock that only opens if:
     The input code is even, and 
     If it is less than 100, say "Weak Code".
     If it is between 100 and 999, say "Strong Code".
     If the code is odd, deny access.

## AIM:
To write a Java program that accepts a code number and determines the security level based on the given conditions:
- If the code is even and less than 100 → Display "Weak Code"
- If the code is even and between 100 and 999 → Display "Strong Code"
- Otherwise → Display "Access Denied"

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read an integer value num from the user.
4.	Check if num is even (num % 2 == 0):
            If yes:         
            If num < 100, display "Weak Code".           
            Else if num is between 100 and 999, display "Strong Code".          
            Else, display "Access Denied".          
            If no, display "Access Denied".
5. End.


## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: PRIYAADARSHINI K
RegisterNumber:  212223240126
*/
```

## SOURCE CODE:
```
import java.util.*;
class prog{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        if(num%2==0){
            if(num<100){
                System.out.println("Weak Code");
            }
            else if(num>=100 && num<999){
                System.out.println("Strong Code");
            }
            else{
                System.out.println("Access Denied");
            }
        }
        else{
            System.out.println("Access Denied");
        }
    }
}
```


## OUTPUT:

<img width="444" height="356" alt="Screenshot 2025-11-28 100314" src="https://github.com/user-attachments/assets/3f648a86-5b5c-468c-a6be-5af5efcd00a3" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.

