# Khushi_02-04-26_Day-12

## Problem Name
Remove Duplicates from Sorted List

## Problem Link
https://leetcode.com/problems/remove-duplicates-from-sorted-list/

## Approach

- Traverse the linked list
- Compare current node with next node
- If values are same → skip next node
- Else → move forward
- Continue till end

## Complexity

- Time Complexity: O(n)
- Space Complexity: O(1)

## Code (C++)

class Solution {
public:
    ListNode* deleteDuplicates(ListNode* head) {
        ListNode* curr = head;

        while (curr && curr->next) {
            if (curr->val == curr->next->val) {
                curr->next = curr->next->next;
            } else {
                curr = curr->next;
            }
        }

        return head;
    }
};
<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/6425b5fc-e638-46e8-b08c-6537430ae49a" />

