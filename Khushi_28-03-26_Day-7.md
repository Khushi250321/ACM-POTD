# Khushi_28-03-26_Day-7

## Problem Name

Rotate Array

## Problem Link

https://leetcode.com/problems/rotate-array/

## Approach

* First reduced `k` using modulo (`k = k % n`) to avoid extra rotations.
* Created a temporary array.
* Placed each element at its new rotated index using:
  `(i + k) % n`
* Copied the result back.

##  Complexity

* Time Complexity: O(n)
* Space Complexity: O(n)

##  Code (C++)
class Solution {
public:
    void rotate(vector<int>& nums, int k) {
        int n = nums.size();

        k = k % n;

        vector<int> temp(n);

        for (int i = 0; i < n; i++) {
            temp[(i + k) % n] = nums[i];
        }

        nums = temp;
    }
};<img width="1920" height="1080" alt="Screenshot (688)" src="https://github.com/user-attachments/assets/bca86a7e-754b-4b99-9d8a-bceff44e7b7f" />


![Accepted](day3.png)
