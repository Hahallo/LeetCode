You are climbing a stair case. It takes n steps to reach to the top.

Each time you can either climb 1 or 2 steps. In how many distinct ways can you climb to the top?

Note: Given n will be a positive integer.

题目：n个阶的阶梯，一次能走一步或两步，解所有从第一个阶梯走到最后一个阶梯的走法。

思路：动态规划，设n个阶的走法有p[n]，则n+1个阶的走法有p[n+1]=p[n]+p[n-1]。
