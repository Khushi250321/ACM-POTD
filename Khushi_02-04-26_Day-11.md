# Khushi_02-04-26_Day-11

## Problem Name
Merge Two Sorted Lists

## Problem Link
https://leetcode.com/problems/merge-two-sorted-lists/

## Approach

- Used iterative method
- Compared nodes of both lists
- Attached smaller node to result list
- Continued until one list ends
- Attached remaining nodes

## Complexity

- Time Complexity: O(n + m)
- Space Complexity: O(1)

## Code (C++)

class Solution {
public:
    ListNode* mergeTwoLists(ListNode* list1, ListNode* list2) {
        ListNode dummy(0);
        ListNode* tail = &dummy;

        while (list1 && list2) {
            if (list1->val < list2->val) {
                tail->next = list1;
                list1 = list1->next;
            } else {
                tail->next = list2;
                list2 = list2->next;
            }
            tail = tail->next;
        }

        tail->next = list1 ? list1 : list2;
        return dummy.next;
    }
};<img width="1920" height="1080" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/694e066c-5bbb-46ff-ab59-3d12c6ad73ea" />
