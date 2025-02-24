Download link :https://programming.engineering/product/homework-1-singlylinkedlist/


# Homework-1-SinglyLinkedList
Homework 1: SinglyLinkedList
You are to code a SinglyLinkedList with head and tail references. A linked list is a collection of nodes, each having a data item and references to other nodes. In a SinglyLinkedList, each node has a reference to the next node. Since it is non-circular, the next reference for the tail is null.

Do not use a phantom node to represent the start or end of your list. A phantom or sentinel node is a node that does not store data held by the list and is used solely to indicate the start or end of a linked list. If your list contains n elements, then it should contain exactly n nodes.

The SinglyLinkedList must follow the requirements stated in the javadocs of each method you must implement. Your linked list implementation will use the default constructor (the one with no parameters) which is automatically provided by Java. Do not write your own constructor.

Nodes

The linked list consists of nodes. A class SinglyLinkedList is provided to you. This class has getter and setter methods to access and mutate the structure of the nodes.

Adding

You will implement three add() methods. One will add to the front, one will add to the back, and one will add to anywhere in the list given a specific index. See the javadocs for more details.

Removing

You will also implement three remove() methods – from the front, the back, or anywhere in the list given a specific index. Make sure that there is no longer any way to access the removed node so that the node will be garbage collected. See the javadocs for more details.

Garbage Collection

Java will automatically mark objects for garbage collection based on whether there is any means of accessing the object. In other words, if we want to remove a node from the list, we must remove all references to that node. What the next reference of that node points to doesn’t particularly matter. As long as no references can reach the node, the node will be garbage collected eventually.

Equality

There are two ways of defining objects as equal: reference equality and value equality.

Reference equality is used when using the == operator. If two objects are equal by reference equal-ity, that means that they have the exact same memory locations. For example, say we have a Person object with a name and id field. If you’re using reference equality, two Person objects won’t be considered equal unless they have the exact same memory location (are the exact same object), even if they have the same name and id.

Value equality is used when using the .equals() method. Here, the definition of equality is custom made for the object. For example, in that Person example above, we may want two objects to be con-sidered equal if they have the same name and id.

Keep in mind which makes more sense to use while you are coding. You will want to use value equality in most cases in this course when comparing objects. Notable cases where you’d use reference equality include checking for null or comparing primitives (in this case, it’s just the == operator being overloaded).

Homework 1: SinglyLinkedList Due: See Canvas

Differences between Java API and This Assignment

Some of the methods in this assignment are called different things or don’t exist in Java’s LinkedList class. Additionally, Java’s built in LinkedList is a Doubly-Linked List, so the efficiency of some opera-tions will differ. This won’t matter until you tackle coding questions on the first exam, but it’s something to be aware of. The list below shows all methods with a different name and their Java API equivalent if it exists. The format is assignment method name Java API name.

addAtIndex(int index, T data) ⇒ add(int index, T data)

addToFront(T data) ⇒ addFirst(T data)

addToBack(T data) ⇒ add(T data) or addLast(T data)

removeAtIndex(int index) ⇒ remove(int index)

removeFromFront() ⇒ poll() or pollFirst()

removeFromBack() ⇒ pollLast()

Homework 1: SinglyLinkedList Due: See Canvas

Grading

Here is the grading breakdown for the assignment. There are various deductions not listed that are incurred when breaking the rules listed in this PDF and in other various circumstances.

Methods:

addAtIndex

10pts

addToFront

5pts

addToBack

5pts

removeAtIndex

10pts

removeFromFront

5pts

removeFromBack

5pts

get

10pts

isEmpty

4pts

clear

5pts

removeLastOccurrence

10pts

toArray

6pts

Other:

Checkstyle

10pts

Efficiency

15pts

Total:

100pts

Provided

The following file(s) have been provided to you. There are several, but we’ve noted the ones to edit.

SinglyLinkedList.java

This is the class in which you will implement the SinglyLinkedList. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance variables, or static variables.

SinglyLinkedListStudentTest.java

This is the test class that contains a set of tests covering the basic operations on the SinglyLinkedList class. It is not intended to be exhaustive and does not guarantee any type of grade. Write your own tests to ensure you cover all edge cases.

Deliverables

You must submit all of the following file(s). Make sure all file(s) listed below are in each submission, as only the last submission will be graded. Make sure the filename(s) matches the filename(s) below, and that only the following file(s) are present. If there are multiple files, do not zip up the files before submitting; submit them all as separate files.

Once submitted, double check that it has uploaded properly on Gradescope. To do this, download your uploaded file(s) to a new folder, copy over the support file(s), recompile, and run. It is your sole responsibility to re-test your submission and discover editing oddities, upload issues, etc.

SinglyLinkedList.java
