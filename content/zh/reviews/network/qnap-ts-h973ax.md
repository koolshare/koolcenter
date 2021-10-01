---
typora-root-url: ../../../..
typora-copy-images-to: ../../../../article/image
title: "QNAP 威联通 TS-h973ax 九盘位 NAS 网络存储 开箱评测"
linkTitle: "qnap-ts-h973ax-nas-9"
date: 2021-09-18
author: "夜半点灯"
coverImg: "/article/reviews/network/qnap-ts-h973ax/ts-h973ax.jpg"
tags: ["nas", "qnap", "威联通"]
categories: ["评测"]
description: >
  TS-h973AX搭载AMD Ryzen V1500B四核心处理器，内建10GbE与2.5GbE高速网络端口，混合式的硬盘配置提供5个3.5英寸SATA 6Gbps硬盘槽、2个2.5英寸U.2 NVMe SSD专用端口 (Slot 1 & 2 同时支持U.2 NVMe或SATA SSD) 与2个2.5英寸SATA 6Gbps SSD专用端口，可启用SSD快取大幅提升IOPS效能以满足密集存取应用需求。
---

## 前言  
  
盘位：5个3.5寸盘位，4个2.5寸盘位，其中S1槽和S2槽支持U.2 NVMe SSD或者SATA SSD  
SoC：AMD Ryzen V1500B，拥有16条PCIe3.0，14nm工艺，12-25W TDP，四核心八线程，主频为2.2GHz。没有集成GPU  
2.5GbE芯片：Intel i225V，支持速率2.5G/1G/100Mbps  
10GbE芯片：Marvell AQC107，支持速率10G/5G/2.5G/1G/100Mbps  
内存：单根Transcend 8GB DDR4 2666 SO-DIMM，最高支持扩展至双通道64GB内存  
FLASH：5GB，用于存放采用ZFS文件系统的QuTS hero操作系统  
PCIe转SATA芯片：ASM1164和ASM1166，其中ASM1164负责S1—S4槽四个2.5寸SATA硬盘，ASM1166负责1—5槽五个3.5寸SATA硬盘  
U.2：当S1槽和S2槽使用U.2 NVMe SSD时，可以不经过ASM1164，直通SoC  
  
