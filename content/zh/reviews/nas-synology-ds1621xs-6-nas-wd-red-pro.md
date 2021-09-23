
---
title: "专业桌面NAS，Synology DS1621xs+ 6盘位NAS搭配WD RED Pro 拆解评测"
linkTitle: "专业桌面NAS，Synology DS1621xs+ 6盘位NAS搭配WD RED Pro 拆解评测"
author: "pufer"
coverImg: "https://image.koolcenter.com/attachment/forum/202102/06/201231e17a7yza7liivhym.jpg"
date: 2021-07-06 16:49:08
tags: ["TODO"]
categories: ["TODO"]
description: >
  TODO
---

_本帖最后由 pufer 于 2021-2-10 10:28 编辑_

**【前言】**

3年前我们第一次评测了群晖xs+/xs系列专业NAS产品，今天我们再一次带来了大家非常关注的群晖专业xs+产品——Synology DS1621xs+。大家都知道xs+/xs代表了群晖桌面最高端的专业系列。

今天评测的产品是Synology DS1621xs+。这台是21年款，6盘位的，最大扩展到16盘位的NAS。

DS1621xs+ 提供了2个千兆口，1个万兆口，万兆口支持2.5G、5G多模式。同时也提供了2个M.2 SSD缓存插槽。

当然PCIe扩展槽依然提供，可以用于安装以太网卡和FC HBA卡。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NzUxfDgzNjhlMzBlfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)




