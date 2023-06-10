Aim:

To write a Java program to create a method to calculate power of a number raised to other.

Algorithm

Step 1 : Open Intelli J application or any other code editor.

Step 2 : Create a class called "Power" and create a method.

Step 3 : Create a main class,called the "Solution".

Step 4 : Calll the method from the Power class in Solution.

Step 5 : Display the result using Solution Class in the terminal.

Program
```
import java.util.Scanner;
class Power {
public static void main(String[] args) {
int base , powerRaised;
Scanner s =new Scanner(System.in);
System.out.println("Enter the Base value:");
base=s.nextInt();
System.out.println("Enter the value of power:");
powerRaised=s.nextInt();
int result = power(base, powerRaised);
System.out.println(base + "^" + powerRaised + "=" + result);
}
public static int power(int base, int powerRaised) {
if (powerRaised != 0) {
// recursive call to power()
return (base * power(base, powerRaised - 1));
}
else {
return 1;
}
}
}
```
Output

<img width="245" alt="power" src="https://github.com/mehanthyka/power-of-number/assets/127507580/c0172465-777d-4160-a0fb-4c2977c7c92c">


Result

We have successfully created a Java program to calculate power of a number raised to other using method
