# [从 0 到 1] - RPM 与 YUM

---

> **何为 [从 0 到 1]** : 即 从对某个事物 **一知半解** 或 **一无所知** 的状态，到 **理解基本概念** 和 **了解基本使用** 的状态。

## 前言

最近搞了台云服务器，准备自己折腾一下，发现自己并不了解 RPM 和 YUM 。

于是，开始在网上搜索一些教程进行学习。但是，我发现很多中文教程并不让我满意，要么是直接上来就告诉你有哪些命令，要么是告诉你怎么制作 RPM 包。其实对于初学者来讲，更需要的是了解相关的概念，这样就不会只知道复制命令执行了。

所以，我查了一些资料，整理出了此文。

**PS: 如果各位同志们有什么好的学习资源，可以分享一下。**

## 什么是 RPM

### 一句话解释

是一款 Linux 系统使用的包管理工具。

### 名称由来

原全称为 `Red Hat Package Manager` (因为最初是为 Red Hat 系列 Linux 开发的)，后来由于一些非 Red Hat 系列的 Linux 发行版本也在使用 RPM，所以把全称改为了 `RPM Package Manager` (递归命名方式) 。

### 使用 RPM 的系统

- Red Hat 系列。如 Fedora 、 CentOS 
- SUSE 系列。
- ……

## RPM 的软件包

以 `amanda-2.6.1p2-7.el6.x86_64.rpm` 为例

![image-20240406231610311]([从 0 到 1] - RPM 与 YUM/image-20240406231610311.png)

`release` 是打包者添加的发布信息。

这里的 `7` 表示这个包发布了 7 次 (可能要修复 bug)

`el6` 表示 **Red Hat Enterprise Linux 6** 。

## 如何使用 RPM





---

## 参考

1. [RPM 官网](https://rpm.org/index.html)
2. [rpm_tutorial_20120831.pdf](https://access.redhat.com/sites/default/files/attachments/rpm_tutorial_20120831.pdf)
   - 注意: **USING THE RPM COMMAND** 一节中使用的 `rpm -qp --checksig amanda-2.6.1p2-7.el6.x86_64.rpm` 命令在 **RPM version 4.11.3** 无法正常执行，改成 `rpm --checksig amanda-2.6.1p2-7.el6.x86_64.rpm` 后可正常执行。
3. [Linux 发行版本](https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg)
4. 
