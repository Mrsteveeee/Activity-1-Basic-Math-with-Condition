//Group 8
//Leader:
//Steve Santos
//Members:
//Charls David P. Agustin
//Michelle Nicolas 
//Chris Anne Magtibay

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double num1, num2;
        int choice;
        
        do {
           
            System.out.print("Enter the first number: ");
            num1 = scanner.nextDouble();
            
            
            System.out.print("Enter the second number: ");
            num2 = scanner.nextDouble();

                   

System.out.println("Sum: " + (num1 + num2));
        System.out.println("Difference: " + (num1 - num2));
        System.out.println("Product: " + (num1 * num2));
        
        if(num2 != 0)
        {
            System.out.println("Quotient: " + (num1 / num2));
        }
        else{
            System.out.println("Cannot Divide by 0");
        }
        System.out.println  ("if u dont sure, U can check it ");
            System.out.println("Select the operation:");
            System.out.println("1. Addition");
            System.out.println("2. Subtraction");
            System.out.println("3. Multiplication");
            System.out.println("4. Division");

           
            System.out.print("Enter your choice 1-4: ");
            choice = scanner.nextInt();

            
            while (choice < 1 || choice > 4) {
                System.out.println(" Please enter a number between 1 and 4.");
                System.out.print("Enter your choice again 1-4: ");
                choice = scanner.nextInt();
            }

            
            if (choice == 1) {
                double result = num1 + num2;
                System.out.println("The result of addition is: " + result);
            } else if (choice == 2) {
                double result = num1 - num2;
                System.out.println("The result of subtraction is: " + result);
            } else if (choice == 3) {
                double result = num1 * num2;
                System.out.println("The result of multiplication is: " + result);
            } else if (choice == 4) {
                if (num2 != 0) {
                    double result = num1 / num2;
                    System.out.println("The result of division is: " + result);
                } else {
                    System.out.println("Error");
                }
            }

           
            System.out.print("Do you want to perform another operation? (Y/N): ");
            String continueChoice = scanner.next();
            
           
            while (!continueChoice.equalsIgnoreCase("Y") && !continueChoice.equalsIgnoreCase("N")) {
                System.out.print("Invalid input! Please enter 'Y' or 'N': ");
                continueChoice = scanner.next();
            }
            
            if (continueChoice.equalsIgnoreCase("N")) {
                break; 
            }
            
        } while (true); 
        
        System.out.println("Thank you!");
        
        scanner.close();
    }
}
