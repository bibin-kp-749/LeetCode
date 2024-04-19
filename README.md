[# **Intuition**
<!-- Describe your first thoughts on how to solve this problem. -->

# Approach
<!-- Describe your approach to solving the problem. -->

# Complexity
- Time complexity:
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity:
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
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
