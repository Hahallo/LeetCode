Given an array of non-negative integers, you are initially positioned at the first index of the array.

Each element in the array represents your maximum jump length at that position.

Determine if you are able to reach the last index.

For example:
A = [2,3,1,1,4], return true.

A = [3,2,1,0,4], return false.

题目：每个整数代表在该位置能够往后跳的最大步数，确定能否从第一个整数跳到最后一个整数。

解题思路：从倒数第二个整数开始，如果能够到达最后一个整数，则把该整数的位置设置为最后一个整数的位置。如果前面的整数能到达该整数则说明
能够到真正的最后一个整数。
