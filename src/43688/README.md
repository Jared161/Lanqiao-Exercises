# 43688 - Excel 地址

![Year: 2017](https://img.shields.io/badge/Year-2017-white)
![Level: Provincial](https://img.shields.io/badge/Level-Provincial-blue)
![Python3](https://img.shields.io/badge/Python3-AC-green)

## 题目

### 题目描述

Excel 单元格的地址表示很有趣，它使用字母来表示列号。

比如，

A 表示第 1 列，

B 表示第 2 列，

Z 表示第 26 列，

AA 表示第 27 列，

AB 表示第 28 列，

BA 表示第 53 列，

$\cdots$

当然 Excel 的最大列号是有限度的，所以转换起来不难。

如果我们想把这种表示法一般化，可以把很大的数字转换为很长的字母序列呢？

本题目即是要求对输入的数字 , 输出其对应的 Excel 地址表示方式。

### 输入描述

输入一个整数 $n$ ，其范围 $[1, 2147483647]$ 。

### 输出描述

输出 $n$ 对应的 Excel 地址表示方式。

### 输入输出样例

#### 示例

> 输入

```txt
26
```

> 输出

```txt
Z
```

## 分析

这是一种特殊的**进制转换**题。

我们需要做的就是将 10 进制换算为 26 进制。唯一的特殊之处就是，这个 26 进制是不存在“0”的，在计算时需要将每个数位减去 1。
