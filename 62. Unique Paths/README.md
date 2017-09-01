
A robot is located at the top-left corner of a m x n grid (marked 'Start' in the diagram below).

The robot can only move either down or right at any point in time. The robot is trying to reach the bottom-right corner of the grid (marked 'Finish' in the diagram below).

How many possible unique paths are there?

题目意思很简单：一个长方形格子盘的左上角为起点，右下角为终点，机器人只能向左和向下移动。解有多少种到达终点的路径。

解题思路：因为要找到目的地的所有路径数，假设到达第i行j列的路径数为p[i][j],则有p[i][j]=p[i-1][j]+p[i][j-i]（只有且所有通过这两个格子的路径都能到达目的格子）。第1列和第1行的格子设p[i][0]=1,p[0][j]=1;然后算法就很容易写出来了。


 这种方法时间复杂度为o(n^2),空间复杂度为o(nxm);
 
上面这个算法可以进行优化，把空间复杂度降低。因为是按一行一行来求路径数的，每次用到的路径数据只有同一列上一行的数据和同一行上一列的数据，所以只要一个长度为min（m，n）的数组就行。

