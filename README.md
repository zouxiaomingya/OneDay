<h1 align="center">One Day</h1>
<p align="center">每天记录一点</p>

### 反转链表

> 2019 年 12 月 19 日

反转一个单链表。


**示例:**

```
  输入: 1->2->3->4->5->NULL
  输出: 5->4->3->2->1->NULL
```
进阶:
你可以迭代或递归地反转链表。你能否用两种方法解决这道题？


### 二叉树的最大深度

> 2019 年 12 月 18 日

给定一个二叉树，找出其最大深度。

二叉树的深度为根节点到最远叶子节点的最长路径上的节点数。

说明: 叶子节点是指没有子节点的节点。

[原题 leetcode 链接](https://leetcode-cn.com/problems/reverse-linked-list/)

**示例:**
给定二叉树 [3,9,20,null,null,15,7]，

```
    3
   / \
  9  20
    /  \
   15   7
```

[原题 leetcode 链接](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree/)


[javaScript 代码实现答案](https://github.com/zouxiaomingya/oneDay/blob/master/answer/19-12-18_maxDepth)

### 阶乘后面的零

> 2019 年 12 月 17 日

给定一个整数 n，返回 n! 结果尾数中零的数量。


**示例1:**

```
输入: 3
输出: 0
解释: 3! = 6, 尾数中没有零。
```
**示例2:**

```
输入: 5
输出: 1
解释: 5! = 120, 尾数中有 1 个零.
```

说明: 你算法的时间复杂度应为 O(log n) 。
**示例3:**

[原题 leetcode 链接](https://leetcode-cn.com/problems/factorial-trailing-zeroes/)

#### 解题思路

- 乘积有0 只有 2 * 5 这样的。
- 所以看有多少个 2，5 那么就有多少个 0
- 由于 2 很多， 所以只要看5
```
比如 1 * 2 * 3 * 4 * 5 * 6 * 7 * 8 * 9 * 10 * 11 * 12 * 13 * 14 * 15 * 。。。。

4 = 2 * 2； 8 = 2 * 2 * 2 
25 = 5 * 5

所以 2 远远比 5 多

```
所以根据这样的方法来寻找可以分解多少个 5 来看有多少个 0 

[javaScript 代码实现答案](https://github.com/zouxiaomingya/oneDay/blob/master/answer/2019-12/19-12-16_trailingZeroes.js)

### 无重复字符的最长子串

> 2019 年 12 月 16 日

给定一个字符串，请你找出其中不含有重复字符的 **最长子串** 的长度。


**示例1:**

```
输入: "abcabcbb"
输出: 3 
解释: 因为无重复字符的最长子串是 "abc"，所以其长度为 3。
```
**示例2:**

```
输入: "bbbbb"
输出: 1
解释: 因为无重复字符的最长子串是 "b"，所以其长度为 1。
```
**示例3:**

```
输入: "pwwkew"
输出: 3
解释: 因为无重复字符的最长子串是 "wke"，所以其长度为 3。
     请注意，你的答案必须是 子串 的长度，"pwke" 是一个子序列，不是子串。

```

[原题 leetcode 链接](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters/)

[javaScript 代码实现答案](https://github.com/zouxiaomingya/oneDay/blob/master/answer/2019-12/19-12-16_lengthOfLongestSubstring)
### 最小栈

> 2019 年 12 月 15 日

设计一个支持 push，pop，top 操作，并能在常数时间内检索到最小元素的栈。

- push(x) -- 将元素 x 推入栈中。
- pop() -- 删除栈顶的元素。
- top() -- 获取栈顶元素。
- getMin() -- 检索栈中的最小元素。


**示例:**

```
MinStack minStack = new MinStack();
minStack.push(-2);
minStack.push(0);
minStack.push(-3);
minStack.getMin();   --> 返回 -3.
minStack.pop();
minStack.top();      --> 返回 0.
minStack.getMin();   --> 返回 -2.
```

[原题 leetcode 链接](https://leetcode-cn.com/problems/min-stack/)

[javaScript 代码实现答案](https://github.com/zouxiaomingya/oneDay/blob/master/answer/2019-12/19-12-15_MinStack)

### 两数相加

> 2019 年 12 月 14 日

给出两个 非空 的链表用来表示两个非负的整数。其中，它们各自的位数是按照 逆序 的方式存储的，并且它们的每个节点只能存储 一位 数字。

如果，我们将这两个数相加起来，则会返回一个新的链表来表示它们的和。

您可以假设除了数字 0 之外，这两个数都不会以 0 开头。

**示例1:**

```
输入：(2 -> 4 -> 3) + (5 -> 6 -> 4)
输出：7 -> 0 -> 8
原因：342 + 465 = 807
```

[原题 leetcode 链接](https://leetcode-cn.com/problems/house-robber/)

[javaScript 代码实现答案](https://github.com/zouxiaomingya/oneDay/blob/master/answer/2019-12/19-12-14_addTwoNumbers.js)



### 打家劫舍

> 2019 年 12 月 13 日

你是一个专业的小偷，计划偷窃沿街的房屋。每间房内都藏有一定的现金，影响你偷窃的唯一制约因素就是相邻的房屋装有相互连通的防盗系统，如果两间相邻的房屋在同一晚上被小偷闯入，系统会自动报警。

给定一个代表每个房屋存放金额的非负整数数组，计算你在不触动警报装置的情况下，能够偷窃到的最高金额。

**示例1:**

```
输入: [1,2,3,1]
输出: 4
解释: 偷窃 1 号房屋 (金额 = 1) ，然后偷窃 3 号房屋 (金额 = 3)。
     偷窃到的最高金额 = 1 + 3 = 4 。

```

**示例2:**

```
输入: [2,7,9,3,1]
输出: 12
解释: 偷窃 1 号房屋 (金额 = 2), 偷窃 3 号房屋 (金额 = 9)，接着偷窃 5 号房屋 (金额 = 1)。
     偷窃到的最高金额 = 2 + 9 + 1 = 12 。
```

[原题 leetcode 链接](https://leetcode-cn.com/problems/house-robber/)

#### 解题思路

- 标签：动态规划
- 动态规划方程：dp[n] = MAX( dp[n-1], dp[n-2] + num )
- 由于不可以在相邻的房屋闯入，所以在当前位置 n 房屋可盗窃的最大值，要么就是 n-1 房屋可盗窃的最大值，要么就是 n-2 房屋可盗窃的最大值加上当前房屋的值，二者之间取最大值
- 举例来说：1 号房间可盗窃最大值为 33 即为 dp[1]=3，2 号房间可盗窃最大值为 44 即为 dp[2]=4，3 号房间自身的值为 22 即为 num=2，那么 dp[3] = MAX( dp[2], dp[1] + num ) = MAX(4, 3+2) = 5，3 号房间可盗窃最大值为 55
- 时间复杂度：O(n)O(n)，nn 为数组长度

[javaScript 代码实现答案](https://github.com/zouxiaomingya/oneDay/blob/master/answer/2019-12/19-12-13_rob.js)

[可以参考的优秀的题解](https://leetcode-cn.com/problems/house-robber/solution/hua-jie-suan-fa-198-da-jia-jie-she-by-guanpengchn/)

### 验证回文串

> 2019 年 12 月 12 日

给定一个字符串，验证它是否是回文串，只考虑字母和数字字符，可以忽略字母的大小写。

说明：本题中，我们将空字符串定义为有效的回文串。

**示例1:**

```
输入: "A man, a plan, a canal: Panama"
输出: true
```

**示例2:**

```
输入: "race a car"
输出: false
```

[原题 leetcode 链接](https://leetcode-cn.com/problems/valid-palindrome/)



### 对称二叉树

> 2019 年 12 月 11 日


给定一个二叉树，检查它是否是镜像对称的。

例如，二叉树 [1,2,2,3,4,4,3] 是对称的。

```
    	1
       / \
      2   2
     / \ / \
    3  4 4  3
```

但是下面这个 [1,2,2,null,3,null,3] 则不是镜像对称的:
```
       1
      / \
     2   2
      \   \
      3    3
```
说明:
如果你可以运用递归和迭代两种方法解决这个问题，会很加分。

[原题 leetcode 链接](https://leetcode-cn.com/problems/symmetric-tree/)

### 仿 antd Table 布局

> 2019 年 12 月 10 日

中间部分溢出可以滚动，如下图 3 中情况所示

[antd Table 来源](https://ant-design.gitee.io/components/table-cn/#components-table-demo-fixed-columns)

![](https://github.com/zouxiaomingya/oneDay/blob/master/img/left.png)

![](https://github.com/zouxiaomingya/oneDay/blob/master/img/mid.png)

![](https://github.com/zouxiaomingya/oneDay/blob/master/img/right.png)

### 数组转二叉树
> 2019 年 12 月 7 日

将 [1,2,2,3,4,4,3] 转成下面的二叉树
```
    	1
       / \
      2   2
     / \ / \
    3  4 4  3
```

### 多数元素
> 2019 年 12 月 6 日

给定一个大小为 n 的数组，找到其中的多数元素。多数元素是指在数组中出现次数大于 ⌊ n/2 ⌋ 的元素。

你可以假设数组是非空的，并且给定的数组总是存在多数元素。

**示例1:**

```
输入: [3,2,3]
输出: 3
```

**示例2:**

```
输入: [2,2,1,1,1,2,2]
输出: 2
```



### 只出现一次的数字

> 2019 年 12 月 5 日

给定一个非空整数数组，除了某个元素只出现一次以外，其余每个元素均出现两次。找出那个只出现了一次的元素。

说明：

你的算法应该具有线性时间复杂度。 你可以不使用额外空间来实现吗？

**示例1:**

```
输入: [2,2,1]
输出: 1
```



**示例2:**

```
输入: [4,1,2,1,2]
输出: 4
```



### 杨辉三件2
> 2019 年 12 月 4 日

给定一个非负索引 *k*，其中 *k* ≤ 33，返回杨辉三角的第 *k* 行。

**示例:**

```
输入: 3
输出: [1,3,3,1]
```

**进阶：**

你可以优化你的算法到 *O*(*k*) 空间复杂度吗？

### 杨辉三角

给定一个非负整数 *numRows，*生成杨辉三角的前 *numRows* 行。

在杨辉三角中，每个数是它左上方和右上方的数的和。

**示例:**

```
输入: 5
输出:
[
     [1],
    [1,1],
   [1,2,1],
  [1,3,3,1],
 [1,4,6,4,1]
]
```



### 最后一个单词的长度
> 2019 年 12 月 3 日


给定一个仅包含大小写字母和空格 ' ' 的字符串，返回其最后一个单词的长度。

如果不存在最后一个单词，请返回 0 。

说明：一个单词是指由字母组成，但不包含任何空格的字符串。

**示例:**

```
输入: "Hello World"
输出: 5
```

[原题 leetcode 链接](https://leetcode-cn.com/problems/length-of-last-word/)



### 罗马数字转整数

罗马数字包含以下七种字符: `I`， `V`， `X`， `L`，`C`，`D` 和 `M`。

```
字符          数值
I             1
V             5
X             10
L             50
C             100
D             500
M             1000
```

通常情况下，罗马数字中小的数字在大的数字的右边。但也存在特例，例如 4 不写做 IIII，而是 IV。数字 1 在数字 5 的左边，所表示的数等于大数 5 减小数 1 得到的数值 4 。同样地，数字 9 表示为 IX。这个特殊的规则只适用于以下六种情况：

I 可以放在 V (5) 和 X (10) 的左边，来表示 4 和 9。
X 可以放在 L (50) 和 C (100) 的左边，来表示 40 和 90。 
C 可以放在 D (500) 和 M (1000) 的左边，来表示 400 和 900。
给定一个罗马数字，将其转换成整数。输入确保在 1 到 3999 的范围内。



[原题 leetcode 链接](https://leetcode-cn.com/problems/roman-to-integer)

### leetcode 盛最多水的容器（11题）

给定 n 个非负整数 a1，a2，...，an，每个数代表坐标中的一个点 (i, ai) 。在坐标内画 n 条垂直线，垂直线 i 的两个端点分别为 (i, ai) 和 (i, 0)。找出其中的两条线，使得它们与 x 轴共同构成的容器可以容纳最多的水。

说明：你不能倾斜容器，且 n 的值至少为 2。

[原题 leetcode 链接](https://leetcode-cn.com/problems/container-with-most-water)

**示例:**

```
输入: [1,8,6,2,5,4,8,3,7]
输出: 49
```



### leetcode 加一（66题）

给定一个由整数组成的非空数组所表示的非负整数，在该数的基础上加一。

最高位数字存放在数组的首位， 数组中每个元素只存储单个数字。

你可以假设除了整数 0 之外，这个整数不会以零开头。

**示例:**

```
输入: [1,2,3]
输出: [1,2,4]
解释: 输入数组表示数字 123。
```

**示例:**

```
输入: [4,3,2,1]
输出: [4,3,2,2]
解释: 输入数组表示数字 4321。
```


### leetcode 有效的括号（20题）

给定一个只包括 '('，')'，'{'，'}'，'['，']' 的字符串，判断字符串是否有效。

有效字符串需满足：

1. 左括号必须用相同类型的右括号闭合。

2. 左括号必须以正确的顺序闭合。

**注意空字符串可被认为是有效字符串。**

`示例1`

```
输入: "()"
输出: true
```

`示例2`

```
输入: "()[]{}"
输出: true
```

