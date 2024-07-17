// Define the Person class
class Person {
    private String name;
    private int age;
    private String address;

    // Constructor with three parameters
    public Person(String name, int age, String address) {
        this.name = name;
        this.age = age;
        this.address = address;
    }

    // Method to display the person's details
    public void displayDetails() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Address: " + address);
    }

    // Method that accepts a Person object and calls the displayDetails method
    public void myDetails(Person person) {
        person.displayDetails();
    }

    // Method to print the current instance
    public void printCurrentInstance() {
        myDetails(this);
    }

    public static void main(String[] args) {
        // Create an object of the Person class
        Person person = new Person("Your Name", 30, "Your Address");

        // Call the printCurrentInstance method using the object
        person.printCurrentInstance();
    }
}
