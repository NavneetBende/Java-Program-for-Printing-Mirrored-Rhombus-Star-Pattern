Printing Mirrored Rhombus Star Pattern
In this problem we’re going to code a Java Program for printing mirrored rhombus star pattern.

For doing so we’ll take a number input from user and store it in variable rows and then run the for loop start from i=0 to ii which print the spaces and then take a another loop to print star start from j=0 to j

Java Program for Mirrored Rhombus Star Pattern
Algorithm:
Take the number of rows as input from the user (length of side of rhombus) and store it in any variable.(‘row‘ in this case).
Run a loop ‘row’ number of times to iterate through each of the rows. From i=0 to i<row. The loop should be structured as for(int i=0;i<rows;i++)
 Run a nested loop inside the main loop to print the spaces before the rhombus. From j=row to j>i. The loop should be structured as for(int j=rows;j>i;j–)
Run another nested loop inside the main loop after the previous loop to print the stars in each column of a row. From j=0 to j<row. The loop should be structured as for(int j=0;j<rows;j++) inside this loop print System.out.println(“*”);
Move to the next line by printing a new line System.out.println();
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter No");
		int rows = sc.nextInt();
		
		
		for(int i=0;i<rows;i++)      //loop controlling number of rows
		   {
		      for(int j=rows;j>i;j--) //inner loop for spaces
		          System.out.print(" "); //printing spaces
		      for(int j=0;j<rows;j++) //inner loop for printing the stars in each column of a row
		           System.out.print("*"); //printing stars
		      System.out.println(); // printing a new line after each row
	   }
	}
}
