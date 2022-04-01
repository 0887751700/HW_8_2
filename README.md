# HW_8_2
import static java.lang.String.*;

public class Exam_8_2 {
    public static void main (String[]args) {
Scanner scanner = new Scanner(System.in);
System.out.println("Enter number 1:");
System.out.println("Enter number 2:");
       float num1 = scanner.nextFloat();
       float num2 = scanner.nextFloat();
       float result = Math.abs(num1 - num2);

        System.out.printf("The result is:" + "%.4f", result);
        boolean theDifferenceIsUpTo1 = result < 0.01;
        boolean theDifferenceIsUpTo2 = result < 0.001;
        boolean theDifferenceIsUpTo3 = result < 0.0001;
        boolean theDifferenceIsUpTo4 = result < 0.00001;

        if (theDifferenceIsUpTo1) {
            System.out.println("\n The numbers are the same until the first decimal place.");
        } if (theDifferenceIsUpTo2) {
            System.out.println("\n The numbers are the same until the second decimal place.");
        } if (theDifferenceIsUpTo3) {
            System.out.println("\n The numbers are the same until the third decimal place.");
        } if (theDifferenceIsUpTo4) {
            System.out.println("\n The numbers are the same until the fourth decimal place.");
        } else {
            System.out.println("\n The numbers is different.");

        }
     }
    }
    Enter number 1:
Enter number 2:
25,1111
25,1110
The result is:0,0001
 The numbers are the same until the first decimal place.

 The numbers are the same until the second decimal place.

 The numbers are the same until the third decimal place.

 The numbers is different.

Process finished with exit code 0
