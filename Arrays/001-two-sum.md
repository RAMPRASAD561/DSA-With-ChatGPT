# Two Sum

- **Day:** 1
- **Date:** 2026-10-04
- **Difficulty:** Easy
- **Pattern:** Arrays / Brute Force

## Problem

Given an array `nums` and a target value, find two different indices whose values add up to the target.

Example:

```text
nums = [2, 7, 11, 15]
target = 9
Output = [0, 1]
```

## My Initial Approach

I used two nested loops. The first loop selects one element, and the second loop checks every element after it. If their sum equals the target, I return the two indices.

```python
def twoSum(nums, target):
    for i in range(len(nums)):
        for j in range(i + 1, len(nums)):
            if nums[i] + nums[j] == target:
                return [i, j]
```

## What ChatGPT Explained

The approach is correct and is called the brute-force approach. Starting the second loop at `i + 1` avoids checking the same pair twice and avoids using the same element twice.

## Complexity

- **Time:** O(n²)
- **Space:** O(1)

## Learning

I learned how to solve Two Sum using nested loops and how to analyze its time and space complexity.

## Key Takeaway

Before optimizing a DSA problem, first build a correct solution. Then look for a pattern that can reduce unnecessary work.
