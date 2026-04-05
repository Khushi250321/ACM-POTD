On Day 15, I solved the Valid Parentheses problem.
<img width="1920" height="1080" alt="Screenshot (70)" src="https://github.com/user-attachments/assets/c4557d48-0301-4c42-af87-582643b74c60" />
Problem Summary
Given a string containing just the characters '(', ')', '{', '}', '[', and ']', determine if the input string is valid.
A string is valid if : 
Open brackets are closed by the same type of brackets
Open brackets are closed in the correct order
Approach:
Used a stack data structure to keep track of opening brackets.
Pushed opening brackets onto the stack.
For every closing bracket, checked if it matches the top of the stack.
If mismatch or stack is empty → invalid.
At the end, if stack is empty → valid string.
Key Concepts:
Stack (LIFO)
String traversal
Matching pairs logic
Complexity:
Time Complexity: O(n)
Space Complexity: O(n)
Outcome: 
Successfully implemented an efficient solution using stack to validate parentheses.
