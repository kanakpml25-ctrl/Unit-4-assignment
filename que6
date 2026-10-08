import java.util.Scanner;

public class Program06_ThrowValidMarks {
    static void checkMarks(int marks) {
        try {
            if (marks < 0 || marks > 100) {
                throw new IllegalArgumentException();
            }
            System.out.println("Valid marks.");
        } catch (IllegalArgumentException e) {
            System.out.println("Invalid marks.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Marks = ");
        int marks = sc.nextInt();
        checkMarks(marks);
    }
}
