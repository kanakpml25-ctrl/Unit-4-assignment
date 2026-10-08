class PriorityTask extends Thread {
    public PriorityTask(String name) {
        super(name);
    }

    public void run() {
        System.out.println(getName() + " = " + getPriority());
    }
}

public class Program18_ThreadPriority {
    public static void main(String[] args) throws InterruptedException {
        PriorityTask low = new PriorityTask("LowPriority");
        PriorityTask high = new PriorityTask("HighPriority");

        low.setPriority(3);
        high.setPriority(8);

        low.start();
        low.join();

        high.start();
        high.join();

        System.out.println("Both threads completed.");
    }
}
