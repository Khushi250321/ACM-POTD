# Khushi_29-03-26_Day-8

## Problem Name

Reverse Linked List

## Problem Link

https://leetcode.com/problems/reverse-linked-list/

## Approach

* Used iterative approach with 3 pointers:

  * `prev` (initially NULL)
  * `curr` (starting from head)
  * `next` (to store next node)
* Reversed links one by one:

  * Stored next node
  * Changed current node’s next to previous
  * Moved pointers forward
* Finally returned `prev` as new head

## Complexity

* Time Complexity: O(n)
* Space Complexity: O(1)

## <img width="1920" height="1080" alt="Screenshot (697)" src="https://github.com/user-attachments/assets/6ade2904-c9e2-4d48-a5f7-ba10bb7984a2" />
Code (C++)

```cpp
class Solution {
public:
    ListNode* reverseList(ListNode* head) {
        ListNode* prev = NULL;
        ListNode* curr = head;

        while (curr != NULL) {
            ListNode* next = curr->next; // store next
            curr->next = prev;           // reverse link
            prev = curr;                // move prev
            curr = next;                // move curr
        }

        return prev;
    }
};



![Accepted](day4.png)