![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI3MDQ0fDYxYzgxOWMwfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**Broadwell-DE**

DS1621xs+的CPU使用了来自Intel的Intel Xeon Processor D-1527，隶属于Broadwell-DE系列产品。这个系列的CPU大家并不是很了解，这里做个介绍。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzE0fDIyODc4Y2IwfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


Broadwell-DE可谓是把我们常见的Broadwell-EP（Intel E5 v4系列）做成了SOC。拥有2-8个核心，14nm工艺，L1数据缓存32KB，指令缓存32KB，L2缓存每核心256KB，L3缓存是每核心1.5MB，这跟Broadwell架构的处理器都是一样的。

内存方面支持双通道的DDR3L和DDR4，这点和服务器等级的Boradwell-EP很像。内存规格支持RDIMM和UDIMM，也就是说支持服务器专用的RECC内存。Broadwell-DE还支持24条PCIe 3.0，8条PCIe 2.0。I/O接口方面支持2个10Gbe万兆Mac，4个USB 3.0，4个USB 2.0，6个SATA 6Gb接口。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzEzfDA0NWZiNGE5fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


Broadwell-DE虽然是个SOC设计，但是我们看到内部架构图，实际上是Broadwell和PCH整合在一起。这样的话，很容易看到24条PCIe 3.0和万兆MAC是由核心IIO直接提供。而SATA接口，8条PCIe 2.0，是由PCH提供，PCH和IIO之间还是通过DMI2.0 x4连接。

**详细规格**



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzE2fDExZDlkODY4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**【开箱】**

专业的机型往往使用了朴素的包装，DS1621xs+依然使用了群晖最经典的牛皮纸包装盒。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTAwfDAxNDdmMjM2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


配件盒里面配备2条网线，1包螺丝，一条电源线以及一套钥匙。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxODk5fGY0OTJkY2U3fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


两本快速上手指南



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTAxfDIwNDNmZWVifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


DS1621xs+保持着群晖6盘位机型的一贯的外形。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTA2fDIyZDNjMGU3fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


DS1621xs+正面6个热插拔盘位。顶部配备了电源，警告指示灯，电源按钮，以及3个网口指示灯。因为DS1621xs+是1个10G、2个1G网口，所以网口指示灯也变为3个，底部有一个USB3.0接口。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTA1fDUzNjczMTVhfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


DS1621xs+背后可以看到2个风扇，也和前几代保持一致。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTA4fGU0NDY2MDFkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


侧面Synology logo的散热孔。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTA3fDczNTRkZmFmfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


下方接口，2个USB3.0，1个万兆口，2个千兆口，2个ESATA扩展柜接口，1个PCIe扩展槽。大家可以注意到万兆口的和千兆口的外观不同。具体原因拆解部分会具体讲述。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTEwfDg5NDUxNzc2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


在DS1621xs+底部有一个内存槽的保护盖，用户升级内存十分方便。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTA5fGU3Nzg2ZDZlfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


内置了一条群晖原厂DDR4 2666 ECC SODIMM内存。DS1621xs+使用了Xeon处理器，推荐使用ECC内存保障系统稳定。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTExfDkyNDhkMGRkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


硬盘插槽依然是热插拔，前面有个锁口。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTEyfGQ4YjE3NmM1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


硬盘托架依然是免螺丝设计。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTEzfGE2ZDA1YzIxfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


安装硬盘后的样子。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTE0fGUyMzdiNjUwfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


拆掉6个硬盘托架后可以看到内部背板，背板使用镂空设计，加强企业级硬盘的散热。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTE2fDFjNjg2YjdlfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


在硬盘槽的侧面有2个M.2 2280 SSD插槽，都是PCIe 3.0 x4满血M.2模式。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTE5fDAzZjdiZmVlfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**【安装PCIe网卡】**

背后拧开6个螺丝后，可以打开DS1621xs+顶盖。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTE3fDhmNTVjMWVjfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


可以看到一侧的DS1621xs+的内置电源



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTE4fGFhNDNiY2Y2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


另外一侧可以看到预留的PCIe 3.0 x8的插槽。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTE1fDFiMmI0MTE1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**Intel Ethernet Network Adapter XXV710**

这次DS1621xs+评测我们首次使用了25G以太网，Intel Ethernet Network Adapter XXV710。测试用的是Intel原厂网卡，采用了牛皮纸包装。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTAyfDAwMmY4ZGFhfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


网卡正面覆盖了黑色散热片，25G不在使用SFP+接口，改为使用SFP28接口。两者外观还是很相似的。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxODk3fGU5YTdjOTdmfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


网卡背面，Intel原厂网卡特有的方位标志



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxODk4fGRmNzE0MzMyfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


网卡安装上NAS后，可以看到DS1621xs+对长网卡的支持还是很不错的。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTAzfGUyYWE5ZmU1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


背后的SFP28 25G光口。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTA0fGIyZWNjYzA1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


DS1621xs+的普通用户拆到这一步就可以了，接下来的部分不建议普通用户自己拆解。

**【拆解】**

首先从电源开始动手，内部电源是1U的定制电源，群晖对线材和接口做了定制。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTIxfDZiN2RjNTBifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


电源是来自台达DPS-250AB，250W 80棕牌认证的电源，满足6盘位NAS的需要。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTIzfGQ3ZTgxNjQyfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


拆除背后的背板。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTIyfDBiOWJhYThkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


可以看到背后的2个风扇，都使用了4Pin PWM调速设计，可以准确的控制风扇。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTIwfDI5OGY5M2JkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


拆除NAS底部的底板。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTI0fDM1NDc5ZWZlfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


可以看到主板。DS1621+使用了4核心的Xeon D-1527，为了更好的散热，这次设计了导风罩，更好的完成散热。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTI1fDEwMjczNzRifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


主板正面有两大块散热片。

大的散热片下面是Intel Xeon D-1527，上面使用散热垫和机箱导热，小的散热片下面是Marvell AQtion AQC107万兆网卡芯片。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTI4fGY3MDUwOTBifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


主板背面，可以看到Xeon D-1527 CPU底部也是做了和底壳的导热加强散热。这次DS1621xs+虽然同样的6盘位，散热做了很大的加强。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTM0fDcwZDg3YTY0fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


接下来详细讲一下主板上的芯片。

[JMicron JMB585](https://www.jmicron.com/products/list/15) PCIe 3.0 x2 to x5 SATA 6Gb/s，5端口SATA控制芯片，负责背后2个ESATA扩展接口和Bay  4-6的三个盘位。Bay 1-3的三个盘位有Xeon D-1527直接提供。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTI2fGZhN2M0YmFjfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


Intel I210 PCIe 2.0 x1 to 1Gb，千兆以太网控制芯片，一共2颗，负责2个千兆网口。这个芯片大家很熟悉了，Intel入门服务器网卡芯片。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTI3fDJlYjNjMWEzfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)




![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTI5fGJmMDI5M2E3fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


[Marvell AQtion AQC107](https://www.marvell.com/content/dam/marvell/en/public-collateral/ethernet-adaptersandcontrollers/marvell-ethernet-controllers-aqtion-aqc107-108-product-brief.pdf)，负责DS1621xs+的万兆网口，拆解时候大力出奇迹，顶盖一起下来了。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTMwfDJiNGE2YmU1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


前面说了DS1621xs+的万兆网口和千兆外观完全不同。因为万兆RJ45接口也是使用了来自Marvell的打包方案，是AQC107芯片推荐的使用方法。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTMzfGU4ZWMxODYzfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


Altera逻辑加密芯片，负责DS1621xs+的底层认证。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTMxfDYzZTNmY2I4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


DS1621xs+的引导DOM盘，出厂安装了DSM6.2的引导。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIxOTMyfDc2YjVjZDc5fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


使用了Intel Xeon D-1527，四核心2.2Ghz设计，支持睿频到2.7Ghz。CPU 6组4x PCIe3.0通道，2组4x组合在一起，成为PCIe Slot 8x插槽。2组4x给2个M.2槽提供支持，所以M.2也是满血性能的。1组4x通过Marvell Aqc107，提供了NAS的万兆接口。最后一组4x，链接了PCIe 3.0 2x的JMicron JMB585，提供了5个SATA接口。其中3个接口负责Bay4-6三个盘尾，2个作为ESATA接口连接扩展柜。

利用SOC中PCH原生提供的3个SATA 6G接口提供3盘位，最后3个盘位使用JMicron JMB585提供。没有使用全部PCH原生SATA，而这么做为了避免当使用6块SATA SSD同时读写时把PCH到CPU之间DMI 2.0 x4通道占满而速度限制。这样3+3的组合可以使得6块sata ssd全部满速。2个千兆网卡使用了Intel I210AT，连接在PCH提供的PCIe 2.0上。USB接口同样也链接在PCH。

3+3的SATA提供方式是由于Intel DMI2.0 x4带宽不足妥协的结果。

最后根据拆解做出的NAS架构图。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDIzNzYzfGJiNWE5MzdifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


在机器散热方面，针对这个4核心CPU群晖也做了优化，比起DS3018xs来说，散热片面积大的增加。同时主板上方和下方都使用了散热垫和机器外壳链接，更好的通过NAS的全金属外壳把热量散发出去。

同时在机器内增加导风罩设计，加大通过CPU的分量加强散热。通过这些方式，DS1621xs+的热量明显比DS3018好。

**【WD HDD】**

xs+/xs机型为群晖高端专业和面向企业的机型，硬盘方面 WD推荐企业盘或者WD Red Pro系列，可以给NAS提供更好的稳定性和吞吐量。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzQwfDZkOTBjZGVkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


本次为DS1621xs+准备的HDD是WD4003FFBX 4TB，属于WD Red Pro系列，采用CMR技术，7200RPM

盘体依然是WD经典红盘样式，但是内部性能大大不同



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzQyfDI5YzFkNTg2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)




![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzQxfDQ0ZDRkZGM1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


在这里简单提一下WD Red、WD Red Plus、WD Red Pro的区别

WD Red系列，2TB—6TB采用SMR技术，5400RPM

WD Red Plus系列，1TB—14TB全系采用CMR技术，5400RPM

WD Red Pro系列，2TB—14TB全系采用CMR技术，7200RPM

Red Pro已经属于准企业级的磁盘了。

WD Red Pro系列NAS盘规格一览



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzE3fDZkMzgwNDc3fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


使用群晖自带磁盘调校来测试磁盘的性能。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2Mjc0fGI4NWMxNDU4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


在NAS的系统中，WD红盘系列会有特殊的固件优化和信息检测，可以在提前预警出磁盘的潜在风险。在DSM7后期会上线合作硬盘的固件更新，合作认证的HDD固件更新会更方便。

**【DSM7】**

目前DSM7还是在公测阶段，DS1621xs+我们也第一时间安装了DSM7的公众测试版本。下面的测试和介绍都会基于DSM7。关于DSM7的全部特性在DSM7正式版上线后会给大家介绍。

在信息中心里可以查看CPU型号、核心数、主频以及NAS当前安装的内存容量等信息



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzUyfGFkZGJjNTJkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


可以看到网卡接口信息。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzUzfDU2ZGQ2ZjI5fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


局域网1是10G内置网口。

局域网2和局域网3是千兆内置网口。

局域网4和局域网5是安装的25G网卡接口。

**存储管理员**

DSM的存储管理员全部重新设计，主页上可以非常清晰的看到磁盘在NAS上的实际位置。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzU0fDRiYjAwYTdmfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


存储池和存储空间的关系更加明确的表示，可以清晰看清两者关系。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzU1fGI3ZGYwYzkzfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


每块磁盘的信息也更加清晰，通过磁盘定位功能，可以夜半点亮磁盘上的指示灯。方便定位寻找故障磁盘。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzU2fDZjN2M5MmU2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


在创建存储空间时候，如果使用的磁盘不在NAS的兼容列表内，会有提示，只是一个提示，不影响用户创建流程

这里使用了2块自己DIY的SSD做演示。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzU3fDNjMzFhNGZjfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


要说明的是在DSM7后

1、磁盘兼容性检查是所有机型都会有的，只是用户一个提示，不影响使用。

2、而硬盘型号的限制，只针对xs+/xs及以上大型企业级机型，家用和小型企业机型不会有限制。

3、现有发售的机型用户目前不会有限制。后续发售的xs+/xs及以上大型企业级机型，有明确说明的才会有限制使用指定的磁盘。

RAID修复这次也新增2个功能

RAID快速修复，在DSM6以前磁盘修复时候需要全盘同步，DSM7支持只同步有数据部分，大大加快磁盘同步的时间。

RAID自动修复，就是当硬盘损坏后安装新硬盘，系统会自动开始修复，不需要人工干预到界面上点击。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzU4fDQzNjRlNDNjfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


同时这次增加自动发现热插入硬盘的数据分区。

DSM7可以发现新插入硬盘上的DSM分区，并且可以直接挂载。当NAS意外故障时候，可以找你朋友用他的NAS读出你的全部数据，也推荐买NAS可以预留盘位。

**Synology Photos**

此次原来的Photo Station和Moments终于合并成一个照片管理APP

Photos去除了Moments被人诟病的每天创建一个文件夹，提供了按时间预览和按文件夹归类预览两个模式。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDI1fDZiNWM3Njg4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)




![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDI2fGIwNWMzYTAyfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


同时在启用共享空间后，可以有一个公共的Photos文件夹，和原来Photo Station达到一样的体验效果。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDI0fDBjZDczY2ZmfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**Synology Drive**

Drive在DSM7.0的变化主要是有用信息更全面。

Drive Server主页增加了外部用户访问最多的文件，可以方便知道文件是否被盗链了。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDM1fGU1M2QxNGNkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


同时增加了历史文件数据库的详细统计。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDM2fDZhNjVmZTZhfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**【性能测试】**

**SAMBA读写测试**

DS1621xs+提供了板载10G接口，同时支持了PCIe扩展，所以这次也首次使用了25Gb以太网来做SAMBA吞吐量性能测试。为了达到最大性能，NAS内安装了6片4TB WD SSD Red Pro，通过RAID 0 的方式组织成存储空间。

测试用的PC

安装了2片网卡

电口网卡为Intel Ethernet Converged Network Adapter X550-T2

光口网卡为Intel Ethernet Network Adapter XXV710-DA2

使用电缆和NAS直接连接。

电口万兆

写入NAS



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDM4fDEzYjZlYzNhfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


从NAS读取



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDM5fDI0Mzc2Zjg2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


光口25G

写入NAS



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDM0fDliZTYyMTFifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


从NAS读取



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDMzfDllOGNjMzE2fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


可以看到DS162xs+的读写速度是非常给力的。

**VMM性能测试**

DS162xs+使用的Xeon D-1527是4核心8线程的规格，在VMM内vCPU可用数量达到了16个之多。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzU5fDZjZGJlZTVhfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


我们在VMM内部署了1台Windows 10，2台Ubuntu（一台Desktop，一台Server）。虚拟机内操作非常流畅。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2MzkzfGZlNmEzNzVjfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


对于DS1621xs+这个性能的机型VMM的使用体验达到了一个非常好的体验。

还是要顺便说一句，如果VMM想要有非常好的体验，请安装支持SR-IOV的网卡，并且开启SR-IOV。这样虚拟机内不需要消耗CPU就能完成数据转发。目前开启SR-IOV成功的只有Intel Ethernet Converged Network Adapter X550-T2，大家认准这个卡。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2Mzk0fDJmNTcwZjIwfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**【SAN存储】**

大家都知道群晖大部分机型都支持IP SAN（iSCSI）。

DSM7开始，原来的iSCSI Manager改名成SAN Manager。没错，从DSM7开始，群晖xs+/xs机型通过安装FC HBA卡的方式可以支持FC SAN。也就是说群晖的NAS可以作为FC存储，给服务器，虚拟化提供存储。也可以和工作站点对点连接，当做剪辑机器的外挂存储。

FC SAN因为对CPU性能，PCIe带宽有要求。也不会对所有机型开放。

目前支持FC SAN的机型：

> UC3200
>
> FS6400，FS3600，FS3400，FS1018，FS2017
>
> SA3600，SA3400
>
> DS1621xs+，RS1619xs+，RS3618xs，DS3018xs，RS18017xs+，RS4017xs+，RS3617RPxs，RS3617xs+，DS3617xs

目前支持的FC HBA卡

> Marvell Qlogic：QLE2690-SR-CK，QLE2692-SR-CK，QLE2670-CK，QLE2672-CK2

安装HBA卡后可以看到卡状态，并且可以挂载存储空间



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2Mzk1fDdkNGFhNmFifDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


工作站用户可以安装FCHBA卡和NAS对接。

Mac用户可以用过Promise SanLink F2实现FC对接



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDE0fDdjMTgxMzlhfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


[https://www.promise.com/Products/SANLink/SANLink3-F2](https://www.promise.com/Products/SANLink/SANLink3-F2)

**【温度测试】**

大家比较关心这个机器跑起来时候的温度和散热情况。

**噪音测试**

环境噪音在38dB左右



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDIyfGRmZTFmOTI4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


静音模式下，DS1621xs+的噪音分贝值在42dB左右



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDIwfGI4ZDI2NjNkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


低温模式下，DS1621xs+的噪音分贝值在48dB左右



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDIxfDZmODBmNGVkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


全速模式下，DS1621xs+的噪音分贝值在75dB左右



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDIzfDI3Mzg1OTNkfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


也就是俗称的NAS起飞了，DS1621xs+在CPU满载情况下也还是会出现NAS起飞现象

**温度测试**

室温在26度左右。



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2NDA0fDQ4MzhkZmU4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


DS1621xs+正常运行4小时左右，CPU温度在52度附近



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2Mzk2fGNjM2M3Y2E4fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


通过计算SHA256命令让CPU满载

1. nohup cat /dev/urandom \| sha256sum &

_复制代码_



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2Mzk3fGExN2E4NDM1fDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


最终CPU温度在64度附近



![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=NDI2Mzk4fGQzOTVhY2UwfDE2MzIzOTA0MDZ8MHwxOTA2Mjk%3D&nothumb=yes)


**【总结】**

曾经DS3018xs是6盘最强NAS，如今地位不保被后浪DS1621xs+轻松超越。这台是目前群晖桌面级NAS的天花板。这机器唯一缺点，可能就是他高昂的价格。如果你预算不是问题，寻找你身边群晖的代理商订货DS1621xs+吧。
