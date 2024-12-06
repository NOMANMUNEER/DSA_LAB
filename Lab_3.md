# Problem Solving: Doubly Linked List (DLL)

### Objective:
To build a **Doubly Linked List (DLL)** class and solve related problems, including deleting nodes by key, counting the number of nodes, and checking if the list is empty.

---

## Problem 1: Doubly Linked List Class

### Description:
Write a **Doubly Linked List (DLL)** class, as discussed in the theory lecture, following a similar pattern as for **Singly Linked List (SLL)**. Implement it so that the following `main()` program works correctly.

### Example Program:
```cpp
#include <iostream>
using namespace std;

class DLList {
public:
    struct Node {
        int data;
        Node* next;
        Node* prev;
        Node(int value) : data(value), next(nullptr), prev(nullptr) {}
    };

    DLList() : head(nullptr), tail(nullptr) {}
    ~DLList();

    void insertAtHead(int value);
    void insertAtTail(int value);
    void deleteHead();
    void deleteTail();
    void print() const;
    DLList& operator=(const DLList& other);
    DLList(const DLList& other); 

private:
    Node* head;
    Node* tail;
};

int main() {
    DLList intDLL;
    for (int i = 1; i < 10; ++i)
    {
        intDLL.insertAtHead(i * 5);   // Insert at head
        intDLL.insertAtTail(i * 10);  // Insert at tail
    }

    intDLL.print();  // Print the list

    DLList int2DLL {intDLL};  // Copy constructor
    int2DLL.deleteHead();     // Delete the head node
    int2DLL.print();          // Print the list after deletion

    int2DLL = intDLL;         // Assignment operator
    for (int i = 1; i < 5; ++i)
    {
        int2DLL.deleteHead();  // Delete from head
        int2DLL.deleteTail();  // Delete from tail
    }
    int2DLL.print();  // Print the list after deletions

    return 0;
}


