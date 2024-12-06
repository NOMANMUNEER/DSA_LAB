# Objectives:
1. To build Circular Doubly Linked List (CDLL) class
2. To solve problems related to Linked List

---

# Problem 1

### Task:
Write a **Circular Doubly Linked List (CDLL)** class, as discussed in the Theory Lecture, and on the same pattern as was done for Doubly Linked List, so that the following `main()` program works correctly:

```cpp
int main() {
    CDLList intCDLL;
    for (int i = 1; i < 10; ++i) {
        intCDLL.insertAtHead(i * 5);
        intCDLL.insertAtTail(i * 10);
    }
    intCDLL.print();

    CDLList int2CDLL {intCDLL};
    int2CDLL.deleteHead();
    int2CDLL.print();

    int2CDLL = intCDLL;
    for (int i = 1; i < 5; ++i) {
        int2CDLL.deleteHead();
        int2CDLL.deleteTail();
    }
    int2CDLL.print();

    return 0;
}
```
# Problem 2

### Task:
Write a member function `deleteNodes` in the `CDLList` class of Problem 1 that accepts a key and deletes all the nodes containing the key from the list if the key is present in the list. Then test it (the `deleteNodes` function) in the `main()` program.

# Problem 3

### Task:
Write a member function `merge` in the `CDLList` class of Problem 1 to merge two circular doubly linked lists. Then, count the number of nodes in the merged list using a `length` function. Test the `merge` and `length` functions in the `main()` program.

