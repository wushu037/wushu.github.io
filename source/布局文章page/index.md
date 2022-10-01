---
title: 布局文章page
date: 2022-10-01 15:49:11
---
# 科普：GNU、LINUX、GUN/LINUX

> [CSDN：论GNU、Linux和GNU/Linux之间的关系
> 
> ](https://blog.csdn.net/tianjindong0804/article/details/85788270)

## GNU

> GNU 是一个操作系统，一个组织，一个计划或者叫运动。在这个旗帜下成立了 FSF，起草了 GPL 等。<br>
> [知乎：](https://www.zhihu.com/question/319783573/answer/656033035)Unix 系统被发明之后，大家用的很爽。但是后来开始收费和商业闭源了。一个叫 RMS 的大叔觉得很不爽，于是发起 GNU 计划，模仿 Unix 的界面和使用方式，从头做一个开源的版本。然后他自己做了编辑器 Emacs 和编译器 GCC。<br>
> [百度知道：](https://zhidao.baidu.com/question/1701652967552092220.html)这个组织中黑客云集，而且多是掌握核心技术的真正高手，他们的作品多是编译器、词法/语法分析器、底层函数库等大作。更重要的不是他们的技术，而是他们的哲学！他们的哲学就是技术上的“共产主义”——人人为我，我为人人。他们发布了一种版权许可协议——GPL——一个神圣的宣言。

GNU是一个自由的操作系统，其内容软件完全以[GPL](https://baike.baidu.com/item/GPL/2357903)方式发布。这个操作系统是[GNU计划](https://baike.baidu.com/item/GNU%E8%AE%A1%E5%88%92)的主要目标，名称来自GNU's Not Unix!的[递归缩写](https://www.cnblogs.com/wonderow/archive/2005/07/09/189523.html)，因为GNU的设计类似Unix，但它不包含具著作权的Unix代码。GNU的创始人，理查德·马修·斯托曼，将GNU视为“达成社会目的技术方法”。

> GNU计划，又译为“革奴计划”，是由理查德·斯托曼在1983年9月27日公开发起的自由软件集体协作计划。它的目标是创建一套完全自由的操作系统GNU。

创始人想要做一个仿照UNIX并且超过UNIX的操作系统。

**作为操作系统，GNU的发展仍未完成，其中最大的问题是具有完备功能的内核尚未被开发成功**。GNU的内核，称为Hurd，是自由软件基金会发展的重点，但是其发展尚未成熟。在实际使用上，多半使用Linux内核、FreeBSD等替代方案，作为系统核心，其中主要的操作系统是Linux的发行版。

[资料：](https://blog.csdn.net/tianjindong0804/article/details/85788270)**到了1990年，GNU计划已经开发出的软件包括了一个功能强大的文字编辑器Emacs，C语言编译器GCC，以及大部分UNIX系统的程序库和工具。唯一依然没有完成的重要组件就是操作系统的内核(称为HURD)**

GNU著名作品：

- GCC(GNU Compiler Collection)：C语言编译器
- Vim：编辑器之神，简单实用。-- 资料：[Vim和Emacs和IDE](https://baijiahao.baidu.com/s?id=1595652598707033588&wfr=spider&for=pc)
- Emacs：神之编辑器，功能足够多，学习使用太复杂

### Hurd

> **资料：**[**（整理）GNU Hurd项目详解**](http://www.ha97.com/3188.html)

简介：GNU Hurd 是 GNU 工程中取代 Unix 的核心。 Hurd 是一组运行在 Mach 微内核上的服务器，用来实现 Unix 或其他核心（如 Linux）实现了的文件系统、网络协议、及文件访问控制等其他功能。

GNU团队有很多牛人，Hurd内核的设计是==微内核设计==，结果太过于先进而导致现在也没有真正地弄出来。

Hurd原本是要成为GNU操作系统的真正内核，然而它从未真正降临人间。Linus Torvalds曾经写过，如果GNU kernel在1991年春天发布，他不会启动Linux项目。GNU操作系统项目始于1984年，在Linux出现之前它有7到8年的时间创造出一个可用的内核，然而它的开发进程，不时被频繁的改变中断。Richard Stallman为了无止境寻找完美内核，而忘记了HURD的原本目的：能用的操作系统。

hurd 一直就有，但总是没办法拿出来用而只能用于“技术试验”。
Debian 有 Hurd 内核的版本。[Debian GNU/Hurd](https://baike.baidu.com/item/Debian%20GNU%2FHurd/911411?fr=aladdin)

[Linux贴吧](http://tieba.baidu.com/p/5592533239)有和Richard Stallman的邮件，表示 GNU 目前没有把 Hurd 当成一个主要工作