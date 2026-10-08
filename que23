class Message {
    String message;

    synchronized void getMessage() throws InterruptedException {
        while (message == null) {
            System.out.println("Waiting for message...");
            wait();
        }
        System.out.println("Message received: " + message);
    }

    synchronized void setMessage(String message) {
        this.message = message;
        notify();
    }
}

class Receiver extends Thread {
    Message msg;

    Receiver(Message msg) {
        this.msg = msg;
    }

    public void run() {
        try {
            msg.getMessage();
        } catch (InterruptedException e) {
            System.out.println("Thread interrupted.");
        }
    }
}

class Sender extends Thread {
    Message msg;

    Sender(Message msg) {
        this.msg = msg;
    }

    public void run() {
        msg.setMessage("Hello Student");
    }
}

public class Program23_WaitNotify {
    public static void main(String[] args) throws InterruptedException {
        Message msg = new Message();

        Receiver receiver = new Receiver(msg);
        Sender sender = new Sender(msg);

        receiver.start();
        Thread.sleep(100);
        sender.start();

        receiver.join();
        sender.join();
    }
}
