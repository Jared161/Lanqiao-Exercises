# 43704 - 移动距离

![Year: 2015](https://img.shields.io/badge/Year-2015-white)
![Level: Provincial](https://img.shields.io/badge/Level-Provincial-blue)
![Python3](https://img.shields.io/badge/Python3-AC-green)

## 题目

### 题目描述

X 星球居民小区的楼房全是一样的，并且按矩阵样式排列。其楼房的编号为 $1,2,3,\cdots$

当排满一行时，从下一行相邻的楼往反方向排号。

比如：当小区排号宽度为 6 时，开始情形如下：

$$
\begin{matrix}
1&2&3&4&5&6\\
12&11&10&9&8&7 \\
13&14&15&\cdots
\end{matrix}
$$

我们的问题是：已知了两个楼号 $m,n$ ，需要求出它们之间的最短移动距离（不能斜线方向移动）

### 输入描述

输入为 3 个整数 $w,m,n$ ，空格分开，都在 1 到 10000 范围内， $w$ 为排号宽度， $m,n$ 为待计算的楼号。

### 输出描述

要求输出一个整数，表示 $m,n$ 两楼间最短移动距离。

### 输入输出样例

#### 示例 1

> 输入

```txt
6 2 8
```

> 输出

```txt
4
```

#### 示例 2

> 输入

```txt
4 7 20
```

> 输出

```txt
5
```

## 分析

本题的时间复杂度可以达到 $O(1)$ 。

按照题目要求进行横竖“真实”坐标差求和即可。
