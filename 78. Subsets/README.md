Given a set of distinct integers, nums, return all possible subsets.

Note: The solution set must not contain duplicate subsets.

For example,
If nums = [1,2,3], a solution is:

[
  [3],
  [1],
  [2],
  [1,2,3],
  [1,3],
  [2,3],
  [1,2],
  []
]

题目：找所有子集
解题思路：
①普通思路:设已知长为n的数组的所有子集组成集合Sn，则长为n+1的数组的所有子集组成的集合Sn+1为Sn中所有集合加上An+1元素与Sn的并集。
所以从第一个元素开始，就可以得到所有子集。
②回溯
