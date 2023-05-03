Download Link: https://assignmentchef.com/product/solved-cs112-problem-set-3
<br>
<strong>Problem Set 3</strong>

<strong>Linked Lists, Recursion</strong>

<ol>

 <li><strong>*</strong>Given the following definition of a circular linked list (CLL) class:</li>

</ol>

public class Node {          public String data;          public Node next;

public Node(String data, Node next) {              this.data = data; this.next = next;

}

}

public class LinkedList {

private Node rear;  // pointer to last node of CLL

…       }

The class keeps a circular linked list, with a rear pointer to the last node.

Implement the following method in the LinkedList class, to delete the <em>first</em> occurrence of a given item from the linked list. The method returns true if the item is deleted, or false if the item is not found.




public boolean delete(String target) {

/* COMPLETE THIS METHOD */

}

<table>

 <tbody>

  <tr>

   <td width="79"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>




<ol start="2">

 <li><strong>*</strong> Implement a method in the circular linked list class of problem 1, to add a new item <em>after</em> the first occurrence (from the front) of a specified item. If the item does not exist in the list, the method should return false, otherwise true</li>

</ol>

public boolean addAfter(String newItem, String afterItem) {

/* COMPLETE THIS METHOD */

}

<ol start="3">

 <li>A <em>doubly linked list</em> (DLL) is a linked list with nodes that point both forward and backward. Here’s an example: 3 &lt;—&gt; 5 &lt;—&gt; 7 &lt;—&gt; 1</li>

</ol>

Here’s a DLL node definition:

public class DLLNode {          public String data;          public DLLNode prev, next;

public DLLNode(String data, DLLNode next, DLLNode prev) {              this.data = data; this.next = next; this.prev = prev;

}       }

The next of the last node will be null, and the prev of the first node will be null.

Implement a method to move a node (given a pointer to it) to the front of a DLL.

// moves target to front of DLL

public static DLLNode moveToFront(DLLNode front, DLLNode target) {

/** COMPLETE THIS METHOD **/       }

<ol start="4">

 <li>With the same DLLNode definition as in the previous problem, implement a method to reverse the sequence of items in a DLL. Your code should NOT create any new nodes – it should simply resequence the original nodes. The method should return the front of the resulting list.</li>

</ol>

public static DLLNode reverse(DLLNode front) {

/** COMPLETE THIS METHOD **/       }

<ol start="5">

 <li>Implement a RECURSIVE method to delete all occurrences of an item from a (non-circular) linked list. Use the Node class definition of problem 1. Return a pointer to the first node in the updated list.</li>

</ol>




public static Node deleteAll(Node front, String target) {

/* COMPLETE THIS METHOD */

}

<ol start="6">

 <li><strong>*</strong> Implement a RECURSIVE method to merge two <strong>sorted</strong> linked lists into a single <strong>sorted</strong> linked list WITHOUT duplicates. No new nodes must be created: the nodes in the result list are a subset of the nodes in the original lists, rearranged appropriately.</li>

</ol>

You may assume that the original lists do not have any duplicate items.

For instance:

l1 = 3-&gt;9-&gt;12-&gt;15    l2 = 2-&gt;3-&gt;6-&gt;12

should result in the following:

2-&gt;3-&gt;6-&gt;9-&gt;12-&gt;15

Assuming a <strong>Node</strong> class defined like this:

public class Node {          public int data;          public Node next;

}

Complete the following method:




public static Node merge(Node frontL1, Node frontL2) {

…

}


