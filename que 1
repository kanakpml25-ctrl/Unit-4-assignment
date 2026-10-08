import java.util.Scanner;

public class DivisionException {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("First number = ");
        int numerator = sc.nextInt();

        System.out.print("Second number = ");
        int denominator = sc.nextInt();

        try {
            int result = numerator / denominator;
            System.out.println("Result = " + result);
        } catch (ArithmeticException e) {
            System.out.println("Cannot divide by zero.");
        }

        sc.close();
    }
}