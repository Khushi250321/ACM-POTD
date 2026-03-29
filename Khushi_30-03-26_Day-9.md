# Khushi_30-03-26_Day-9<img width="1920" height="1080" alt="Screenshot (698)" src="https://github.com/user-attachments/assets/6f2b2e20-39b2-4fcf-80d4-f4a53ab24356" />


## Problem Name

Linked List Cycle

## Problem Link

https://leetcode.com/problems/linked-list-cycle/

## Approach

* Used Floyd’s Cycle Detection Algorithm (Tortoise and Hare)
* Took two pointers:

  * `slow` moves one step at a time
  * `fast` moves two steps at a time
* If a cycle exists, both pointers will meet at some point
* If fast reaches NULL, then no cycle exists

## Complexity

* Time Complexity: O(n)
* Space Complexity: O(1)

## Code (C++)
class Solution {
public:
    bool hasCycle(ListNode *head) {
        ListNode* slow = head;
        ListNode* fast = head;

        while (fast != NULL && fast->next != NULL) {
            slow = slow->next;
            fast = fast->next->next;

            if (slow == fast) {
                return true;
            }
        }

        return false;
    }
};


![Accepted](day5.png)
