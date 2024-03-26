# codsoft
I am excited to complete this internship of java programming
import java.util.Scanner;
import java.util.Random;
public class NumberGuessingGame {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner scanner=new Scanner(System.in);
		Random random=new Random();
		int targetNumber=random.nextInt(100)+1;//Generate a target element between 1 to 100
		int attempts=0;
		System.out.println("Welcome to Number Guessing Game!");
		System.out.println("The number between 1 and 100.can you guess it?");
		while(true) {
			System.out.println("Enter your Guess:");
			int guess=scanner.nextInt();
			attempts++;
			if(guess<targetNumber) {
				System.out.println("Value is too low! Try Again.");
			}else if(guess>targetNumber){
				System.out.println("Value is too High! Try Again");
			}
			else{
				System.out.println("Congratulations! You have guessed the number in "+attempts+" attempts!");
				break;
			}
			
			
			}
		scanner.close();
		}
	}


