import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        
        System.out.println("Enter the first number: ");
        double num1 = s.nextDouble();
        
        System.out.println("Enter the second number: ");
        double num2 = s.nextDouble();
        
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
    } 
}
