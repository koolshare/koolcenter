
---
title: "橙色的性能猛兽——希捷酷玩 FireCuda 530 系列固态盘评测"
linkTitle: "橙色的性能猛兽——希捷酷玩 FireCuda 530 系列固态盘评测"
author: "御剑江湖"
coverImg: "https://www.koolcenter.com/article/image/fc530/01.jpg"
date: 2021-11-09T15:04:23+08:00
description: >
  转眼间PCI-E 4.0接口在消费级平台上市已经有一年多的时间了，各大主流厂商都陆续推出了基于PCI-E 4.0的消费级固态盘产品。就在不久前传统存储巨头希捷推出了自家第二代的PCI-E 4.0消费级固态盘产品——酷玩FireCuda 530。
--- 

# 

## 前言

​	转眼间PCI-E 4.0接口在消费级平台上市已经有一年多的时间了，各大主流厂商都陆续推出了基于PCI-E 4.0的消费级固态盘产品。就在不久前传统存储巨头希捷推出了自家第二代的PCI-E 4.0消费级固态盘产品——酷玩FireCuda 530。

​	酷玩FireCuda系列定位于游戏和创作，前两代的酷玩510和520均是基于群联定制方案，性能也处于当时的第一梯队。这次的酷玩530则是采用了群联目前高端E18主控，我们也很期待他的性能表现

## 外观

​	希捷酷玩FireCuda 530的外包装延续了该系列的橙色画风

<img src="https://www.koolcenter.com/article/image/fc530/01.jpg" style="zoom:50%;" />

​	包装盒里除了SSD本体以外还有一些贴纸和说明书

<img src="https://www.koolcenter.com/article/image/fc530/03.jpg" alt="image-20211024211937699" style="zoom:50%;" />

​	SSD本体给包了一层防静电袋，希捷这是我见过唯一这么做的厂家。应该是多年来在机械硬盘领域养成的习惯

<img src="https://www.koolcenter.com/article/image/fc530/04.jpg" alt="image-20211024212227565" style="zoom:50%;" />

​	2TB版本双面均有颗粒分布，盘体正反面均贴有贴纸

<img src="https://www.koolcenter.com/article/image/fc530/05.jpg" alt="image-20211024212946782" style="zoom:50%;" />

​	正反面各4颗NAND和一颗DRAM，正面则多了一枚主控和电源管理芯片

<img src="https://www.koolcenter.com/article/image/fc530/07.jpg" alt="image-20211024213825298" style="zoom:50%;" />

​	酷玩FireCuda 530虽然使用的是定制版群联E18主控，但并没有使用群联E18公版布局。群联的公版布局是主控芯片靠近M.2接口处，DRAM紧随其后，接下来是四颗NAND依次排开，比如像我们之前所测过的HOF EXTREME。而希捷酷玩FireCuda 530则采取了主控和DRAM居中，NAND分列两端的新颖布局。并且定制E18主控上面的印字也是希捷的，而并非是群联。这也说明希捷酷玩FireCuda 530相比其他群联公版方案有其与众不同之处

<img src="https://www.koolcenter.com/article/image/fc530/08.jpg" alt="image-20211024214524371" style="zoom:50%;" />

​	从官方给出耐久度指标来看，希捷酷玩FireCuda 530给出了大约1275PE，而目前主流厂商对于TLC NAND产品给出的参考耐久度普遍为600PE左右，可见希捷对这款产品的信心十足

<img src="https://www.koolcenter.com/article/image/fc530/image-20211104142031533.png" alt="image-20211104142031533" style="zoom: 25%;" />

## 性能简测

​	测试平台选择了Intel的11代RocketLake-S

| CPU  | Intel CORE I9-11900K  |
| :--: | :-------------------: |
| 主板 | ROG MAXIMUS XIII HERO |

​	CrystalDiskInfo 能够清楚地看到写入量，通电次数等信息。但是温度显示18度应该是识别有误，因为此时室温约为24度，通电状态下的固态盘温度是不可能低于室温的。

<img src="https://www.koolcenter.com/article/image/fc530/09.png" alt="image-20211024215001685" style="zoom:50%;" />

​	由于是群联主控，我们可以通过Phison Flash Id来查看一下这块SSD的一些信息，群联PS5018-E18主控的主频提高到了1000Mhz，而上一代的E16只有733Mhz。2TB版本的酷玩530是8通道每通道4CE，总计32CE的满配。NAND则是搭配镁光B47R，最新型的176层堆叠3D NAND，也是目前市面上堆叠层数最多的NAND之一。

<img src="https://www.koolcenter.com/article/image/fc530/10.png" alt="image-20211024215645559" style="zoom:50%;" />

