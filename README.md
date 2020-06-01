# code_snippet_all_in_one
总结各种语言常见操作的代码，不熟悉新学习语言的语法也能快速开发.

- [code_snippet_all_in_one](#code_snippet_all_in_one)
  - [程序入口](#程序入口)
    - [c](#c)
    - [c++](#c-1)
    - [python](#python)
    - [java](#java)
    - [go](#go)
    - [rust](#rust)
    - [c-sharp](#c-sharp)
    - [Sleep](#sleep)
  - [代码组织](#代码组织)
    - [c](#c-2)
    - [python](#python-1)
  - [字符串](#字符串)
    - [字符串拼接](#字符串拼接)
      - [python](#python-2)
      - [Sleep](#sleep-1)
    - [判断字符串是否存在于另一个字符串](#判断字符串是否存在于另一个字符串)
      - [python](#python-3)
      - [Sleep](#sleep-2)
    - [搜索字符串位置](#搜索字符串位置)
      - [python](#python-4)
      - [Sleep](#sleep-3)
    - [字符串拆分](#字符串拆分)
    - [字符串统计](#字符串统计)
    - [字符串合并](#字符串合并)
    - [编码问题](#编码问题)
    - [空字符串，字符串比较](#空字符串字符串比较)
  - [类型转换](#类型转换)
  - [流程控制](#流程控制)
  - [基本复合类型](#基本复合类型)
  - [自定义类型](#自定义类型)
  - [用户输入输出](#用户输入输出)
  - [文件io](#文件io)
    - [写字符串到文件](#写字符串到文件)
      - [python](#python-5)
      - [Sleep](#sleep-4)
    - [读文件内容到字符串](#读文件内容到字符串)
    - [按行读取文件内容到数组](#按行读取文件内容到数组)
  - [错误处理](#错误处理)
  - [日期时间](#日期时间)
  - [随机数](#随机数)
  - [并发](#并发)
  - [http](#http)
  - [socket](#socket)
  - [加解密](#加解密)
  - [数据压缩](#数据压缩)
  - [测试](#测试)
  - [包管理](#包管理)

## 程序入口
### c
```
#include <stdio.h>
int main()
{
    printf("hello\n");
}
```
### c++
```
#include <iostream>
int main()
{
    std::cout << "hello" << endl;
}
```
### python
python可以不像c那样有特定入口函数main()
但可以用__name__
```
if __name__ == "__main__":
    print("hello")
```
### java
### go
### rust
### c-sharp
### Sleep
Sleep 是一个基于Java的，语法类似perl的语言，是cobalt strike的扩展语言
官方文档 http://sleep.dashnine.org/manual/index.html
没有入口函数，代码从上执行到下
解释器下载地址 http://sleep.dashnine.org/download.html
打开控制台
```
java -jar sleep.jar
```
加载写的脚本
```
load 1.cna
```

## 代码组织
### c
a.c
```
#include "b.h"
int main()
{
    test();
}
```
b.c
```
#include <stdio.h>
void test()
{
    printf("hello");
}
```
b.h
```
void test();
```
编译命令
```
gcc a.c b.c
```
### python

## 字符串

### 字符串拼接
#### python
```
a = "hello"
b = "world"
c = a + b
```
#### Sleep
```
$a = "hello";
$b = "world";
$c = $a . $b;
println($c);
```
### 判断字符串是否存在于另一个字符串
#### python
```
a = "h"
if a in "hello":
    print("in")
else:
    print("not in")
```
#### Sleep
```
$a = "hello world";
$b = 'hello';
$c = '*' . $b . '*';
if ( $c iswm $a) {
    println("match");
}
```
### 搜索字符串位置
#### python
```
```
#### Sleep
```
```
### 字符串拆分
### 字符串统计
### 字符串合并
### 编码问题
### 空字符串，字符串比较

## 类型转换

## 流程控制

## 基本复合类型

## 自定义类型

## 用户输入输出

## 文件io
### 写字符串到文件
#### python
```
with open('a.txt', w) as f:
    f.write('hello')
```
#### Sleep
openf打开文件时可以指定是覆盖还是追加，一个>是覆盖
```
if (-canwrite "/etc/passwd")
{
   $handle = openf(">>/etc/passwd");
   println($handle, "raffi::0:0::/:/bin/sh");
   closef($handle);
}
```
### 读文件内容到字符串
### 按行读取文件内容到数组

## 错误处理

## 日期时间

## 随机数

## 并发

## http

## socket

## 加解密

## 数据压缩

## 测试

## 包管理
