# CountPrime
import java.util.Scanner;

public class PrimeNumberBetweenIntegers {

	public static void main(String[] args) {

		Scanner get = new Scanner(System.in);
		System.out.println("enter range for display prime number \n From");
		int p = get.nextInt();
		System.out.println("To :");
		int b = get.nextInt();
		int l = 0;
		int count=0;
		System.out.println("the Prime numbers are");
		for (int a = p; a <= b; a++) {
			for (int i = 2; i < a / 2; i++) {
				if (a % i == 0) {
					l = 1;
					break;
				}
			}
			if (l == 0) {
				System.out.println(" " + a);
			++count;
			}
			l = 0;
		}
		System.out.println("count is +"+count);
	}

}
