# Age-Driving
My first Java coding
import java.util.Scanner;

public class DrivingAgeSimulator{
    public static void main(String[] args) {
        int age;
        int birthYear;
        int currentYear;
        String answer;

        

        Scanner input = new Scanner(System.in);

        System.out.println("Welcome to the Driving Age Simulator!\n I will ask you a few questions to determine if you meet the legal driving age.");

        
        do{
            System.out.print("Enter the current year: ");
            currentYear = input.nextInt();
    
            System.out.print("Enter your birth year: ");
            birthYear = input.nextInt();

            age = currentYear - birthYear;

            if(age >= 21){
                System.out.println("Congratulations! You are eligible to drive.");
            }else if(age == 16){
                System.out.println("You are eligible to get your driver's permit. Congratulations!");
            }else{
                System.out.println("You are not old enough to drive.");
            }

            System.out.println("Do you want to continue? Type Yes or No: ");
            answer = input.next();






        } while(answer.equalsIgnoreCase("Yes"));
        
        System.out.println("Thanks for using the Driving Age Simulator");
        
        input.close();
        
    }

    
    
}
