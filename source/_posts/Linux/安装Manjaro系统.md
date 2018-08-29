---
title: 安装Manjaro系统
date: 2018-07-29T00:50:59.664Z
tags: [Linux]
categories: [Linux]
---
# 前沿
>最近，接触到了一个新的Linux系统，这是基于ArchLinux的系统，听说有很好的软件支持和十分方面的使用方式，那么接下来回顾一下我的安装历程。

<!--more-->
# 制作启动盘

我用过这两个U盘启动盘制作器，Rufus,USBWriter。两个都曾失败过，不过后来用Rufus使用DD模式写入就成功了。
![](/images/Snipaste_2018-07-29_08-54-01.png)
制作的过程我们就不细说了，应该都会了。

# 重启

由于Manjaro的原因，我们需要先进入Boot，关闭securityboot，然后用U盘启动

# 进入Manjaro前的选择

emmmm，进入安装界面前会有一个选择面板，语言大家自己选，没影响的，在drive=free的时候大家可以选择nonfree，不过有的也是说按e键会进入编辑模式，把free改成intel好一点，我的就是这么做的，接下来选择boot进入liveCD系统进行安装。

# 安装Manjaro

emmmm,桌面会有一个安装程序，接下来打开它，按顺序进行，分区时选择手动分区（双系统），我预留了80G，拿出400M给了fat32,/boot/efi(这个Ubuntu之类的不是这个)，标记选择/boot,/efi什么的。/用了20G，无标记。/home用了剩余的。接下来就开始安装了。不过有可能会卡住，我们需要在某个文件注释两行代码，代码等会公司发。然后进安装成功了。
[驱动问题导致需要注释掉的代码](https://forum.manjaro.org/t/calamares-install-fails/16511/7)
[Ubuntu/Win10双系统安全删除Ubuntu的方法](https://blog.csdn.net/Meditator_hkx/article/details/52626077)
[删除Ubuntu的UEFI启动项](https://blog.csdn.net/smilingc/article/details/51236717)
[manjaro安装时卡住的解决办法](https://www.vcvoo.com/archives/101/)

# 问题：没有gruB启动项

[删除Ubuntu的UEFI启动项](https://blog.csdn.net/smilingc/article/details/51236717)


