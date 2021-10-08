# hello-world
Testing Github
package Challenges;

public class Driver {
	public static void main(String[] args) {
		int[] nums = { 5, 10, 3, 6, 7, 8, 9 };
		int index1 = 0, index2 = 0,index3 = 0;

		// Your code here
		for (int i = 0; i < nums.length; i++) {
			if (nums[i] >= nums[index1]) {
				index1 = i;
			}
			if (nums[i] >= nums[index2] && index1 != i) {
				index2 = i;
			}
			if (nums[i] >= nums[index3] && index1 != i  && index2 != i) {
				index3 = i;
			}
		}
		System.out.println("[" + index1 + "," + index2 + "]");

	}
}
