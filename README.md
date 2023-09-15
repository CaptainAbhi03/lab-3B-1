import java.util.Scanner;

public class ElementSearch {
    public static void main(String[] args) {
        // Create an array of size 10
        int[] array = new int[10];

        // Get input from the user to fill the array
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter 10 integers to fill the array:");
        for (int i = 0; i < 10; i++) {
            System.out.print("Enter number at index " + i + ": ");
            numbers[i] = scanner.nextInt();
        }

        // Get the element to search for from the user
        System.out.print("Enter the element to search for: ");
        int number = scanner.nextInt();

        // Perform the search and display the result
        int foundIndex = -1;
        for (int i = 0; i < numbers.length; i++) {
            if (numbers[i] == target) {
                foundIndex = i;
                break;
            }
        }

        if (foundIndex != -1) {
            System.out.println("Element " + target + " found at index " + foundIndex);
        } else {
            System.out.println("Element " + target + " not found in the array.");
        }
    }
}
