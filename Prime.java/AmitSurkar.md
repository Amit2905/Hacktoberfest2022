// A school method based Java program to
// check if a number is prime
import java.lang.*;
import java.util.*;

class Prime {

	// Check for number prime or not
	static boolean isPrime(int n)
	{

		// Check if number is less than
		// equal to 1
		if (n <= 1)
			return false;

		// Check if number is 2
		else if (n == 2)
			return true;

		// Check if n is a multiple of 2
		else if (n % 2 == 0)
			return false;

		// If not, then just check the odds
		for (int i = 3; i <= Math.sqrt(n); i += 2) {
			if (n % i == 0)
				return false;
		}
		return true;
	}

	// Driver code
	public static void main(String[] args)
	{
		if (isPrime(19))
			System.out.println("The number is prime");

		else
			System.out.println("The number is not prime");
	}
}
 
 Output:-
 ![image](https://user-images.githubusercontent.com/72159431/198521518-69325104-8acc-4107-a3a0-2131d9839fe6.png)
