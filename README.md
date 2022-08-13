# Monkey Compiler
《用Go语言自制编译器》
https://www.ituring.com.cn/book/2882

## CH1
介绍概念：编译器和虚拟机，以及项目目标

## CH2
如果没有实现过Monkey解释器，需要下载随书的代码，把ast，lexer，parser，repl，token目录和main.go复制到项目下，
本项目需要复用解释器中的这部分解析ast的逻辑。

这个章节定义了字节码指令，实现了最小的编译器原型，从源码编译出字节码，并且实现栈式虚拟机，把编译出的字节码扔到虚拟机里执行，输出结果。

实现了两个Op：Constant和Add，能够实现两个数的加法。

实现基于编译器和虚拟机的REPL，便于调试

主要时间在写测试的代码，单元测试对实现过程有很大帮助