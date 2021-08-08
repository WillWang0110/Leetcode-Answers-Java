# Leetcode-Answers-Java

## 榜样link： https://github.com/wisdompeak/LeetCode 北美代码下限跳槽，每日分栏目打卡五题到跳槽成功为止

Week 0 - 5 * 4 = 20 题
### 08/02 Two Pointers - 5
Two pointers 用来找sum
### 08/03 Binary Search - 5
二分法思想:
  int left = 0, right = nums.length - 1;
  while(left < right) {
    int mid = (left + right) / 2; // **此处可以用 (left + right) >> 1 避免overflow**
    ...
    ...
    ...
  }
  
  难点：上下界"="情况, edge case, bit左右移,
       Integer.MIN_VALUE = -2147483648, Integer.MAX_VALUE = 2147483647, 所以MIN_VALUE取反会造成overflow
       MAX_VALUE + 1 == MIN_VALUE, int型的最大值+1溢出后等于-214783648。二进制系统是通过补码来保存数据的。第一位是符号位，0为正，1为负，当正的除了符号位全为1，再加1就进位了，符号位就会变成1，是负数，其他为0。
  
### 08/04 Hash Table - 1
  
### 08/05 Heap - 0

### 08/06 Tree - 0

Binary search tree: 
```
 * The left subtree of a node contains only nodes with keys less than the node's key.
 * The right subtree of a node contains only nodes with keys greater than the node's key.
 * Both the left and right subtrees must also be binary search trees.
```
/**
 * Definition for a binary tree node.
 * public class TreeNode {
 *     int val;
 *     TreeNode left;
 *     TreeNode right;
 *     TreeNode() {}
 *     TreeNode(int val) { this.val = val; }
 *     TreeNode(int val, TreeNode left, TreeNode right) {
 *         this.val = val;
 *         this.left = left;
 *         this.right = right;
 *     }
 * }
 **/
 
要会三种traverse:
Inorder traverse




