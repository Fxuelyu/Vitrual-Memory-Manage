# Vitrual Memory Manage
> This is BUAA OS Experiment 3. 

> OS实验3 - 虚存管理

## Introduction 介绍
基本要求：
了解Linux系统下页式存储管理机制，并实现一个简单的虚存管理模拟程序。具体要求如下：
* 设计并实现一个虚存管理模拟程序，模拟一个单道程序的页式存储管理，用一个一维数组模拟实存空间，用一个文本文件模拟辅存空间。
* 建立一张一级页表。
* 程序中使用函数do_request()随机产生访存请求，访存操作包括读取、写入、执行三种类型。
* 实现函数do_response()相应访存请求，完成虚地址到实地址的定位及读/写执行操作，同时判断并处理缺页中断。
* 实现LFU页面淘汰算法。

提高要求：

1. 实现多道程序的存储控制。
1. 建立一张多级页表或快表。
1. 将do_request()和do_response()函数实现在不同的进程中，通过进程间通信（如FIFO）完成访存控制的模拟。
1. 实现其他页面淘汰算法，如页面老化算法。

## How to use 使用方法
在Unix/Linux终端中，通过`cd`命令修改至源文件目录，执行`make`即可编译。
执行`make clean`可以执行清理操作。