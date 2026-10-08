class StudentMessage implements Runnable {
    public void run() {
        for (int i = 1; i <= 3; i++) {
            System.out.println("Hello Student");
        }
    }
}

public class Program10_RunnableInterface {
    public static void main(String[] args) throws InterruptedException {
        Thread t = new Thread(new StudentMessage());
        t.start();
        t.join();

        System.out.println("Main thread completed.");
    }
}
