class LifeCycleThread extends Thread {
    public void run() {
        System.out.println("Thread is running.");
    }
}

public class Program16_ThreadLifeCycle {
    public static void main(String[] args) throws InterruptedException {
        System.out.println("Thread is starting.");

        LifeCycleThread t = new LifeCycleThread();
        t.start();
        t.join();

        System.out.println("Thread has completed.");
    }
}
