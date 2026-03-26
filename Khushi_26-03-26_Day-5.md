# KHUSHI_26-03-26_Day-5

##  Problem Name

Move Zeroes

##  Problem Link

https://leetcode.com/problems/move-zeroes/

##  Approach

* Used two-pointer approach.
* Maintained index `j` to place non-zero elements.
* Swapped elements to maintain order.
* Zeroes moved to the end automatically.

##  Complexity

* Time Complexity: O(n)
* Space Complexity: O(1)

##  Code (C++)

```cpp
class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        int j = 0;
        for (int i = 0; i < nums.size(); i++) {
            if (nums[i] != 0) {
                swap(nums[i], nums[j]);
                j++;
            }
        }
    }
};
```

## <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2ab8fa14-1552-4cc0-ad2c-b9480a15c8ec" />


![Accepted](day5.png)<img width="1920" height="1080" alt="day5" src="https://github.com/user-attachments/assets/e2ed7583-fe76-470c-a621-b38a95666136" />
<img width="1920" height="1080" alt="day5" src="https://github.com/user-attachments/assets/9ca3adf0-bcaf-4114-b9f5-908c8617f586" />

