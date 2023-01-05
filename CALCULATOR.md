
import java.util.*;
import java.lang.Math;
public class Calculator {
    public static void main(String[] args) {
        Scanner sc= new Scanner(System.in);                       //Input:----------------------------------------------
        int x = sc.nextInt();                                     //Declaration of input variables:
        int y = sc.nextInt();
        int operations = sc.nextInt();
        switch (operations) {                                     //Calling the operations using SWITCH statement-------
            case 1 -> System.out.println(x + y);                  //addition of the numbers-----------------------------
            case 2 -> System.out.println(x - y);                  //subtraction of the numbers--------------------------
            case 3 -> System.out.println(x * y);                  //multiplication of two numbers-----------------------
            case 4 -> {                                           //Division of two numbers-----------------------------
                if (y == 0) {
                    System.out.println("Not defined");            //Divide by ZERO
                } else {
                    System.out.println(x / y);
                }
            }
            case 5 -> {                                           //Find SIN of a given number
                double a = sc.nextDouble();
                double b = Math.toRadians(a);                     //Convert to Radians
                System.out.println(Math.sin(b));
            }
            default -> {                                          //Modulo: To find remainder post division-------------
                if (y == 0) {
                    System.out.println("Not Defined");
                } else {
                    System.out.println(x % y);
                }
            }
        }
    }
}
