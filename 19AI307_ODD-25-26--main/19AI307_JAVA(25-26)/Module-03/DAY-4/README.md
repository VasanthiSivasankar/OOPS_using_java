# Ex.No:3(D)    INTERFACE 

## QUESTION:
Two types of traffic controllers decide whether a vehicle can pass based on signal color. The decision logic varies by controller.
AggressiveController: Allows only if "GREEN".
DefensiveController: Allows for "GREEN" or "YELLOW".

## AIM:
To develop a Java program that decides whether a vehicle can move or must stop based on the signal color and the type of traffic controller (Aggressive or Defensive) using interfaces.

## ALGORITHM :
1. Define an interface `TrafficController` with the method:
   - `boolean canGo(String signalColor)`
2. Create class `AggressiveController` implementing the interface:
   - Allows passage only if the signal color is GREEN.
3. Create class `DefensiveController` implementing the interface:
   - Allows passage if the signal color is GREEN or YELLOW.
4. In the `main` method:
   - Read `color` (signal color)
   - Read `type` (controller type: 1 or 2)
5. Based on `type`:
   - If 1 → create `AggressiveController`
   - Else → create `DefensiveController`
6. Call `canGo(color)` to check permission.
7. If true → print `"GO"`
   - Else → print `"STOP"`
8. End the program.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: PRIYAADARSHINI K
RegisterNumber:  212223240126
*/
```

## SOURCE CODE:
```
import java.util.*;
interface controller
{
    String show(String signalColor);
}
class AggressiveController implements controller
{
    public String show(String signalColor)
    {
        if(signalColor.equals("GREEN"))
        {
            return "GO";
        }
        else
        {
            return "STOP";
        }
    }
}
class DefensiveController implements controller
{
    public String show(String signalColor)
    {
        if(signalColor.equals("GREEN")||signalColor.equals("YELLOW"))
        {
            return "GO";
        }
        else
        {
            return "STOP";
        }
    }
}
public class prog
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        String signalColor=sc.next();
        int type=sc.nextInt();
        controller c;
        if(type==1)
        {
            c=new AggressiveController();
        }
        else
        {
            c=new DefensiveController();
        }
        System.out.println(c.show(signalColor));
    }
}
```

## OUTPUT:
<img width="416" height="295" alt="image" src="https://github.com/user-attachments/assets/4bbe9bd0-68b0-45ee-82fc-93f44340368c" />

## RESULT:
The program successfully determines whether a vehicle can move based on the signal color and controller type using interface-based polymorphism.
