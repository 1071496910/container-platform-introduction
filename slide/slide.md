title: 容器平台介绍
speaker: 和盼晨
transition: slide3
theme: moon
usemathjax: yes

[slide]

# 容器平台介绍
<small>作者：和盼晨</small>

[slide]
# 目录

<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:0 orderedList:0 -->

- [容器平台](#2)
	- [特性](#3)
	- [docker介绍](#4)
		- [什么是容器](#5)
			- [linux命名空间](#6)
		- [最简单的container](#7)
		- [kubernetes](#8)
	- [平台架构](10)
		- [k8s组件](#11)
		- [calico](#12)
			- [calico 组件](#13)
			- [calico 架构](#14)
		- [monitor](#15)
		- [monitor(新)](#16)
		- [日志系统](#17)
	- [发布系统](#18)

<!-- /TOC -->

[slide]
# 容器平台
<small> 基于docker和kubernetes的paas平台</small>

[slide]
## 特性
* 提高资源使用率
* 环境一致
* 自动扩缩容
* 自动故障恢复
* 自动滚动升级
* 自动服务发现

[slide]
## docker介绍

[slide]
### 什么是容器
![](/assets/markdown-img-paste-20180706103022546.png)

[slide]
#### linux命名空间
![](/assets/markdown-img-paste-20180706103607527.png)

[slide]
### 最简单的container
![](/assets/markdown-img-paste-20180706115626337.png)

![](/assets/container-sh.gif)

[slide]
### kubernetes
![](/assets/markdown-img-paste-20180706104939784.png)

[slide]
- pod
  - 一组容器，同一个Pod里的容器共享同一个网络命名空间，可以使用localhost互相通信。k8s调度的基本单位。</small>
- service
  - Service是定义一系列Pod以及访问这些Pod的策略的一层抽象。Service通过Label找到Pod组。

[slide]
## 平台架构
![](/assets/markdown-img-paste-20180705204537341.png)

[slide]
### k8s组件
![](/assets/markdown-img-paste-20180705204839726.png)

[slide]
### calico

[slide]
#### calico 组件
![](/assets/markdown-img-paste-2018070520500947.png)

[slide]
#### calico 架构
![](/assets/markdown-img-paste-20180705204927536.png)

[slide]
### monitor
![](/assets/markdown-img-paste-2018070520520887.png)

[slide]
### monitor(新)
![](/assets/markdown-img-paste-20180705205258708.png)

[slide]
### 日志系统
![](/assets/markdown-img-paste-20180705210420582.png)

[slide]
## 发布系统
----
http://d.zcontainer.meizu.com:8421