​	首先在空盘全默认配置下跑了一个CrystalDiskMark，顺序读写基本都可以达到7000MB/S左右

<img src="https://www.koolcenter.com/article/image/fc530/12.png" alt="image-20211024220651335" style="zoom:50%;" />

​	而切换到IOPS视图，可以看到4K随机读写也都超过了百万IOPS

<img src="https://www.koolcenter.com/article/image/fc530/13.png" alt="image-20211024220751377" style="zoom:50%;" />

​	把测试数据块大小调整为32GB之后，也没有发生多少性能衰减

<img src="https://www.koolcenter.com/article/image/fc530/image-20211024224207719.png" alt="image-20211024224207719" style="zoom:50%;" />

​	而向盘内装入游戏、视频等1600GB数据占用87%空间后，也依然能够维持和空盘差不多的性能水准

<img src="https://www.koolcenter.com/article/image/fc530/image-20211024224256854.png" alt="image-20211024224256854" style="zoom:50%;" />

​	而在PCMARK10的存储测试中，希捷酷玩FireCuda 530是要超过三星980pro的，落后于浦科特M10P

<img src="https://www.koolcenter.com/article/image/fc530/23.png" alt="image-20211024230304999" style="zoom: 33%;" />

## 极限吞吐量测试

​	随机读写固然是超过官方给出的100万，然而顺序读取却始终停留在7000出头，即使采用全0填充的测试数据也没有更多提高

<img src="https://www.koolcenter.com/article/image/fc530/18.png" alt="image-20211024222901207" style="zoom:50%;" />

​	希捷酷玩FireCuda 530 2T版本官方给出的性能指标，128k数据块顺序读取是可以达到7300MB/S的，剩余的那200多MB/S哪里去了呢？

​	这和PCI-E协议中的一个参数有关——Maximum Payload Size（MPS）。简单的来说每一帧PCI-E数据都有基本固定长度的头部和尾部，中间传输的我们认为才是“有用的数据”，而这个参数便是控制这些“有用的数据”长度的。由于报文首位的长度基本固定，所以中间部分越长，用在协议上的传输损耗也就越少。这和我们追求万兆网络传输的极限速度时，我们要开启交换机的巨型帧功能来降低协议损耗是一个原理

​	而Intel的RocketLake-S，目前支持最大的MPS为256字节

<img src="https://www.koolcenter.com/article/image/fc530/15.png" alt="image-20211024222426635" style="zoom: 33%;" />

​	而AMD的Zen3平台支持512字节，与希捷酷玩FireCuda 530匹配。所以要想追求酷玩FireCuda 530的极限吞吐量，我们需要切换到AMD平台

<img src="https://www.koolcenter.com/article/image/fc530/16.png" alt="image-20211024222609614" style="zoom: 33%;" />

​	这样我们便得到了酷玩FireCuda 530的最高读取性能，我们想要看到的7300+出现了

<img src="https://www.koolcenter.com/article/image/fc530/19.png" alt="image-20211024223100425" style="zoom:50%;" />

​	但由于AMD Zen3平台的随机性能要略逊于Intel RocketLake-S，所以除了这段极限吞吐量以外，其余的测试还依旧是基于Intel平台来做

## 写入性能测试

​	SLC Cache技术在消费级SSD中的普及可以大幅提高日常使用体验，但对于固件算法和NAND品质不佳的固态盘，SLC Cache却成了一块遮羞布。要说现在拿到一个SSD，玩家们最关心的一个话题便是这个盘的SLC CACHE有多大，当CACHE耗尽之后实际的写入速度优势多少。那么这款酷玩FireCuda 530 2TB版本的表现如何呢？

​	我这里使用128KB大小的数据块对它进行了持续写入，从空盘一直写满整盘2TB容量为止。总共用时595秒，简单用除法算出来的平均速率高达3361MB/S。从任务管理器所记录的性能监控中可以看到，写入速度总共分为三个阶段，6.8GB/S，3.8GB/S，1.5GB/S

