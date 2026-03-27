# Khushi_27-03-26_Day-2

## Problem Name

Check If N and Its Double Exist

## Problem Link

https://leetcode.com/problems/check-if-n-and-its-double-exist/

## Approach

* Used hash set for efficient lookup.
* For each element `x`, checked if `2*x` or `x/2` already exists in the set.
* If found, return true.
* Otherwise, insert the element into the set.

## Complexity

* Time Complexity: O(n)
* Space Complexity: O(n)

##  Code (C++)

```cpp
class Solution {
public:
    bool checkIfExist(vector<int>& arr) {
        unordered_set<int> s;

        for (int x : arr) {
            if (s.count(2 * x) || (x % 2 == 0 && s.count(x / 2))) {
                return true;
            }
            s.insert(x);
        }

        return false;
    }
};
```
<img width="1920" height="1080" alt="Screenshot (687)" src="https://github.com/user-attachments/assets/f2de1146-63c6-4d47-a55a-51d22cb54c28" />


![Accepted](day2.png)
