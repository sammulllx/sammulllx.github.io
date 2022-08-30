---
title:C语言笔记
author: sammul
date: 2022-08-08 11:33:00 +0800
categories: [Blogging, Demo]
tags: [typography]
math: true
mermaid: true
image:
  path: /commons/devices-mockup.png
  width: 800
  height: 500
  alt: Responsive rendering of Chirpy theme on multiple devices.
---


# C语言判断题

------

- C语言实数：E 前E 后有数字，E 后数字为整数✅
- c语言中“.1e0"是什么意思 等于0.1相当于 0.1*10^0✅
- C语言整数 25u,+20L,-32 ✅
- C 语言整数 12f❌
- c语言实数 .e-1，2.1e0.2，E1，0.10E，1.0E4.0，1.2E1.2 ❌
- C语言程序可以定义多个不同内容的main函数❌
- 可运行C语言程序不需要包含main()函数 ❌
- C程序必须由main语句开始❌
- C程序的执行总是从main函数开始，在main函数结束。✅
- 结构化程序的三种基本结构是循环结构、选择结构、顺序结构 ✅
- 函数体必须由 {开始✅
- 注释中间可以嵌套另一个注释❌
- C语言本身没有输入输出语句，printf和scanf都是C语言标准函数库里实现的,并不是C语法里规定的,不是C的关键字✅
- C语言中数据类型包括整型，实型（也称浮点型），字符型✅
- 函数是C语言的基本组成单位✅
- break语句只能用在循环语句内部❌
- 可以根据需要在一个函数中定义另一个函数❌
- 对于字符串数组或字符串指针变量，由于数组名可以转换为数组和指针变量名本身就是地址，因此使用scanf()函数时，不需要在它们前面加上"&"操作符。✅
- 井号Define不是c语句所以后面不用加分号，typedef是c语句要加分号✅

# VIM

[vim文字教程](https://www.tuyrk.cn/imooc/1129-vim/)

四种模式：普通，插入，命令，可视化。



- 插入模式的操作

  - i #insert 光标位置插入

  - a #appent 光标后一位插入

  - o #open a line below 光标所在行下新一行

  - A #appent after line 光标行最后位置插入

  - I #insert before line 光标所在行最前方位置插入

  - O #append a line above 光标所在行上一行插入



- 可视化模式的操作

  - v/V进行可视化（光标/整行选中）操作,加ctrl可实现块状操作；

  - y命令可以复制选中的块，p可以粘贴复制的块，d可以删除选中的块。命令模式中的操作





- - 命令模式中使用set nu设置行号

  - 用syntax on开启语法高亮

  - sp(split水平)、vs(vertical split垂直)可进行分屏编辑

  - % s/str1/str2/[g] 可进行文本[全局]替换。 （无需输入中括号）



- 输入模式下快速纠错(终端下也有类似的快捷键)

  - ctrl+h 删除上一个字符

  - ctrl+w 删除上一个单词

  - ctrl+u 删除当前行

  - ctrl+a (终端) 快速移动到开头

  - ctrl+e (终端)快速移动到结尾

  - ctrl+f (终端)光标后移

  - ctrl+b (终端)光标迁移



-  快速切换 insert 和 normal 模式

  - insert->normal: ctrl+c 或者 ctrl+[

  - gi: normal 模式切换到 insert 模式，且到上次编辑的地方



- 正常模式移动的快捷方式

  - w/W: 移动到下一个word/WORD 开头

  - e/E: 移动到下一个 word/WORD 结尾

  - b/B: 移动到上一个 word/WORD 开头 (backword)

  

- 正常模式行间搜索移动

  - f{char}: 当前光标往行后搜索字符, 分号(;)下一个找到的字符，逗号(,)上一个找到的字符(无需打出大括号)

  - F{char}: 当前光标往前搜索字符

  - 0: 移动到行首第一个字符

  - ^: 移动到第一个非空白字符

  - $: 移动到行尾

  - g_: 移动到行尾非空白字符



- 正常模式垂直移动

  - 使用括号()在句子间移动

  - 使用{}在段落中移动

  - 可用esay-motion插件移动



- 正常模式页面移动

  - gg: 文件开头

  - G: 文件结尾

  - H: 屏幕的开头(Head)

  - M: 屏幕的中间(Middle)

  - L: 屏幕的结尾(Lower)

  - crtl+u: 上翻页（upword）

  - ctrl+f: 下翻页（forword）

  - zz: 屏幕置为中间