# Khushi_05-04-26_Day-13

## Problem Name
Intersection of Two Linked Lists

## Problem Link
https://leetcode.com/problems/intersection-of-two-linked-lists/

## Approach

- Used two-pointer technique
- Pointer A starts at headA, Pointer B at headB
- When A reaches end → move it to headB
- When B reaches end → move it to headA
- If intersection exists → they meet at intersection node
- Else → both reach NULL

## Complexity

- Time Complexity: O(n + m)
- Space Complexity: O(1)

## Code (C++)

class Solution {
public:
    ListNode *getIntersectionNode(ListNode *headA, ListNode *headB) {
        ListNode* a = headA;
        ListNode* b = headB;

        while (a != b) {
            a = a ? a->next : headB;
            b = b ? b->next : headA;
        }

        return a;
    }
};

## Screenshot

![Accepted](day13.png)<img width="1920" height="1080" alt="Screenshot (63)" src="https://github.com/user-attachments/assets/969bf6c8-0a1f-45b8-a663-3775fb008020" />
