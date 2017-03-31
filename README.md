# LinkedLists

This is my knowledge gathering resource for all things LinkedLists. I try to use examples where possible to demontrate the functionality. 

<h1>HackerRank Solution<h1>

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
