# 3sum-java-solution
Leetcode 3Sum problem solved in Java using two pointers

3Sum Solution
This Java program finds all unique triplets in the array which gives the sum of zero.

Problem Statement
Given an integer array nums, find all unique triplets [nums[i], nums[left], nums[right]] such that their sum is zero (nums[i] + nums[left] + nums[right] == 0).

Approach
Sort the array to easily avoid duplicates and use the two-pointer technique.

Iterate over the array, fixing one element (nums[i]) at a time.

Use two pointers (left and right) to find pairs whose sum with nums[i] is zero.

Skip duplicates for i, left, and right to ensure unique triplets.

Add the triplet to the result list when the sum equals zero.

Adjust pointers based on the sum to find all possible triplets.

Code Explanation
Sort the input array nums.

Loop through each element i from 0 to nums.length - 3.

Skip duplicate values of nums[i].

Initialize two pointers: left = i + 1, right = nums.length - 1.

While left < right, calculate the sum of nums[i] + nums[left] + nums[right].

If sum == 0, add triplet to result and move pointers inward, skipping duplicates.

If sum < 0, increment left to increase the sum.

If sum > 0, decrement right to decrease the sum.

Return the list of unique triplets.

Time Complexity
Sorting: O(n log n)

Two-pointer scanning: O(n²)

Overall complexity: O(n²)
