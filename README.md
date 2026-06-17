# A-university-wants-a-system-to-store-student-information-and-display-admission-details.
// Student class
class Student {
    // Attributes
    private String name;
    private int rollNumber;
    private String faculty;

    // Constructor for initialization
    public Student(String name, int rollNumber, String faculty) {
        this.name = name;
        this.rollNumber = rollNumber;
        this.faculty = faculty;
    }

    // Getters
    public String getName() {
        return name;
    }

    public int getRollNumber() {
        return rollNumber;
    }

    public String getFaculty() {
        return faculty;
    }

    // Setters
    public void setName(String name) {
        this.name = name;
    }

    public void setRollNumber(int rollNumber) {
        this.rollNumber = rollNumber;
    }

    public void setFaculty(String faculty) {
        this.faculty = faculty;
    }

    // Method to display student profile
    public void displayProfile() {
        System.out.println("----- Student Profile -----");
        System.out.println("Name: " + name);
        System.out.println("Roll Number: " + rollNumber);
        System.out.println("Faculty: " + faculty);
    }
}

// Main class
public class UniversitySystem {
    public static void main(String[] args) {
        // Creating student object
        Student student1 = new Student("Nabin", 101, "Computer Science");

        // Displaying profile
        student1.displayProfile();

        // Updating details using setters
        student1.setFaculty("Information Technology");

        // Display updated profile
        student1.displayProfile();
    }
}
