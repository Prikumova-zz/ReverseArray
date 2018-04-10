# ReverseArray

import java.util.Scanner;
public class ReverseArray {

	public static void main(String[] args) {
		System.out.println("Insert the number");
		Scanner in = new Scanner (System.in);
		int n = in.nextInt();
		int [] arr = new int [n];
		for(int i = 0; i<n; i++) {
			arr[i] = in.nextInt();
		}
		for (int i = 0; i < arr.length/2; i++) 
        {
			int temp = arr[i];
		    arr[i] = arr[arr.length - i - 1];
		    arr[arr.length - i - 1] = temp;
        }
		for(int i = 0; i<n; i++) {
			System.out.println(arr[i]);
		}
	}	

}
