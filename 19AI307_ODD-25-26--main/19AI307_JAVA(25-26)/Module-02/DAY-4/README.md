# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class that uses a constructor to initialize variables and overrides toString() method.

## AIM:
To write a Java program that initializes object variables using a constructor and overrides the toString() method to display object details in a readable format.

## ALGORITHM :
1. Define a class Student with two instance variables:
     String name
     int age
2. Create a parameterized constructor to initialize these variables.
3. Override the toString() method to return the student details in a formatted string.
4. In the main() method:
    - Read the name and age from the user.
    - Create a Student object using the constructor.
5. Print the object, which automatically calls the overridden toString() method.
6. End the program.

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: PRIYAADARSHINI K
RegisterNumber:  212223240126
*/
```

## SOURCE CODE:
```
import java.util.*;
class student{
    private String name;
    private int age;
    public student(String name,int age){ 
        this.name=name;
        this.age=age;
    }
    @Override
    public String toString(){
        return "Student{name='"+name+"', age="+age+"}";
    }
}
public class prog{
    public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
    String name = sc.nextLine();
    int age = sc.nextInt();
    student st = new student(name,age);
    System.out.print(st);
    }
}
```
## OUTPUT:

<img width="689" height="363" alt="Screenshot 2025-11-28 131414" src="https://github.com/user-attachments/assets/dc94cb30-7bc2-44b8-9c51-a4bde5d37272" />

## RESULT:
The program has been executed successfully and the desired output has been obtained.
