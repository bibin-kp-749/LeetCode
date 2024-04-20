# 1. Two Sum
## Question ❓ <br>
 Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.  
 You may assume that each input would have exactly one solution, and you may not use the same element twice.
<br><br>

## Example

__Example 1:__
Input: nums = [2,7,11,15], target = 9  
Output: [0,1]  
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1]. 
<br>

__Example 2:__  
Input: nums = [3,2,4], target = 6  
Output: [1,2] 
<br>

__Example 3:___
Input: nums = [3,3], target = 6  
Output: [0,1]
<br>
  
## Constraints:

- 2 <= nums.length <= 104
- -109 <= nums[i] <= 109
- -109 <= target <= 109

# Code
```javascript
const twoSum = (nums, target) => {
    let newarray=[],num=1;
    for (let i = 0; i < nums.length - 1; i++) {
        for (let j = num; j < nums.length; j++) {
            if(nums[i] + nums[j] == target) { 
                newarray.push(i,j);
            }
        }
        num++
    }
    return newarray;
}
let result = twoSum([2,7,11,15], 9)
console.log(result)
```
