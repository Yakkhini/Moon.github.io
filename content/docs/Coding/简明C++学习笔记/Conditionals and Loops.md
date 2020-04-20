---
weight: 2
---
# 简明C++学习笔记

# Conditionals and Loops 条件与循环
本章记录了C++条件语句与一些循环(for, while, switch等)的用法。

## Increment Operator 增量运算符

增量运算符有两种，一种是 **prefix** 形式，一种是 **post fix** 形式。

```c++
++x; //prefix
x++; //postfix
```
它们有什么区别呢？

{{< tabs "01">}}
{{< tab "Prefix">}}
```c++
x = 5;
y = ++x;
//Then x = 6, y = 6
```
Prefix先令x增值，再代入计算。
{{< /tab >}}
{{< tab "Postfix" >}}
```c++
x = 5;
y = x++;
//Then x = 6, y = 5
```
Postfix先让x代入计算，再令其增值。
{{< /tab >}}
{{< /tabs >}}

同样的，我们也有 **递减运算符** 。
```c++
--x; //prefix
x--; //postfix
```
它的所有特性都与增量运算符相同，只不过它可以令数字递减。
_注：在具有意义的数学计算中，我们仍然建议使用"x = x + 1;"，只有在逻辑运算中再使用递增、递减运算符。_

## Assignment Operators 赋值运算符
不需多讲，一个例子就好。

```c++
int x = 10;
x += 4; // equivalent to x = x + 4
x -= 5; // equivalent to x = x - 5
x *= 3; // equivalent to x = x * 3
x /= 2; // equivalent to x = x / 2
x %= 4; // equivalent to x = x % 4
```

不建议使用。

![测试图片](/Moon.github.io/docs/Coding/C++Notes/img/test.JPG)