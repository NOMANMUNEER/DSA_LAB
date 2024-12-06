# Problem Solving: Singly Linked List (SLL)

## Objectives:
1. To build a **Singly Linked List (SLL)** class.
2. To solve problems related to SLL.

---

## Problem 1: Singly Linked List Class

### Description:
Write a **Singly Linked List (SLL)** class as discussed in the theory lecture. The `SLList` class should have methods that allow inserting at the head and tail of the list, deleting from the head and tail, and printing the list.

### Requirements:
- The class should support the following methods:
  - **insertAtHead(int value)**: Inserts a node with the given value at the head of the list.
  - **insertAtTail(int value)**: Inserts a node with the given value at the tail of the list.
  - **deleteHead()**: Deletes the node at the head of the list.
  - **deleteTail()**: Deletes the node at the tail of the list.
  - **print()**: Prints the contents of the list.

### Example of the main program:
```cpp
int main()
{
    SLList intSLL;
    for (int i{1}; i < 10; ++i)
    {
        intSLL.insertAtHead(i*5);   // Insert at head
        intSLL.insertAtTail(i*10);  // Insert at tail
    }
    
    intSLL.print();  // Print the list
    
    for (int i{1}; i < 5; ++i)
    {
        intSLL.deleteHead();  // Delete from head
        intSLL.deleteTail();  // Delete from tail
    }
    
    intSLL.print();  // Print the list again
}
