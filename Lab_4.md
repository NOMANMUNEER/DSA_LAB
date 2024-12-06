# Objectives:
1. To build Stack class using array
2. To solve problems related to Stack

---

# Problem 1

### Task:
Write a `Stack` class, as discussed in the Theory Lecture, using an array so that the following `main()` program works correctly.

```cpp
int main()
{
    Stack aStack;
    for (int i{0}; i < 10; ++i)
    {
        aStack.push(i * 5);
    }
    for (int i{0}; i < 5; ++i)
    {
        cout << aStack.top();
        aStack.pop();
    }

    return 0;
}
```
# Problem 2

### Task:
Write a non-member function `print` that prints the contents of the stack, with the item at the top printed first. The contents of the stack shall remain the same after the `print` function execution. No other data structure except `Stack` is allowed for this question.

**Note:** The entire Stack ADT, as discussed in the lecture, shall be implemented.


