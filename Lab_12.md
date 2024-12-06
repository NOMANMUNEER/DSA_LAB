# Data Structures & Algorithms (CC-213)
**Sessional 1 (Spring ‘24)**

**Roll No.:** __________________  
**Date:** July 8, 2024  
**Time:** 90 mins.  
**Marks:** 30

**AKhuwat College University, Kasur**  
**Department of Information Technology**

---

## Q1: (10)

### Code:

```cpp
CQueue pFunc(int times) {
    CQueue q1;
    for (int i{}; i < times; ++i) {
        q1.enqueue(1);
        q1.enqueue(2);
        int a = q1.front(); // First element value.
        q1.dequeue();
        int b = q1.rear(); // Last element value.
        q1.enqueue(a + b);
    }
    return q1;
}

int main() {
    CQueue aQ;
    aQ = pFunc(6);
    int value {};
    for (int i{}; i < aQ.size(); ++i) {
        value = aQ.front();
        aQ.dequeue();
        cout << value << ' ';
    }
}
```
# Q2: (10)

## Problem Description

Write a member function `delete` in the `DLList` class that accepts a key and removes all elements from the list that contain the key.

### Class Definitions

#### `DLLNode` Class

```cpp
class DLLNode {
    int data {};
    DLLNode *RLink{}, *LLlink{};
    friend class DLList;
public:
    DLLNode(int = {}, DLLNode *RLink = {}, DLLNode *LLlink = {});
};
class DLList {
    DLLNode *head{}, *tail{};
    int size_{};
public:
    int size();
    // Write delete member function that removes all occurrences of the given key.
};
```
# Q3: (10)

## Problem Description

Write a non-member function that returns the maximum value from the given stack. You should also write its time complexity. The given stack shall remain the same after the function finishes its execution. No data structure other than stack is allowed in this function.
### Example:
Stack Contents: 2 -1 5 12 -3 21 9 0 //The left most element i.e. 2 is on top of stack.  
Function Returns: 21