![image-20211024223936078](https://www.koolcenter.com/article/image/fc530/20.png)

​	而这595秒具体的写入速度分布如下，前33秒处于SLC CACHE状态，一直维持6800MB/S左右的高速；第34秒开始进入TLC NAND直写状态，速度下滑至3800MB/S左右，而在第425秒开始进入边回收边写入状态，速度下滑至1500MB/S左右。

![image-20211024224611203](https://www.koolcenter.com/article/image/fc530/21.png)

​	如果我们把写入时间切换为写入容量，那么会得到下面这个图。前220GB为SLC CACHE空间，中间约1500GB为TLC NAND直写过程，最后接近300GB边回收边写入。当然因为酷玩FireCuda 530速度太快，这里是以秒为单位做计算，可能会存在几GB的误差，但整体不会有什么变化。

​	3800MB/S的直写速度是目前市面上消费级固态盘毫无疑问的No.1，因为我目前连超过2000MB/S的几乎都没见到过。这当然很大程度上得益于先进的176层堆叠NAND

![image-20211024225611701](https://www.koolcenter.com/article/image/fc530/22.png)

## 随机读写测试

​	接下来使用IOMETER来测试一下酷玩FireCuda 530的随机性能表现

![image-20211024230613605](https://www.koolcenter.com/article/image/fc530/25.png)

​	读取方面IOPS随着队列和线程数的提高而稳步上升，直到Q32T16时才达到峰值，约103万IOPS。而写入则要更早的进入状态，在Q4T16即达到最高约130万IOPS

![image-20211024230814991](https://www.koolcenter.com/article/image/fc530/26.png)

​	在高强度的离散度测试中，希捷酷玩FireCuda 530表现得并没有上面几项测试中那么出色。虽然IOPS维持在3万以上，但在长达3个小时的过程中没有进入稳定态。当然这也是群联方案的传统弱项，希捷定制版本并没有能够实现更高的突破。

![image-20211024231035480](https://www.koolcenter.com/article/image/fc530/27.png)

## 游戏测试

​	在今年9月份的时候，索尼PlayStation 5系统更新，开放了M.2接口扩展SSD。定位于游戏玩家的酷玩FireCuda 530也早早宣布支持PS5，那么下面我就来测试一下它在PS5中的表现

<img src="https://www.koolcenter.com/article/image/fc530/28.jpg" alt="image-20211024231550096" style="zoom:50%;" />

​	安装方式很简单，知道怎么打开PS5的侧板就行了，当然要先关机就是了。

<img src="https://www.koolcenter.com/article/image/fc530/29.jpg" alt="image-20211024231637192" style="zoom:50%;" />

​	然后就是按系统提示格式化M.2 SSD了

<img src="https://www.koolcenter.com/article/image/fc530/30.jpg" alt="image-20211024231713175" style="zoom:50%;" />

​	PS5在格式化之后还会帮玩家测个速，这里测出来6558.481MB/S的速度比在PC上略慢了一点

<img src="https://www.koolcenter.com/article/image/fc530/31.jpg" alt="image-20211024231741900" style="zoom:50%;" />

​	2TB存储空间完美识别，型号也正常识别

<img src="https://www.koolcenter.com/article/image/fc530/32.jpg" alt="image-20211024231834587" style="zoom: 25%;" />

​	首先先来测试一下游戏拷贝速度。这里选了一款PS5游戏《破晓传说》，今年9月9日刚刚上市的新作

<img src="https://www.koolcenter.com/article/image/fc530/36.jpg" alt="image-20211024232936728" style="zoom: 25%;" />

​	另一款是PS4游戏《英雄传说：创之轨迹》，也是我作为一个轨迹粉丝的情怀作品

<img src="https://www.koolcenter.com/article/image/fc530/34.jpg" alt="image-20211024233023630" style="zoom: 25%;" />

​	先从PS5内置SSD中移动到酷玩 530，再从酷玩530移动回来

<img src="https://www.koolcenter.com/article/image/fc530/33.jpg" alt="image-20211024232420273" style="zoom: 25%;" />

​	这个结果可能大大出乎玩家们的预料，当然我也一度怀疑测试除了问题，但是连测了三次均是如此。游戏移动到PS5内置硬盘的耗时居然差不多是移动到希捷酷玩FireCuda 530的5倍左右，也就是说酷玩 530的写入性能要远远好于PS5内置硬盘，甚至已经接近一个量级

<img src="https://www.koolcenter.com/article/image/fc530/35.png" alt="image-20211024232507964"  />

​	接下来是游戏加载，两款游戏分别在内置盘和酷玩530上进行读档、场景切换等操作。使用秒表测试耗时，每个场景测3遍取平均值

<img src="https://www.koolcenter.com/article/image/fc530/39.jpg" alt="image-20211024233214256" style="zoom: 25%;" />

​	希捷酷玩FireCuda 530在游戏加载方面略好于PS5内置盘，没有了之前拷贝那么夸张的性能差距，区别在几个百分点之间

![image-20211024233757186](https://www.koolcenter.com/article/image/fc530/37.png)

## 总结

​	与一般贴牌的公版群联产品不同，我们在酷玩FireCuda 530的身上看到了希捷下的功夫。论缓存外的持续写入，酷玩FireCuda 530可以说是目前消费级SSD的最强者。经过精心调教的固件加上两倍于主流产品的耐久度，相信酷玩FireCuda 530是将是游戏玩家的首选

