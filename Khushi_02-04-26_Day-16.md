On Day 16, I solved the Implement Queue using Stacks problem.

Problem Summary:

Design a queue (FIFO) using only two stacks. The implemented queue should support standard operations such as push, pop, peek, and empty.

Approach:
Used two stacks to simulate queue behavior.
First stack (s1) is used for push operations.
Second stack (s2) is used for pop and peek operations.
When s2 is empty, elements from s1 are transferred to s2, reversing their order to maintain FIFO behavior.
Key Concepts:
Stack operations (LIFO)
Queue implementation (FIFO)
Amortized time complexity
Data structure transformation
Complexity:
Time Complexity:
Push: O(1)
Pop/Peek: Amortized O(1)
Space Complexity: O(n)
Outcome:<img width="1920" height="1080" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/2a3f8746-0ef9-401a-9907-a958f90f3dcc" />

Successfully implemented a queue using stacks while maintaining efficient operations.
