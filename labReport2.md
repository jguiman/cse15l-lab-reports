
# Lab Report #2
<br>
## Part 1: 3 screenshots
<br>
## Part 2: Two Bugs From Different Files
<br>
### Bug #1: reverseInPlace() for Array
<br>
1. reversing in Place does not correctly reverse half of the list of arrays greater than length 1.
2. The symptom is incorrect values for the second half of the array.
3. The bug is overwriting the original values of the second half of the array, we need a copy of the array for reference.
4. The symptom is getting a symmetric array instead of getting a reveresed in place array and it is connected to the bug is overwriting the first half of the indeces with the values at the end of the array and we lose access to the first half of values in the array due to it being overwritten.
<br>
### Bug #2: append() for Linked List
<br>
1. Appending to the LinkedList when the size is 2 or greater.
2. The symptom is an infinite loop.
3. The bug is attempting to iterate to the end of the linkedlist, but the bug makes it endless by adding a new node at the end and continuing to iterate.
4. The symptom of the infinite loop is related to the bug of not ending after we add the new node because we do not break out of the loop after creating and appending the new node.
