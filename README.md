import java.util.Scanner;

public class InputNumbers {
    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.print("Enter the number of elements: ");
            int n = scanner.nextInt();
            
            int[] numbers = new int[n];
            
            System.out.println("Enter the numbers:");
            
            for (int i = 0; i < n; i++) {
                numbers[i] = scanner.nextInt();
            }
            
            System.out.println("The input numbers are:");
            
            for (int i = 0; i < n; i++) {
                System.out.print(numbers[i] + " ");
            }
        }
    }
}
