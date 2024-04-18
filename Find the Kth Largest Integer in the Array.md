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
```
## BigInteger in Java: Summary

1. **Creating BigInteger from a String:**

    - `BigInteger` represents arbitrary-precision integers in Java.
    - Use `BigInteger(String value)` to create a `BigInteger` object from a String representation of an integer.
    - This is necessary for numbers exceeding primitive integer types (`int`, `long`) to avoid precision loss.

2. **Converting BigInteger to int:**

    - `BigInteger` provides methods to convert its values to primitive types (`int`, `long`, `float`, `double`).
    - Use `intValue()` to convert a `BigInteger` to an `int`, allowing interaction with parts of your program expecting primitive types.

**Use Cases:**

- Employ `BigInteger` for calculations involving very large integers.
- Utilize `intValue()`, `longValue()`, `floatValue()`, and `doubleValue()` methods for conversions to primitive types:
  - Performing calculations requiring primitive types.
  - Compatibility with methods expecting primitive types.

**In essence:**

- `BigInteger` handles arbitrarily large integers.
- `new BigInteger(String value)` initializes `BigInteger`s from String representations.
- Methods like `intValue()` convert `BigInteger` values to primitive types when necessary.

