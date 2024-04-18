```java
import java.util.* ;
import java.io.*; 
public class Solution {
	public static int findSecondLargest(int n ,int[] arr) {
		if (arr.length<2) {
			return -1;
		}
		int max = Integer.MIN_VALUE;
		int secmax = Integer.MIN_VALUE;

		for(int i =0;i<arr.length;i++){
			if (arr[i]>max) {
				max=arr[i];
			}
		}

		for (int i = 0; i < arr.length; i++) {
			if (arr[i]>secmax && arr[i]!=max) {
				secmax = arr[i];
			}
		}
		if (secmax!=Integer.MIN_VALUE) {
			return secmax;
		}else{
			return -1;
		}
		
	}
}
```
