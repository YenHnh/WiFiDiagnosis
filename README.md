import java.util.Scanner;

public class WiFiDiagnosis
{

	public static void main(String[] args) 
	{
		String answer1, answer2, answer3, answer4;
		
	Scanner keyboard = new Scanner(System.in);
	
	System.out.println("If you have a problem with internet connectivity, this WiFi Diagnosis might work");
	System.out.println(" ");
	System.out.println("First step: reboot your computer");
	System.out.println("Are you able to connect with the internet? (yes or no): ");
	
	answer1 = keyboard.nextLine();

	
	if((answer1.equals("yes")) || (answer1.equals("Yes")) || (answer1.equals("YES")))
	{
	System.out.println("Rebooting your computer seemed to work");
	}
	else if ((answer1.equals("no")) || (answer1.equals("No")) || (answer1.equals("NO")))
	{
		System.out.println("Second step: reboot your router");
		System.out.println("Now are you able to connect with the internet? (yes or no): ");
		
		answer2 = keyboard.nextLine();
		
		if((answer2.equals("yes")) || (answer2.equals("Yes")) || (answer2.equals("YES")))
		{
		System.out.println("Rebooting your router seemed to work");
		}
		else if ((answer2.equals("no")) || (answer2.equals("No")) || (answer2.equals("NO")))
		{
			System.out.println("Third step: make sure the cables to your router are plugged in firmly and your router is getting power");
			System.out.println("Now are you able to connect with the internet? (yes or no): ");
			
			answer3 = keyboard.nextLine();
			
			if((answer3.equals("yes")) || (answer3.equals("Yes")) || (answer3.equals("YES")))
			{
			System.out.println("Checking the router's cables seemed to work");
			}
			else if ((answer3.equals("no")) || (answer3.equals("No")) || (answer3.equals("NO")))
			{
				System.out.println("Fourth step: make your computer closer to your router");
				System.out.println("Now are you able to connect with the internet? (yes or no): ");
				
				answer4 = keyboard.nextLine();
				
				if((answer4.equals("yes")) || (answer4.equals("Yes")) || (answer4.equals("YES")))
				{
				System.out.println("Move your computer seemed to work");
				}
				else if ((answer4.equals("no")) || (answer4.equals("No")) || (answer4.equals("NO")))
				{
					System.out.println("Fifth step: contact your ISP");
					System.out.println("Make sure your ISP is hooked up to your router.");
			}
		}
	}
		

	}

}
}
