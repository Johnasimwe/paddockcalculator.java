import java.util.Scanner; // Importing the Scanner class from the java.util package to read user input

public class PaddockCalculator {

    // Method to calculate the area of a paddock
    public static int calculatePaddockArea(int length, int width) {
        return length * width;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Requesting user input for length and width of the paddocks
        System.out.print("Enter the length of the paddock: ");
        int length = scanner.nextInt();

        System.out.print("Enter the width of the paddock: ");
        int width = scanner.nextInt();

        // Calculating the area of one paddock
        int paddockArea = calculatePaddockArea(length, width);

        // Calculating the total area needed for 100 paddocks
        int totalArea = paddockArea * 100;

        // Printing the results
        System.out.println("The area of each paddock is: " + paddockArea + " square units.");
        System.out.println("The total area needed for 100 paddocks is: " + totalArea + " square units.");

        scanner.close();
    }
}
