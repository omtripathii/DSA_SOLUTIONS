**Easy Solution -- Not all test cases **

```java
import java.util.ArrayList;

public class Solution {
	public static ArrayList<Integer> rotateArray(ArrayList<Integer> arr, int k) {
        // Write your code here.
        ArrayList<Integer> rotated = new ArrayList<>();
        for(int i = k; i<arr.size() ; i++){
            rotated.add(arr.get(i));
        }
        for(int i = 0; i <k ;i++){
             rotated.add(arr.get(i));
        }

        return rotated;
    }
}
```

