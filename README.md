# Merge-two-sorted-linked-lists-hackerank-solution
You’re given the pointer to the head nodes of two sorted linked lists. The data in both lists will be sorted in ascending order. Change the next pointers to obtain a single, merged linked list which also has data in ascending order. Either head pointer given may be null meaning that the corresponding list is empty.

Input Format

You have to complete the SinglyLinkedListNode MergeLists(SinglyLinkedListNode headA, SinglyLinkedListNode headB) method which takes two arguments - the heads of the two sorted linked lists to merge. You should NOT read any input from stdin/console.

The input is handled by the code in the editor and the format is as follows:

The first line contains an integer

, denoting the number of test cases.
The format for each test case is as follows:

The first line contains an integer
, denoting the length of the first linked list.
The next lines contain an integer each, denoting the elements of the linked list.
The next line contains an integer , denoting the length of the second linked list.
The next

lines contain an integer each, denoting the elements of the second linked list.


Output Format

Change the next pointer of individual nodes so that nodes from both lists are merged into a single list. Then return the head of this merged list. Do NOT print anything to stdout/console.

The output is handled by the editor and the format is as follows:

For each test case, print in a new line, the linked list after merging them separated by spaces.

Sample Input

1
3
1
2
3
2
3
4

Sample Output

1 2 3 3 4 

Explanation

The first linked list is: 1 -> 2 -> 3 -> NULL

The second linked list is: 3 -> 4 -> NULL

Hence, the merged linked list is: 1 -> 2 -> 3 -> 3 -> 4 -> NULL

## MY SOLUTION
Merging two sorted linked list is performed by the use of three pointers i.e. p pointer that points to the head of first linked list ,q pointer that points to the head of second linked list and head pointer that points to the head of new linked list. The corresponding value which is less among the p and q pointer is pushed untill end of any list is reached. If on reaching the end if still any list is left to be evaluated then the while loop is used which simply pushes the data in the new link list referenced by the head pointer.
