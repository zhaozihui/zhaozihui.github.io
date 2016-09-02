---
layout: post
title: Nexus 原生系统刷机教程
date: 2016-09-02 09:32:24.000000000 +09:00
---

![](https://lh3.googleusercontent.com/ms7mwMf7R0GX-lvCrfFptekdsTSMcKyJeFNtIyIGx-q_W3TnSs_E2zShxAaug75otw)

##### 教程
---
1. 下载官方[刷机包](https://developers.google.com/android/nexus/images)
2. 连接你的手机和电脑
3. 打开开发者模式
4. 打开USB调试
5. 使用adb 命令启动手机的 fastboot模式

	~~~ 
	adb reboot bootloader 
	~~~
6. 解锁你的手机

	~~~ 
	fastboot flashing unlock
	~~~
对于比较旧的版本的手机 使用命令

	~~~ 
	fastboot oem unlock
	~~~
这个时候手机会显示确认画面,确认解锁
7. 打开电脑终端,并解压缩下载的image文件
8. 直行解压缩文件夹中的

	~~~
	flash-all.sh(windows 系统请直行flash-all.bat) 
	~~~
9. 等待刷入结束,system刷入相对速度会慢一些,请耐心等待
10. 刷入结束后 系统自动重启
11. 为了安全,请锁定手机
~~~
fastboot flashing lock
~~~
对于比较旧的版本的手机 使用命令

	~~~ 
	fastboot oem lock
	~~~

新系统刷机完成


[官方rom和刷机教程](https://developers.google.com/android/nexus/images)

~~~ 
https://developers.google.com/android/nexus/images
~~~