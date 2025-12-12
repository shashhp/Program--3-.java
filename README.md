# Program--3-.java
import java.util.Scanner;

public class OddSeriesPattern {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a value for a: ");
        int a = sc.nextInt();
        int terms = (a % 2 == 0) ? a - 1 : a;
        for (int i = 1; i <= terms; i++) {
            int term = 2 * i - 1;   // i-th odd number
            if (i == terms) {
                System.out.print(term);
            } else {
                System.out.print(term + ", ");
            }
        }
        sc.close();
    }
}
