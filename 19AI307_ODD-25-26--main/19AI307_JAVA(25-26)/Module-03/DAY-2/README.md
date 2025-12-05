# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator with:
area(int side) for square
area(int length, int breadth) for rectangle
area(double radius) for circle

## AIM:
To write a Java program that calculates the area of different shapes (square, rectangle, and circle) using method overloading by defining multiple area() methods with different parameter lists.

## ALGORITHM :
1. Create a class `AreaCalculator` with three overloaded static methods:
   - `area(int side)` for calculating the area of a square
   - `area(int length, int breadth)` for calculating the area of a rectangle
   - `area(double radius)` for calculating the area of a circle
2. In the `main` method:
   - Create a `Scanner` object to read input.
   - Read the side of a square and call `area(side)`.
   - Read the length and breadth of a rectangle and call `area(length, breadth)`.
   - Read the radius of a circle and call `area(radius)`.
3. Each overloaded method computes and returns the area of the corresponding shape.
4. Display the result for each shape.
5. End the program.

## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: PRIYAADARSHINI K
RegisterNumber:  212223240126
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class AreaCalculator {
    public static int area(int side) {
        return side * side;
    }

    public static int area(int length, int breadth) {
        return length * breadth;
    }

    public static double area(double radius) {
        return Math.PI * radius * radius;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        int side = sc.nextInt();
        System.out.println("Area of square: " + area(side));

        int l = sc.nextInt();
        int b = sc.nextInt();
        System.out.println("Area of rectangle: " + area(l, b));

        double r = sc.nextDouble();
        System.out.println("Area of circle: " + area(r));
    }
}

```
## OUTPUT:
<img width="823" height="457" alt="Screenshot 2025-11-28 135313" src="https://github.com/user-attachments/assets/e27e7cf8-f24d-42b8-8796-fb613806d192" />

## RESULT:
The program successfully calculated and displayed the areas of a square, rectangle, and circle using method overloading.

