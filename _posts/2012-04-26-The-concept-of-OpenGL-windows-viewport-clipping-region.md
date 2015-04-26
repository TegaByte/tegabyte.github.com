---
layout: post
title: The concept of OpenGL: windows, viewport, clipping region
category: OpenGL
---

##OpenGL概念辨析： 窗口，视口，裁剪区域

网上很多文章都谈过窗口，视口，裁剪区域这些概念，但感觉看了还是不很明白。下面是我个人实践过后的一些看法：

- 窗口：这就不用解释了吧
- 视口：就是窗口中用来显示图形的一块矩形区域，它可以和窗口等大，也可以比窗口大或者小。只有绘制在视口区域中的图形才能被显示，如果图形有一部分超出了视口区域，那么那一部分是看不到的。通过glViewport()函数设置。如下图所示：
![enter image description here](http://tegabyte.qiniudn.com/20150426_1.jpg)
图1. 不同大小的视口
- 裁剪区域（平行投影）：就是视口矩形区域的最小最大x坐标（left,right)和最小最大y坐标(bottom,top)，而不是窗口的最小最大x坐标和y坐标。通过glOrtho()函数设置，这个函数还需指定最近最远z坐标，形成一个立体的裁剪区域。
![enter image description here](http://tegabyte.qiniudn.com/20150426_2.jpg)

