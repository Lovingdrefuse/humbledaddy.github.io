---
title: 计算机网络-SAP和OSI
top: false
cover: false
toc: true
mathjax: true
date: 2020-10-20 18:16:40
password:
summary:
tags: 笔记
categories: 计算机网络
---

# OSI 网络体系结构

## OSI

OSI 具有七层协议

> （应用层 表示层 会话层 运输层 网络层 数据链路层）

TCP/IP 具有四层协议

> （应用层 运输层 网络层 网络接口层）

在学习网络体系结构时，折中采用五层协议，也就是把网络接口层拆开为数据链路层和物理层

> （具体应用还是四层协议，没有这么麻烦，）

<<<<<<< Updated upstream
![计算机网络体系结构](<img src="https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/20201021174526.png"/>)
=======
![](https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/20201021174526.png)
>>>>>>> Stashed changes

**只有物理层的连接才是真连接，其他层的连接都是靠软件实现的逻辑上的连接**

 :computer:\- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -:computer:

![数据在各层直接传递](https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/a.png)

## SWP(Service Access Point)服务访问点

1. 服务数据单元 SDU（Service Data Unit）。OSI 模型把相邻层实体间传送信息的数据单元称为服务数据单元，并将（N+1）层与（N）层之间传送信息的服务单元记为（N）SDU。（N）服务数据单元实际上是确保（N）服务传输需要的逻辑单元。

2. 协议数据单元 PDU（Protocol Data Unit）。OSI 模型把对等实体间传送信息的数据单元称为协议数据单元，并将（N）层的协议数据单元记为（N）PDU。（N）PDU 由两部分组成，即（N）用户数据［记为（N）UD］和（N）协议控制信息［记为（N）PCI］。如果某层的协议数据单元只用于控制，则该协议数据单元中的用户数据可省略，此时只有该层的 PCI。

3. 接口数据单元 IDU（Interface Data Unit）。OSI 模型把相邻层实体通过层间服务访问点依次交互信息的数据单元称为接口数据单元，并将（N）层的接口数据单元记为（N）IDU。（N）IDU 也由两部分组成。其中，一部分是（N+1）实体与（N）实体交互的数据，称为接口数据［记为（N）ID］；另一部分是为了协调（N+1）实体与（N）实体的交互操作而附加的控制信息（如服务原语中的某些参数），这些拉制信息称为接口控制信息［记为（N）ICI］。由于接口控制信息只在交互信息通过服务访问点时才起作用，所以，当接口数据单元通过服务访问点后就可以将其取掉。
<<<<<<< Updated upstream
   <img alt="SWP" src="https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/test.png" style="zoom: 67%;" />

## PDU SDU IDU 三者关系

   <img src="https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/test1.png" alt="SDU在实体之间传递" style="zoom: 64%;" />

上课的时候龙崽想了一个比较恰当的比方，最开始的 data(最初的 SD)就是一块洋葱芯 🧅，随着一层一层实体传递，没传递一层就给洋葱芯裹上一层洋葱皮(PCI)🧅，最后到第 0 层也就是物理层的时候就是一个洋葱 🧅，然后通过物理管道，丢雷老母~🧅
=======
   ![](https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/test.png)

## PDU SDU IDU 三者关系

   ![](https://raw.githubusercontent.com/HUMBLEDADDY/ImageHosting/master/img/test1.png)
上课的时候龙崽想了一个比较恰当的比方，最开始的data(最初的SD)就是一块洋葱芯🧅，随着一层一层实体传递，没传递一层就给洋葱芯裹上一层洋葱皮(PCI)🧅，最后到第0层也就是物理层的时候就是一个洋葱🧅，然后通过物理管道，丢雷老母~🧅
>>>>>>> Stashed changes
