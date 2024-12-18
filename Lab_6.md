# Objectives:
1. To build Binary Heap (Priority Queue) class
2. To solve problems related to Priority Queue

---

# Problem 1

### Task:
Write a class for a **max Priority Queue** that executes the following program successfully:

```cpp
int main() {
    maxPQ pq1;
    for (int i = 0; i < 13; ++i) {
        pq1.enqueue(i);
    }
    pq1.print();
    return 0;
}
```

# Problem 2

### Task:
Make additions to the class written in Problem 1 above so that the following program works correctly:

```cpp
int main() {
    maxPQ pq1;
    for (int i = 0; i < 13; ++i) {
        pq1.enqueue(i);
    }
    pq1.print();
    cout << pq1.max() << endl;
    pq1.dequeue();
    pq1.print();
    cout << pq1.max() << endl;
    pq1.dequeue();
    pq1.print();
    return 0;
}
```
# Problem 3
**(Note: write buildQueue() function in the class as done in the previous lecture. )**
### Task:
Make additions to the class written in **Problem 2** above so that the following program works correctly.

```cpp
int main() {
    int arr[15];
    for (int i = 0; i < 15; ++i) {
        arr[i] = i;
    }

    maxPQ pq1(arr);
    pq1.print();
    cout << pq1.max() << endl;
    pq1.dequeue();
    pq1.print();
    cout << pq1.max() << endl;
    pq1.dequeue();
    pq1.print();
    return 0;
}
