# LinkedList


LinkedList 


Problem: Simple manipulations of an array using LinkedList

import java.util.*;

class Java{
    public static void main(String... r){
        LinkedList<Integer> ll=new LinkedList<>();
        ll.add(1);
        ll.add(2);
        ll.add(3);
        ll.addFirst(0);
        ll.addLast(4);
        System.out.println("original linkedlist : " + ll);
        System.out.println("The size of original linkedlist is : "+ ll.size());
        LinkedList<Integer> LL=new LinkedList<>();
        LL.add(5);
        LL.add(6);
        LL.add(7);
        ll.addAll(LL);
        System.out.println("Updated linkedlist is : "+ ll);
        System.out.println("The size of an updated linkedlist is : " +  ll.size());
    }
}


/*
original linkedlist : [0, 1, 2, 3, 4]
The size of original linkedlist is : 5
Updated linkedlist is : [0, 1, 2, 3, 4, 5, 6, 7]
The size of an updated linkedlist is : 8
 */




Problem: Removeall and retainall usage in Linkedlist

import java.util.*;

class Java {
    public static void main(String... r) {
        LinkedList<Integer> ll = new LinkedList<>();
        ll.add(1);
        ll.add(2);
        ll.add(3);
        ll.addFirst(0);
        ll.addLast(4);
        System.out.println(ll);
        LinkedList<Integer> LL = new LinkedList<>();
        LL.add(5);
        LL.add(6);
        LL.add(7);
        //ll.addAll(LL);
        System.out.println(LL);
        ll.retainAll(LL);
        System.out.println("Only LL Linkedlist elements are retained in the updated one " + LL);
        LL.retainAll(ll);
        System.out.println("All the elements are removed in the list " + ll);
    }
}


/*
[0, 1, 2, 3, 4]
[5, 6, 7]
Only LL Linkedlist elements are retained in the updated one [5, 6, 7]
All the elements are removed in the list []
 */




