![](https://image.koolcenter.com/attachment/forum/202105/10/211845kifh3iif0zfsvyyv.png)

  
▲TS-h973ax芯片拓扑图  
  
![](https://image.koolcenter.com/attachment/forum/202105/11/150625zsrou4ccrcc9cj4q.jpg)


  
▲TS-h973AX搭载AMD Ryzen V1500B四核心处理器，内建10GbE与2.5GbE高速网络端口，混合式的硬盘配置提供5个3.5英寸SATA 6Gbps硬盘槽、2个2.5英寸U.2 NVMe SSD专用端口 (Slot 1 & 2 同时支持U.2 NVMe或SATA SSD) 与2个2.5英寸SATA 6Gbps SSD专用端口，可启用SSD快取大幅提升IOPS效能以满足密集存取应用需求  
  
![](https://image.koolcenter.com/attachment/forum/202105/11/214438j5m6u7zy5uv1f516.png)


  
▲产品规格  
  
  
## 开箱  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM5ODQ1fGMyMTI2MzMyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲TS-h973ax采用牛皮纸盒子包装，QNAP一贯的风格。正面张贴了NAS的型号和规格  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM5ODQ2fDAzMTdjNTY0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲包装盒内填充有泡棉，上层是附件和说明书，下层固定在泡棉中的是TS-h973ax NAS本体  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM5ODUwfGRhOWYxZjg0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲电源适配器采用12V 20A的输出规格  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM5ODQ4fDY2OWE5MjdhfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲国标电源线一根  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM5ODQ5fGJmY2RlNWY4fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲蓝色CAT6A屏蔽网线一根  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM5ODQ3fGJiNWRiNmI2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲全家福一张。分别是TS-h973ax NAS、PWR-ADAPTER-120W-A01电源适配器、电源线一根、网线一根、快速安装手册、32颗十字螺丝 (适合3.5寸硬盘) 、24颗十字螺丝 (适合2.5寸硬盘)、2个硬盘槽钥匙  
  
  
## 外观  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTM4fDIwMzUwNjU2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲TS-h973ax正面有9个盘位，5个3.5寸硬盘位和4个2.5寸硬盘槽，每个硬盘槽都带有锁止旋钮，可以使用附赠的硬盘槽钥匙对其进行操作。NAS尺寸（高x宽x深）为182.65×224.6×224.1mm  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTM5fDBhMTY4NGQyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲左侧从上往下分别是电源按钮，复制按钮和一个USB 3.2 Gen 2 10Gbps Type-A接口。使用时，将U盘插入USB 3.2接口，再按一下复制按钮，就可以将U盘中的数据上传到NAS中，非常方便  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTQwfDdlZDdiZmY4fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲侧面和留有散热孔，有利于NAS的散热  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTQxfGRkNGUzZTVifDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲顶部贴有云钥安装的教程，右下角标识了这台NAS的型号，以及内置的AMD Ryzen V1500B四核CPU  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTQyfGYxYTdhNTEzfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲底部铭牌  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTQzfDU4ZWE5NGIyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲背部IO接口一览  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTQ1fDU0MThlOTRlfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
A. USB 3.2 Gen 2 Type-C端口（10Gbps）  
B. USB 3.2 Gen 2 Type-A端口（10Gbps）  
C. 2.5GbE端口 x2  
D. 10GbE端口  
E. 重置按钮  
F. 电源输入插孔  
G. Kensington 安全锁孔  
H. 14cm风扇  
  
  
## 拆解  
  
TODO for video
  
  
## 硬盘  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMTk5fDYxZmM3Yzg2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲测试使用HDD是西数WD4003FFBX 4TB，属于WD Red Pro系列，SSD是西数的SA500 500GB  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjAwfDE1NTQ1NzYxfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲WD Red Pro专为处理24×7全天候环境中的高强度工作负载而设计，是存档和共享以及在扩展操作系统（例如ZFS或其他文件系统）上进行 RAID 阵列重建的理想选择  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjAxfDUxMGM0YTczfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲西数WD4003FFBX 4TB，采用CMR技术，7200RPM，缓存是256MB  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjAyfDlmMzk3NWI5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲背面一览。PCB板通过螺丝固定在盘体上  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjAzfDI5MzYxZmQ2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲拆下PCB主板，PCB主板与盘体电路采用公母座互联，之间有一层泡棉作为缓冲  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjA0fDhiNzg3ODllfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲PCB主板正面一览。NT5CC128M16IP-DI，DRAM缓存，大小为256MB，来自南亚；主控为TTT3KR3310，制造厂商是AVAGO；PCB左下方和右上方各有一颗RV传感器  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjA2fGU4MThmZDFlfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲为TS-h973ax选择的SATA SSD是WD Red SA500 500GB  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjA3fDkzOGMwZjBifDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲WD Red SA500 500GB SATA SSD具有卓越的耐久度，可处理NAS系统所需的繁重读写负载，能带来24×7全天候运行环境所需的可靠性  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNjI3fGZkYjBhMTQyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲U.2 NVMe SSD选用的是Intel P4420 7.68T  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMTEwfGQ3ZDJjNzZhfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲如果手头没有U.2 NVMe SSD的话可以使用QNAP的QDA-UMP（[官网链接](https://www.qnap.com.cn/zh-cn/product/qda-ump)）转接盒来实现，QDA-UMP 转接盒可容纳1个M.2 PCIe 3.0 x4 NVMe SSD，并安装于 2.5寸SFF-8639接口U.2 PCIe 3.0 x4 NVMe固态硬盘槽中  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwMjA1fDY3NDNjYjVifDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲将硬盘装上TS-h973ax，由于NAS系统要一直保持运行，因此可靠的硬盘至关重要  
  
  
## 固件  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMjM1fGJlYzA5YzhjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲TS-h973ax支持安装QTS和QTS Hero系统，在NAS没有安装硬盘启动时，在向导页面可以选择  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDIyfGQwOGVjZWU3fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QTS和QTS Hero系统之间的区别  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMzEyfGQ3NzRmOGU4fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲控制台中可以很清晰的看到当前的系统版本  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMzY3fGNmYjIzYjhkfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMzY1fGJjNTI3ODRhfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMzY2fDU1NTk0OTQxfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲储存空间——磁盘中可以查看当前安装的硬盘信息  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDIzfDBjZmU5OTZkfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QTS Hero系统采用了ZFS文件系统，存储池这边只能创建存储池，无法新加卷了  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxMzY5fDM1MzU0YTljfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
创建储存池向导中创建RAID类型，这里多出来两个新的RAID 模式——Triple Mirror 和 RAID-TP  
  
由于文件系统不同，所以 RAID 类型其实也是有所变化的  
RAID 0 : 在ZFS存储池中，称为Stripe  
RAID 1：在ZFS存储池中，称为Mirror  
RAID 5：在ZFS存储池中，称为RAID Z1（RAID Z是ZFS提供的数据冗余方式，ZFS提供三种冗余级别，称为RAID Z，其中RAID Z之后的数字表示每个存储池可丢失多少个磁盘而不丢失数据）  
RAID 6：在ZFS存储池中，称为RAID Z2  
RAID-TP：在ZFS存储池中，称为RAID Z3（是ZFS文件系统独有的，三重奇偶校验，当至少有五个磁盘可用时，可以选择RAID-TP。它可针对三个磁盘出现故障提供保护，RAID-TP提供的磁盘故障保护能力高于普通的RAID 6）  
Triple Mirror：牺牲总存储空间的三分之二。当选定磁盘数是三的倍数时，可以选择Triple Mirror 。在每个由三个磁盘构成的组中﹐每个磁盘所包含的数据均相同。您将失去总存储空间的三分之二﹐以换取极佳的磁盘故障保护能力  
  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDI0fDVhZjc0M2Y4fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲ZFS文件系统下的RAID 0，硬盘间是一个条带化（Stripe）关系，不再是最小磁盘容量 X 磁盘数量  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDI4fDA1NGJiNDMzfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲重复数据删除是一种用于删除重复数据的技术。重复数据删除减少了存储文件所需的空间，减少文件传输的体积。在线数据重复删除需至少16 GB内存，并且这个数据重复删除是实时的  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDI5fDRiZTc1NDMwfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲创建共享文件夹  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDMwfDQyZWZlZDNmfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲ZFS文件系统下的共享文件夹容量最大可以达到1PB  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDMxfGRjOGZjZDhjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲由于我手里这台TS-h973ax只配备的8GB内存，所以重复数据删除功能不能使用，这里仅使用压缩功能（让大档变小档，节省存储空间占用）  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDMzfDE5MjFjNTlhfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲对共享文件夹进行管理  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDM0fGM3OWM4YWI2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲ZIL（Copy-on-Write）同步I/O模式有标准、始终和从不三种模式，这里推荐使用标准模式。ZIL同步I/O即使断电恢复后服务也能继续。QuTS hero系统的压缩系统默认配置为LZ4压缩（LZ4 是一种无损数据压缩算法，可提供极快的压缩和解压缩速度，是商用领域中所需100 MB/s 以上的高速传输存储里，能够提供低延迟、高IO量的压缩选择）  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDM1fDFkNWM4OGRjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE口将文件上传到共享文件夹，传输速度在800MB/s左右，因为要同步进行压缩，这个速度还是不错的  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQxNDM3fGRhYTkzOWUzfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲数据压缩后，占用空间减少  
  
  
## 性能测试  
  
**1\. 4块WD4003FFBX 4TB组建RAID 5**  
  

**hdd 2.5写.png** _(30.73 KB, 下载次数: 46)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQ0fDNlNTY1ZWU3fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在276MB/s左右  
  

**hdd 2.5读.png** _(30.59 KB, 下载次数: 45)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQzfDg4OTE2NDY2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在280MB/s左右  
  

**2.5Gbe cdm.png** _(564.19 KB, 下载次数: 48)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQ1fGUxYWI1ODY1fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用2.5GbE端口的CrystalDiskMark测试  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQ2fDU3MDVhMWIwfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在798MB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQ3fDA0ZDdlMjc5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在1.09GB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQ4fDEyMjg3Yzk5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用10GbE端口的CrystalDiskMark测试  
  
  
**2\. 4块WD4003FFBX 4TB组建RAID 5 + 2块SA500 500GB组建RAID 1作为读写缓存**  
  

**hdd+sata ssd 2.5写.png** _(30.44 KB, 下载次数: 44)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODQ5fDM2NGEzYmQ0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在244MB/s左右  
  

**hdd+sata ssd 2.5读.png** _(30.51 KB, 下载次数: 43)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODUwfGJjYTBhZWQyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在282MB/s左右  
  

**2.5Gbe hdd+SATA ssd cdm.png** _(563.24 KB, 下载次数: 45)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODUxfGFlYjY5ZmM5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用2.5GbE端口的CrystalDiskMark测试  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODUyfGVjNThkOWRkfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在245MB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODUzfDhjODkxNTEwfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在1.08GB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODU0fDgzOThmYTg2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用10GbE端口的CrystalDiskMark测试  
  
  
**3\. 4块WD4003FFBX 4TB组建RAID 5 + 2块Intel P4420 7.68T组建RAID 1作为读写缓存**  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODU1fDU0OGMxZjIxfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲本次评测的TS-h973ax搭载的是8GB内存，提示内存容量不够，无法测试。如果是32GB版本，就不会出现这种问题  
  
  
**4\. 2块Intel P4420 7.68T组建RAID 1**  
  

**2.5GbE Nvme ssd 写.png** _(30.7 KB, 下载次数: 43)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODU2fDczMWRiYWY5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在283MB/s左右  
  

**2.5GbE Nvme ssd 读.png** _(30.78 KB, 下载次数: 43)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODU3fGRkMzA0ZWNjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在279MB/s左右  
  

**2.5GbE Nvme ssd cdm.png** _(563.37 KB, 下载次数: 44)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODU4fDhlMWU5YTI0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用2.5GbE端口的CrystalDiskMark测试  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODU5fGVjYmNiM2IxfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在959MB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODYwfGQ4YmYxY2JifDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在1.08GB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODYxfDFjYzg3ZDczfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用10GbE端口的CrystalDiskMark测试  
  
  
**5\. 2块SA500 500G组建RAID 1**  
  

**2.5GbE sata ssd 写.png** _(30.81 KB, 下载次数: 44)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODYyfDdhODdkZTM1fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在283MB/s左右  
  

**2.5GbE sata ssd 读.png** _(30.67 KB, 下载次数: 42)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODYzfDgyZDMzMjM5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过2.5GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在280MB/s左右  
  

**2.5GbE SATA ssd cdm.png** _(566.52 KB, 下载次数: 45)_

![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODY0fDAxYWMzMzFjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用2.5GbE端口的CrystalDiskMark测试  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODY2fGM4YzYyOGUyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口向NAS中上传文档，此时TS-h973ax的写入速度在257MB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODY3fGY3YzNiMzk4fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲通过10GbE端口从NAS中取回文档，此时TS-h973ax的读取速度在1.09GB/s左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODY4fDQ0NDBiNjBlfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲挂载ISCSI储存后，使用10GbE端口的CrystalDiskMark测试  
  
  
## 功耗测试  
  
测试使用4块WD4003FFBX 4TB，2块WD SA500 500GB和两块Intel P4420 7.68T  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwNzI3fDcyOWZhZDI2fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QNAP TS-h973ax休眠时功耗为18.5W左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwNzI4fDEzOTk0MmYzfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QNAP TS-h973ax使用2.5GbE端口正常运行时功耗为52.7W左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwNzI5fDc3NzY3OTlkfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QNAP TS-h973ax使用2.5GbE端口上传文档时功耗为70.7W左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwNzMxfDY2NDI3ZjE5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QNAP TS-h973ax使用10GbE端口正常运行时功耗为55.1W左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwNzMwfDRkYTU0ZmJifDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲QNAP TS-h973ax使用10GbE端口上传文档时功耗为74.4W左右  
  
  
## 温度测试  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODAyfDMyMWIyMDcyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲环境温度在25.9度左右，湿度在74.1%左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODAxfGEwMDI0ZTQ0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲NAS运行1个小时左右，NAS风扇策略为智能常态  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODA1fDFhYTZjNjg1fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲此时四块HDD和四块SSD的温度，CPU温度以及系统温度一览  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODAzfGQxMjNmMTc5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲SSD 3的测得温度在31.5度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODA0fDI3NGVhZDk0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲SSD 4的测得温度在33度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODA2fGIyN2E0YTcyfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲SSD 1的测得温度在43.8度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODA3fDFiMTM0OTc4fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲SSD 2的测得温度在44.2度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODA4fGRkZGNkMDk3fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲HDD 4的测得温度在37.7度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODA5fDU0NjQyZmRjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲HDD 3的测得温度在38度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODEwfDI2ODg0YTdifDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲HDD 2的测得温度在38.1度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODExfDg1YjExMmE1fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲HDD 1的测得温度在40度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODEyfDE0NGU4OWNjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲CPU散热片测得温度在50.7度左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODEzfGRmNjgwNGE3fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲此时电源适配器温度在38度左右  
  
  
## 噪音测试  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODczfGUyMzRjOGE0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲环境噪音在35.7dB左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODc0fDY3MzZlNWRmfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲系统风扇转速设为1%时，NAS噪音为42.6dB左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODc1fGVkYWUwNGE5fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲系统风扇转速设为25%时，NAS噪音为51.9dB左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODc2fGQ2NzUzNzExfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲系统风扇转速设为50%时，NAS噪音为57.5dB左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODc3fDc1MDg1Y2Y0fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲系统风扇转速设为75%时，NAS噪音为61.9dB左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODc4fDk1NThkZjdjfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲系统风扇转速设为100%时，NAS噪音为66.9dB左右  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODc5fDEzYjQ0N2IzfDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲NAS正常作业时，噪音为43.1dB左右  
  
  
## 总结  
  


![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDQwODgwfGYwZTQyYTM3fDE2MzE5MzQ5ODN8MjM4MHwxOTQ5Nzk%3D&nothumb=yes)


  
▲TS-h973ax延续了QNAP 9盘位NAS的经典外形设计，并对硬盘槽进行了重新设计，带来了更稳固的锁止方式。TS-h973ax搭载的QTS Hero系统整合了强大的128位ZFS文件系统，集结超灵活容量管理、完善数据保护机制，以及效能优化等优势，更能适应数据量日益庞大、复杂的商务关键应用。内置的2个2.5GbE和1个10GbE网络端口，可以充分满足用户对大量文件存取、备份和复原等高带宽作业的需求。无论是文件服务器、虚拟服务器、影音编辑协作、以及文件备份及异地备援等应用，TS-h973AX皆能完美胜任
