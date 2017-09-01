Find the contiguous subarray within an array (containing at least one number) which has the largest sum.

For example, given the array [-2,1,-3,4,-1,2,1,-5,4],
the contiguous subarray [4,-1,2,1] has the largest sum = 6.

题目：一个数组，找到连续的几个整数相加使其和是所有可能情况中最大的。

解题思路：①如果数组中的值都为负数，则找最大的负数。
②若果有正有负，则:
从第一个元素开始，如果元素为负数则跳过；如果元素为正数，则从该元素之后的第一个元素开始，如果该元素为正数，则直接与之前的和相加；若果为负数，则
该负数与之后的元素一个一个相加，直到其和为正数，然后再与之前的和相加。
数组中的每个正数都会得到一个最大的和，通过从这些和中找到最大的和，就是结果。
