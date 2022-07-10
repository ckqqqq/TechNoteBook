课程名称： 云计算技术

项目名称： Opentack部署实验

项目完成人

姓名：\_\_\_陈可淇\_\_\_\_\_ 学号：\_\_\_2019211955\_\_\_\_\_

姓名：\_\_\_\_\_\_\_\_ 学号：\_\_\_\_\_\_\_\_

指导教师：\_\_\_\_\_\_\_\_崔毅东\_\_\_\_\_\_\_\_\_\_

日 期： 2022 年 3 月 27 日

# 目录 {#目录 .TOC-Heading}

[1. 实验概述 3](#实验概述)

[1.1. 实验目的 3](#实验目的)

[1.2. 实验内容 3](#实验内容)

[1.3. 实验环境 3](#实验环境)

[1.3.1. 硬件环境 3](#硬件环境)

[1.3.2. 网络环境 3](#网络环境)

[1.3.3. 软件环境 3](#软件环境)

[1.4. 实验结果 4](#实验结果)

[2. 实验方案 5](#实验方案)

[2.1. 总体方案设计 5](#总体方案设计)

[3. 实验结果 6](#实验结果-1)

[3.1. 在VMware中安装Ubuntu20.04.04 6](#在vmware中安装ubuntu20.04.04)

[3.1.1. Ubuntu版本 6](#ubuntu版本)

[3.1.2. 资源配置 7](#资源配置)

[3.1.3. 资源配置 7](#资源配置-1)

[3.2. 安装包管理工具Snap 7](#安装包管理工具snap)

[3.3. 按照Ubuntu官网教程安装MicroStack版本
8](#按照ubuntu官网教程安装microstack版本)

[3.3.1. 安装microstack---beta版本 8](#安装microstackbeta版本)

[3.3.2. Microstack配置文件 8](#microstack配置文件)

[3.3.3. 测试Microstack基本命令获取基本信息
9](#测试microstack基本命令获取基本信息)

[3.3.4. 从web端进入管理界面 9](#从web端进入管理界面)

[3.4. 在Openstack中创建虚拟机实例 11](#在openstack中创建虚拟机实例)

[3.5. 在Openstack中创建存储卷 12](#在openstack中创建存储卷)

[3.6. 在Openstack中测试其他功能 13](#在openstack中测试其他功能)

[4. 问题及调试过程 14](#问题及调试过程)

[4.1. 问题1：openstack内存/磁盘分配不足导致一系列问题
14](#问题1openstack内存磁盘分配不足导致一系列问题)

[4.2. 问题2：snap安装速度很慢 15](#问题2snap安装速度很慢)

[4.3. 问题3：microstack.-beta 版本安装太慢，即使设置代理后安装速度也太慢
15](#问题3microstack.-beta-版本安装太慢即使设置代理后安装速度也太慢)

[4.4. 问题4：在init时出现错误 15](#问题4在init时出现错误)

[4.5. 问题5：无法从web界面访问程序入口
16](#问题5无法从web界面访问程序入口)

[4.6. 问题6：HTTP400 17](#问题6http400)

[4.7. 问题7：gitclone失败 18](#问题7gitclone失败)

[5. 实验心得 18](#实验心得)

# 实验概述

## 实验目的

学习如何安装部署使用开源Iaas平台，了解如何部署开源IaaS系统。提升实践能力和工程能力，总结部署经验和教训。

## 实验内容

在Linux上运行开源Iaas平台，部署虚拟机。

+------+---------------------------+----------+------------+
|      | 任务说明                  | 负责人   | 工作量比例 |
+======+===========================+==========+============+
| 1.   | 选择Ubuntu环境(建议20.04) | 独自完成 |            |
+------+---------------------------+----------+------------+
| 2.   | 安装/更新包管理工具       |          |            |
+------+---------------------------+----------+------------+
| 3.   | 下载Microstack/Openstack  |          |            |
+------+---------------------------+----------+------------+
| 4.   | 配置环境                  |          |            |
+------+---------------------------+----------+------------+
| 5.   | 试运行Openstack           |          |            |
+------+---------------------------+----------+------------+
| 6.   | 试创建实例                |          |            |
+------+---------------------------+----------+------------+
| 7.   |                           |          |            |
+------+---------------------------+----------+------------+

## 实验环境

### 硬件环境

x86笔记本电脑，Intel Core i5，NVIDIA GeForce MX150，50GB RAM

树莓派3

### 网络环境

校园网WiFi环境

### 软件环境

VMware+Ubuntu 20.04.4 LTS服务器版

阿里云服务器Ubuntu18.04 LTS服务器版

树莓派Ubuntu16.04 LTS

XShell XFTP Xmanager等远程ssh工具

## 实验结果

一共尝试以下平台和Ubuntu版本

+------------------------------+-------------------+------+-------------------------+
| 软件平台                     | IaaS平台          | 结果 | 失败原因                |
| 阿里云ECS服务器(ubuntu18.04) | Openstack         | 失败 | 资源不足+阿里云底层实现 |
+------------------------------+-------------------+------+-------------------------+
| 树莓派(ubuntu16.04)          | Openstack         | 失败 | 内存不足+版本过老       |
+------------------------------+-------------------+------+-------------------------+
| WMware(ubuntu20.04)          | Microstack        | 成功 |                         |
|                              |                   |      |                         |
|                              | （内含openstack） |      |                         |
+------------------------------+-------------------+------+-------------------------+
| WMware(ubuntu20.04)          | Openstack         | 成功 |                         |
+------------------------------+-------------------+------+-------------------------+

Web 端访问

![](openstack文档的图片\media\image1.png){width="5.9944444444444445in"
height="2.8381944444444445in"}

![](openstack文档的图片\media\image2.png){width="6.0in"
height="3.3291666666666666in"}

创建虚拟机和挂载volume存储

![](openstack文档的图片\media\image3.png){width="6.0in"
height="2.890972222222222in"}

![](openstack文档的图片\media\image4.png){width="6.0in"
height="3.314583333333333in"}

# 实验方案

## 总体方案设计

![](openstack文档的图片\media\image5.png){width="1.3956583552055992in"
height="6.280464785651794in"}

在ubuntu20.04上安装microstack虚拟机流程

# 实验结果

## 在VMware中安装Ubuntu20.04.04

从清华镜像源下载 ubuntu-20.04.1-Live-server
-amd64.iso后，新建空的虚拟机，配置CD/DVD为所下载的ISO文件，分配内存为4GB，磁盘为50GB，配置源为清华源，处理器为4，如下图。

### Ubuntu版本

![](openstack文档的图片\media\image6.png){width="6.0in"
height="0.2465277777777778in"}

### 资源配置

![](openstack文档的图片\media\image7.png){width="3.0933628608923884in"
height="4.166146106736658in"}

### 资源配置

安装系统，安装好系统后安装并设置ssh

![](openstack文档的图片\media\image8.png){width="6.0in"
height="1.3611111111111112in"}

此处碰到问题3：openstack内存/磁盘分配不足将会导致openstack出现错误，所以虚拟机安装时要分配足够的磁盘

## 安装包管理工具Snap

Snap是包管理工具，其比ubunt自带的apt更智能，资源更多

![](openstack文档的图片\media\image9.png){width="6.0in"
height="2.7729166666666667in"}

此处碰到问题2：snap下载过慢解决方法为安装snap代理

![](openstack文档的图片\media\image10.png){width="6.0in"
height="1.520138888888889in"}

## 按照Ubuntu官网教程安装MicroStack版本

参考：https://ubuntu.com/tutorials/install-openstack-on-your-workstation-and-launch-your-first-instance\#2-install-openstack

按照上述网站内容进行安装

### 安装microstack---beta版本

![](openstack文档的图片\media\image11.png){width="6.0in"
height="1.7444444444444445in"}

此处碰到问题2 ：解决方法见附录

### Microstack配置文件

MicroStack需要初始化，以便配置网络和数据库

![](openstack文档的图片\media\image12.png){width="6.0in"
height="3.0729166666666665in"}

此处碰到问题4：解决方法见附录

### 测试Microstack基本命令获取基本信息

![](openstack文档的图片\media\image13.png){width="6.0in"
height="1.667361111111111in"}

### 从web端进入管理界面

使用Web端管理界面可以配置VMware防火墙于主机上使用，也可以配置apche2+W3M使用终端访问，也可以通过Xmanager访问终端图形界面.

![](openstack文档的图片\media\image14.png){width="6.0in"
height="2.310416666666667in"}

此处碰到问题5：解决方法见附录

Web端访问

![](openstack文档的图片\media\image15.png){width="6.0in"
height="3.129166666666667in"}

![](openstack文档的图片\media\image2.png){width="6.0in"
height="3.33125in"}

## 在Openstack中创建虚拟机实例

使用如下命令在openstack中创建虚拟机实例

![](openstack文档的图片\media\image16.png){width="6.0in"
height="3.15in"}

![](openstack文档的图片\media\image3.png){width="6.0in"
height="2.890972222222222in"}

## 在Openstack中创建存储卷

使用如下命令在openstack 中创建并挂载存储卷

此处遇到了问题6：端口错误 解决方法见附录

![](openstack文档的图片\media\image17.png){width="6.0in"
height="0.75in"}

![](openstack文档的图片\media\image4.png){width="6.0in"
height="3.314583333333333in"}

可见下图中my-new-volum卷创建成功，其大小为1GB，
状态为可用，（之前创建失败的为Volume1卷，创建失败的原因可见附录问题6）

![](openstack文档的图片\media\image18.png){width="6.0in"
height="0.9722222222222222in"}

如何获取 Image ID？

![](openstack文档的图片\media\image19.png){width="6.0in"
height="1.26875in"}

如何获取availabl zone

![](openstack文档的图片\media\image20.png){width="6.0in"
height="1.2958333333333334in"}

## 在Openstack中测试其他功能

该命令用于陈列microstack网络信息，可以看到虚拟机网络的ID，用户名和子网信息

![](openstack文档的图片\media\image21.png){width="6.0in"
height="2.6222222222222222in"}

该命令用于陈列openstack中server信息

![](openstack文档的图片\media\image22.png){width="6.0in"
height="1.0958333333333334in"}

该命令用于获得test实例的基本信息

![](openstack文档的图片\media\image23.png){width="4.902597331583552in"
height="3.2519422572178476in"}

# 问题及调试过程

## 问题1：openstack内存/磁盘分配不足导致一系列问题

此处碰到问题：openstack内存/磁盘分配不足将会导致openstack出现错误，所以虚拟机安装时要分配足够的磁盘。如果资源不足将会导致分配存储时出现错误，或者出现问题四所见报错。

![](openstack文档的图片\media\image24.png){width="6.0in"
height="1.125in"}

## 问题2：snap安装速度很慢

此处碰到问题二：snap下载过慢

解决方法：安装snap代理

![](openstack文档的图片\media\image10.png){width="6.0in"
height="1.520138888888889in"}

## 问题3：microstack.-beta 版本安装太慢，即使设置代理后安装速度也太慢

问题原因：beta版本在属于较新的版本，下载资源较少，可以通过先下载-edge版本，再升级为-beta版本

## 问题4：在init时出现错误

![](openstack文档的图片\media\image12.png){width="6.0in"
height="3.0729166666666665in"}

如果出现如下python错误：

需要检查：

1.  足够的内存空间和较新的Ubuntu版本（16.04始终会出现如下错误）

2.  使用以下命令彻底删除microstack并且重传（版本冲突）

3.  关闭VPN，防止因为IE代理错误导致安装失败

sudo apt-get \--purge remove XXX \--purge

![](openstack文档的图片\media\image25.png){width="6.0in"
height="2.067361111111111in"}

## 问题5：无法从web界面访问程序入口

1 设置VMware防火墙,开放5000端口或者下载apche+live server浏览器

2 检查网址 尝试http://10.20.20.1/和<https://10.20.20.1/>

![](openstack文档的图片\media\image26.png){width="6.0in"
height="1.5131944444444445in"}

## 问题6：HTTP400

![](openstack文档的图片\media\image27.png){width="6.0in"
height="0.5305555555555556in"}

HTTP400错误

原因 clinder错误

解决方法重新初始化clinder

![](openstack文档的图片\media\image28.png){width="6.0in"
height="3.1798611111111112in"}

![](openstack文档的图片\media\image29.png){width="6.0in"
height="1.2597222222222222in"}

重新挂载

![](openstack文档的图片\media\image30.png){width="6.0in"
height="2.145138888888889in"}

可见初始化前volume1出现错误，重新初始化后状态为Available

![](openstack文档的图片\media\image31.png){width="6.0in"
height="0.9930555555555556in"}

## 问题7：gitclone失败

原因：github今年年初被墙了

![](openstack文档的图片\media\image32.png){width="6.0in"
height="0.95625in"}

解决方法

在站点查询github的国内服务器地址,在host文件中修改dns定向。

["www.github.com"A记录/cname检测结果\--Dns查询\|dns查询\--站长工具
(chinaz.com)](https://tool.chinaz.com/dns?type=1&host=www.github.com&ip=)

# 实验心得

官方教程属实不给力，很多意外情况要自己摸索Orz。

本次实验过程过几天会放在blog(CSDN:
ckqqqqq)上，希望不会有人再踩这些奇奇怪怪的坑了。

此外除了在Ubuntu20.04live
server上安装microstack外，我还在以下平台尝试过安装openstack。具体情况如下。

其中在Ubuntu20.04上安装openstack（非micrstack）时，如有用到gitclone操作，需要修改host,可见问题7。

总而言之，安装openstack还是挺锻炼人的

一共尝试以下平台和Ubuntu版本

  软件平台                       IaaS平台     结果   失败原因
------------------------------ ------------ ------ -------------------------
  阿里云ECS服务器(ubuntu18.04)   Openstack    失败   资源不足+阿里云底层实现
  树莓派(ubuntu16.04)            Openstack    失败   内存不足+版本过老
  WMware(ubuntu20.04)            Microstack   成功   
  WMware(ubuntu20.04)            Openstack    成功   
