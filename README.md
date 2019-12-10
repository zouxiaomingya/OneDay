<h1 align="center">One Day</h1>
<p align="center">每天记录一点</p>



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

