**Problem Statement:**

Given an integer array `nums` and an integer `k`, return the kth largest element in the array.

Note that it is the kth largest element in the sorted order, not the kth distinct element.

Can you solve it without sorting?

**Example 1:**

Input: nums = [3,2,1,5,6,4], k = 2
Output: 5
**Example 2:**

Here's your text formatted in GitHub-flavored Markdown for easy copying and pasting:

markdown
Copy code
**Problem Statement:**

Given an integer array `nums` and an integer `k`, return the kth largest element in the array.

Note that it is the kth largest element in the sorted order, not the kth distinct element.

Can you solve it without sorting?

**Example 1:**

Input: nums = [3,2,1,5,6,4], k = 2
Output: 5

markdown
Copy code

**Example 2:**

Input: nums = [3,2,3,1,2,4,5,5,6], k = 4
Output: 4


**Code:**

```java
import java.math.BigInteger;
import java.util.Arrays;

class Solution {
    public int findKthLargest(int[] nums, int k) {
        BigInteger[] arr = new BigInteger[nums.length];
        for (int i = 0; i < arr.length; i++) {
            arr[i] = new BigInteger(String.valueOf(nums[i]));
        }
        Arrays.sort(arr);
        BigInteger result = arr[arr.length - k];
        return result.intValue();
    }
}
