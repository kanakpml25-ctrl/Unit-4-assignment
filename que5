import java.util.Scanner;

public class Program05_ThrowVotingEligibility {
    static void checkAge(int age) {
        try {
            if (age < 18) {
                throw new ArithmeticException();
            }
            System.out.println("Eligible to vote.");
        } catch (ArithmeticException e) {
            System.out.println("Not eligible to vote.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Age = ");
        int age = sc.nextInt();
        checkAge(age);
    }
}
