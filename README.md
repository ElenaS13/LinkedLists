##### LinkedLists

This is my knowledge gathering resource for all things LinkedLists. I try to use examples where possible to demontrate the functionality. 

##### Comparing two lists
In this exercise, we compare two linkedlists and return 1 if they are identical and 0 if they are not. 

```
int CompareLists(Node n1, Node n2) {
    if (n1 == null && n2 == null) {
        return 1;
    }
    while (n1 != null && n2 != null) {
        if (n1.data != n2.data) {
            return 0;
        }
        n1 = n1.next;
        n2 = n2.next;
    }
    return (n1 == null && n2 == null) ? 1 : 0;
}
```
##### Reverse a linked list
Return pointer to the head. The input list will have at least one element  

```
Node Reverse(Node head) {
    if (head == null && head.next == null) {
        return head;
    }
    Node prev = null;
    Node curr = head;
    Node next = null;
    while (curr != null) {
        next = curr.next;
        curr.next = prev; // changes arrow direction
        prev = curr;
        curr = next;
    }
    return prev;
}
```
##### From TutorialsPoint

Each link contains a connection to another link. 
Each link of a linked list can store data called element.
Each link contains a link to next link called next.
A linked list contains a connection link to the first link called first. 

##### Types of LinkedList 

Singly linked list - item navigation only forward
Doubly linked list - item navigation can be forward and backward
Cingular linked list - last item contains link as the first element as next and the first element has link to last element as prev. 

##### Basic Operations
Insertion - add an element at the beginning of the list.
Deletion - delete an element at the beginning of the list.
Display - display complete list.
Search - search an element using given key.
Delete - delete an element using given key. 

Algorithm is a sequence of steps, not a program. The same algorithm can be used in different programs. 
Data Strutures - schemes for organizing data. 

