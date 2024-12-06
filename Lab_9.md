# Objectives:
1. To build problem-solving skills

---

# Problem 1

### Part a: Function to Merge Two Sorted Arrays

Write a function `merge(..)` that is passed two arrays, `arr1` & `arr2`, of integers. These arrays are in non-decreasing order. The function shall merge the contents of both arrays into a new array `arr`, which contains all the elements of `arr1` & `arr2` in non-decreasing order. Finally, the function should return the merged array.
# Example

**Array arr1:**  
`2 5 8 12 45 67`

**Array arr2:**  
`1 11 21 31 35 44 53`

**Array arr (merged):**  
`1 2 5 8 11 12 21 31 35 44 45 53 67`

## Part b: Write the `main(..)` function to test the function written in part a)

Below is the `main()` function to test the `merge(..)` function from part a):
# Problem 2

### a) Write a function, `insert(..)`, that takes a sorted array of integers and a value, and inserts the value in the array such that the array remains sorted after the insertion.

### Example:

**Array before function call:**  
`34 31 27 22 18 15 12 9`

**Value:**  
`26`

**Array after function call:**  
`34 31 27 26 22 18 15 12 9`
### b) Write the `main(..)` function to test the function written in part a)
# Problem 3

### a) Write a recursive C++ function, `countOccurrences(…)`, to count all the occurrences of a given number `K` in a given array of integers. The prototype of the function is given below:

```cpp
int countOccurrences(int *array, int startIndex, int endIndex, int K);
```
**Note:** Do not use any global or static variables.

### b) Write the `main(..)` function to test the function written in part a)

