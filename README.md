# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over arrays.  The `BuggyArray.java` file contains the erroneous code, which attempts to access an array element beyond its valid index. The `FixedArray.java` provides the corrected version.

**Problem:**
The original code's `for` loop condition `i <= arr.length` is incorrect when accessing array elements.  Array indices start at 0 and go up to `arr.length - 1`.  The loop attempts to access `arr[5]` which is outside of bounds of the array with length 5 causing an ArrayIndexOutOfBoundsException. 

**Solution:**
The corrected code uses the condition `i < arr.length` which correctly iterates up to the last valid index. 

This example highlights the importance of careful array index management to avoid common runtime exceptions.