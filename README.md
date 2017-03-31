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
