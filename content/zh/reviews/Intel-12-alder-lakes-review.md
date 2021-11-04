---
title: "蓝色巨人的觉醒——Intel 第12代酷睿处理器Alder Lake S首发评测"
linkTitle: "蓝色巨人的觉醒——Intel 第12代酷睿处理器Alder Lake S首发评测"
author: "御剑江湖"
coverImg: "https://www.koolcenter.com/article/image/12900k/cover.jpg"
date: 2021-11-04 21:00:08
description: >
  在Intel长达数十年的制程演进历史中，从未遇到过10nm节点这样的困难。10nm工艺多次跳票，摩尔定律作古，让Intel面临着前所未有的危机。
--- 
## 千呼万唤始出来——跳票多年的10nm工艺终于降临桌面平台

​	在Intel长达数十年的制程演进历史中，从未遇到过10nm节点这样的困难。10nm工艺多次跳票，摩尔定律作古，让Intel面临着前所未有的危机。当竞争对手在桌面级高性能处理器上使用7nm工艺时，Intel只能使用老态龙钟的14nm后面继续添加号来苦苦支撑。即使三星和台积电的制程数字上有些许注水，但这无法改变Intel依然处于落后地位的事实

​	其实Intel在这么多年来在10nm节点做过多次尝试：

> - 最早在2018年曾推出过基于初代10nm工艺的Cannon Lake系列，代表作品便是NUC Crimson Canyon深红峡谷，本站也曾经做过相关评测。然而初代的不成熟工艺甚至连集显都做不出来，Crimson Canyon深红峡谷还需要外挂一颗AMD的GPU才能使用。，i3-8121U即是第一款也是最后一款的Cannon Lake处理器。~~这也成了Intel的一段不愿回首的黑历史，拼命想将其抹掉，以至于在其官网的ark库里关于Cannon Lake的条目都已经是“Page Not Found”了~~
> - 第二次便是我们比较熟悉的Ice Lake系列了，2019年问世，代表作品便是i7-1065G7。功耗和性能的平衡表现使其在许多轻薄笔记本中予以采用，Intel更愿意将Ice Lake称为第一代10nm工艺，我现在也正在使用着基于这款处理器的笔记本来编辑这篇文章。但这代工艺也有着一定的问题，那便是无法冲击高性能，i7-1065G7最高功耗配置仅为25瓦，最高单核心主频也仅能维持在4GHz上下。这对于移动平台来说或许还够用，但对于桌面平台来讲是远远不够的
> - 第三次是去年年底的Tiger Lake，按照Intel的想法，这算是第二代的10nm工艺，按照以往的命名规则应该叫做10nm+。或许是之前14nm的加号太多，被消费者疯狂吐槽的缘故，这次Intel并没有用加号，而是改叫10nm Super Fin。这代保留了Ice Lake的优点，搭建了Evo生态平台。同时也逐渐克服上一代的缺点，在今年的H45构架下，单核心主频已经可以达到5GHz，有向桌面平台叫板的实力了

​	在经过三次改良之后，10nm工艺终于登堂入室。桌面版的Alder Lake S发布，制程命名也从10nm Enhanced Super Fin改为Intel 7。其实叫什么并不重要，重要的是效果。Alder Lake S挟异构大小核、DDR5内存、PCI-E 5.0等诸多新科技降临桌面平台，究竟会激起怎样的浪花呢？

## 大与小，5与5——混合架构和次时代接口标准

​	Big. Little，这是手机处理器领域的一个流行词。让少数“大”核处理单线程复杂计算，让多数“小”核处理后台多线程简单运算从而提升能效比，大小核架构是手机领域对有限电池容量的一种妥协。而Intel也曾经在移动平台的Lakefield上短暂尝试过。以往在桌面平台不需要考虑耗电问题，所以无论是Intel还是AMD，两家都在尽可能多地做大核。然而今时不同往日，在处理器TDP突破200瓦的当下，能效比也不得不进入桌面平台的考虑范畴。Alder Lake上的大小核混合架构，无疑是一次大胆地尝试

​	Alder Lake的“大”核基于Golden Cove架构，命名为Performance Core；而“小”核基于Grace Mont架构，命名为（Efficient Core）。从理论上来说，“大”核更适用于单线程、高负载的游戏及生产力应用，而“小”核更适用于后台多线程轻度工作负载。

​	从物理上实现大小核或许还容易一些，毕竟业界也有过不少“胶水”CPU的案例，但如何调度大小核成为了一个巨大的难题。吸取了之前的Lakefield的经验，Intel在Alder Lake上开发了一套全新的调度系统——Intel thread Director。并且在操作系统层面，微软的Windows 11也大幅改进了任务调度规则。二者相结合将更好的分配任务给两类核心，从而避免出现张冠李戴的情况。

<img src="https://www.koolcenter.com/article/image/12900k/01.png" style="zoom:50%;" />

​		除了大小核，Alder Lake还为我们带来了两个5，那便是DDR5内存和PCI-E 5.0。其实在推行新的内存和PCI-E标准的道路上，Intel本是走在前面的，P915的DDR2、P35的DDR3、X99的DDR4、P45的PCI-E 2.0、Z77的PCI-E 3.0，只有在PCI-E4.0的时代被AMD Zen2抢了先手。这次Intel的Alder Lake抢先发布了PCI-E 5.0和DDR5，又再次占得了先机

<img src="https://www.koolcenter.com/article/image/12900k/02.png" style="zoom:50%;" />

​	与Alder Lake同时发布的还有其标配座驾Z690芯片组，以往被玩家们疯狂吐槽的牙签总线不见了踪影，取而代之的是DMI 4.0 X8，带宽是原来的4倍。同时也支持下挂PCI-E4.0接口了

![](https://www.koolcenter.com/article/image/12900k/03.png)

## 卷土重来——再与Zen3争高下

### 	ROG MAXIMUS Z690 HERO 与 宇瞻DDR5内存

​	早在前几天新闻稿解禁之日，我曾经介绍了一下MAXIMUS Z690 HERO的外观和配置。接下来我们结合Alder Lake以及Z690的新特性看一下他的BIOS

<img src="https://www.koolcenter.com/article/image/12900k/04.png" style="zoom:50%;" />

​	首先是DDR5内存，我们用来测试的内存是一对来自宇瞻的普条，就这这样的普通外观

<img src="https://www.koolcenter.com/article/image/12900k/mem01.jpg" style="zoom:50%;" />

​	从内存的JEDEC Profile也看得出来，这款内存并不支持什么XMP，原生便是DDR5-4800 CL40

<img src="https://www.koolcenter.com/article/image/12900k/mem02.png" style="zoom:50%;" />

​	而MAXIMUS Z690 HERO则增加了一个选项，叫做ASUS Enhance Memory Profile

<img src="https://www.koolcenter.com/article/image/12900k/05.png" style="zoom:50%;" />

​	开启这个选项之后，我们会惊喜的发现宇瞻这对普条可以像XMP一样选择配置档案了。这对于正处于DDR5初期，对新内存玩法还不甚了解的玩家来说，提供了一个非常便捷的超频方式

<img src="https://www.koolcenter.com/article/image/12900k/06.png" style="zoom:50%;" />

​	除此之外，如果想手动获得更高频率的话，MAXIMUS Z690 HERO提供了最高DDR5-13333的频率

<img src="https://www.koolcenter.com/article/image/12900k/07.png" style="zoom:50%;" />

​	Alder Lake S的内存控制器，保留了上一代Rocket Lake S的GEAR1和GEAR2模式以外，还增加了GEAR4模式，为挑战极限内存频率增加了一些筹码

<img src="https://www.koolcenter.com/article/image/12900k/08.png" style="zoom:50%;" />

​	内核方面的相关设置都被拆分为Performance Core和Efficient Core两部分二分开设置

<img src="https://www.koolcenter.com/article/image/12900k/09.png" style="zoom:50%;" />

​	其中Performance Core可以单独设定每个内核的倍频和电压

<img src="https://www.koolcenter.com/article/image/12900k/10.png" style="zoom:50%;" />

​	高级电源管理中可以看到默认情况下每个Performance Core核心的最高倍频，从而知道哪些核心体质更好

<img src="https://www.koolcenter.com/article/image/12900k/13.png" style="zoom:50%;" />

​	而Efficient Core被分为两组来进行控制，并不能细化到每一个

<img src="https://www.koolcenter.com/article/image/12900k/11.png" style="zoom:50%;" />

​	不过Efficient Core可以选择开启数量，或全部关闭

<img src="https://www.koolcenter.com/article/image/12900k/12.png" style="zoom:50%;" />

### 基准测试

​	接下来的部分便是针对Alder Lake S的性能测试了，首先介绍一下测试平台。除了12代以外，还找来了11代的I9-11900K与AMD目前主流桌面平台的5950X作为比较。操作系统当然是最新的Windows 11，有一些软件内依然识别为Windows 10，认为是软件bug了。测试方法是每种测试跑三遍，如果区别不大就选三次中的最高值；如果差别较大就再跑两次，选五个结果中第二高的值

| CPU    | Intel Core i9-12900K       | Intel Core i5-12600K       | Intel Core i9-11900K       | AMD Ryzen 9 5950X          |
| ------ | -------------------------- | -------------------------- | -------------------------- | -------------------------- |
| 主板   | ROG MAXIMUS Z690 HERO      | ROG MAXIMUS Z690 HERO      | ROG MAXIMUS VIII HERO      | ROG STRIX X570-I           |
| 内存   | 宇瞻 DDR5-4800 CL40        | 宇瞻 DDR5-4800 CL40        | KLEVV DDR4-4000 CL18       | KLEVV DDR4-4000 CL18       |
| 显卡   | 影驰 RTX 3080 GAMER OC     | 影驰 RTX 3080 GAMER OC     | 影驰 RTX 3080 GAMER OC     | 影驰 RTX 3080 GAMER OC     |
| 系统盘 | 三星 980PRO 1TB            | 三星 980PRO 1TB            | 三星 980PRO 1TB            | 三星 980PRO 1TB            |
| 游戏盘 | 希捷 酷玩 FireCuda 530 2TB | 希捷 酷玩 FireCuda 530 2TB | 希捷 酷玩 FireCuda 530 2TB | 希捷 酷玩 FireCuda 530 2TB |
| 散热器 | 利民 冰封远景 360          | 利民 冰封远景 360          | 利民 冰封远景 360          | 利民 冰封远景 360          |

​	此次收到的评测样品为I9-12900K和I5-12600K，I9-12900K的配置为8大核（全核心4.9Ghz，单核心5.2Ghz）+8小核（全核心3.7Ghz），而I5-12600K的配置为6大核+4小核。由于Alder Lake仅有大核（Performance Core）才配备超线程技术，所以我们会见到16核24线程与10核16线程这种“奇葩”组合

<img src="https://www.koolcenter.com/article/image/12900k/14.png" style="zoom:50%;" />

​	由于DDR5内存内部是两组32bit通道传输数据，所以单根内存即可实现双通道，两根内存则被识别为四通道。与此同时，上文所说提到的ASUS Enhance Memory Profile功能顺利开启无压力

<img src="https://www.koolcenter.com/article/image/12900k/mem03.png" style="zoom:50%;" />

​	内存的带宽测试非常夸张，DDR4很难达到这种数据了

<img src="https://www.koolcenter.com/article/image/12900k/mem04.png" style="zoom: 33%;" />

​	CPU-Z基准测试，I9-12900K单线程突破了800分。10代到12代实现了cpu-z单线程跑分整百关口的二连跳，IPC的提升很可观

<img src="https://www.koolcenter.com/article/image/12900k/15.png" style="zoom: 50%;" />

​	在和其他处理器对比下，I9-12900K的单线程优势巨大，多线程也基本追上32线程的5950X。而I5-12600K也要超过上代的I9-11900K

<img src="https://www.koolcenter.com/article/image/12900k/16.png" style="zoom:50%;" />

​	在另一个常用的测试工具Cinebench R23中，I9-12900K表现仍旧出色，单线程接近2000分

<img src="https://www.koolcenter.com/article/image/12900k/17.png" style="zoom: 33%;" />

​	在与其他参测处理器的对比中I9-12900K也是一骑绝尘，甚至已经超过了5950X。I5-12600K也是单线程和多线程全都超过I9-11900K

<img src="https://www.koolcenter.com/article/image/12900k/18.png" style="zoom:50%;" />

​	接下来是两个解压缩测试，7zip和WinRAR。在这两项压缩解压测试中，或许是由于DDR5内存高延迟的拖累，12代的IPC优势未能得到很好的体现，导致单线程中12900K甚至弱于11900K

<img src="https://www.koolcenter.com/article/image/12900k/19.png" style="zoom:50%;" />

​	而在这项测试中5950X则独占鳌头

<img src="https://www.koolcenter.com/article/image/12900k/20.png" style="zoom:50%;" />

<img src="https://www.koolcenter.com/article/image/12900k/21.png" style="zoom:50%;" />

​	3DMark Timespy测试，更贴近游戏中的物理运算，12900K得分达到了18388分

<img src="https://www.koolcenter.com/article/image/12900k/22.png" style="zoom: 25%;" />

​	相比之下其他处理器均为超过14000分，12900K再次赢得巨大优势

<img src="https://www.koolcenter.com/article/image/12900k/23.png" style="zoom: 67%;" />

​	在3DMARK的CPU Profile测试中，我们可以看到CPU在不同线程数的表现

<img src="https://www.koolcenter.com/article/image/12900k/24.png" style="zoom: 25%;" />

​	虽然5950X要多8个线程，但这多出来的超线程对于3DMARK来说并没有多大作用，无论线程数多大，12900K依然保持着领先优势。

<img src="https://www.koolcenter.com/article/image/12900k/25.png" style="zoom: 67%;" />

​	由于游戏中的物理测试交给了3DMARK，所以用PCMARK10主要测试一下日常生产力应用的情况

<img src="https://www.koolcenter.com/article/image/12900k/26.png" style="zoom:33%;" />

​	在这个项目中，各自的差距并不大，不过依然能够看得出12900K的领先优势

<img src="https://www.koolcenter.com/article/image/12900k/27.png" style="zoom:50%;" />

​	

### 游戏测试

​	首先是战争机器5，使用内置基准测试程序

<img src="https://www.koolcenter.com/article/image/12900k/28.jpg" style="zoom:50%;" />

​	12900K全面领先于其他处理器，画质和分辨率越低，12900K的优势越明显。随着分辨率提高到4K，这种优势消耗殆尽

<img src="https://www.koolcenter.com/article/image/12900k/29.png" style="zoom: 67%;" />

​	接下来是古墓丽影：暗影，同样适用内置测试程序

<img src="https://www.koolcenter.com/article/image/12900k/30.jpg" style="zoom:50%;" />

​		在这项测试中个CPU的差距比较小，仅有12900K在1080P分辨率下显示出稍大的优势，而12600K和11900K的表现几乎一样

<img src="https://www.koolcenter.com/article/image/12900k/31.png" style="zoom:67%;" />

​	接下来是地平线：零之曙光，采用内置测试工具

<img src="https://www.koolcenter.com/article/image/12900k/32.jpg" style="zoom:50%;" />

​	地平线的测试结果中，12600K拉开了与11900K的差距，更接近于12900K

<img src="https://www.koolcenter.com/article/image/12900k/33.png" style="zoom:67%;" />

​	接下来是仙剑奇侠传七，由于这款游戏并没有内置测试工具，选取了两个场景进行测试。一个是在天师门中庭这个场景比较复杂的位置，另一个是在御灵飞行在云端时这个相对简单的画面。~~10G显存的3080惨遭鄙视~~

<img src="https://www.koolcenter.com/article/image/12900k/34.jpg" style="zoom: 25%;" />

​	仙剑七的测试和地平线的结果类似，12600k超过11900k，总体差距并不大

<img src="https://www.koolcenter.com/article/image/12900k/35.png" style="zoom:67%;" />

​	在游戏方面，12代的Alder Lake延续了传统优势并且以肉眼可见的优势领先



## 神魔两面——看过了Alder Lake光鲜的一面，那么他的背后是什么样的呢？

​	Windows 11和Intel thread Director虽然能解决大部分调度问题，但仍有部分软件就是那么的有个性。比如wPrime这款8年前的多线程圆周率计算软件就为我们上演了一出小核有难大核围观的杯具。测试刚开始时24个线程全部满载，CPU符合达到100%，但在几秒钟之后大核们的使用率纷纷降为0，而小核们则一直保持的100%

<img src="https://www.koolcenter.com/article/image/12900k/51.png" style="zoom: 33%;" />

​	当然这种现象比较罕见，测试了许多软件也只有wPrime出现了调度问题，概率还是可以接受。不过功耗问题则就不那么容易回避了

<img src="https://www.koolcenter.com/article/image/12900k/52.png" style="zoom: 33%;" />

​	在AIDA64的Stress FPU测试中，i9-12900K的8个Performance Core都维持在4.9GHz，8个Efficient Core维持在3.7GHz，此时的功耗接近230W，而在运行CineBench R23的时候甚至要更高。

<img src="https://www.koolcenter.com/article/image/12900k/53.png" style="zoom: 67%;" />

​	在功耗上，新制程的12900k比11900k还是低了一些的。但相比于竞争对手，还有比较大的劣势



## 任重道远

​	Alder Lake S的性能表现是值得称赞的，IPC再度提升使得自家11代之前的处理器都远远地被甩在了后面，即使在少8个线程的情况下，也能在多线程测试中与5950X打得有来有回。**特别是12600K，作为本代i5已经可以把上代I9拉下马，性价比较为突出**

​	而在游戏方面，12代的酷睿继续保持了领先的身位，并且将后面的Ryzen越甩越远

​	然而山雨欲来风满楼，Intel的王座在风雨飘摇中岌岌可危。自从Coffee Lake的I9诞生以来，Intel在桌面平台走上了一条以功耗换性能的不归路。反观苹果M1已经走在了能耗比的前方，诚然二者目前并不在同一赛道上，但谁又能保证未来不会出现正面碰撞呢？

​	12代很好，但还不够。Intel要想坐稳天下第一，还差一个从奔腾D到酷睿2的飞跃。随着Intel的制程逐步走回正轨，这一切似乎也不是那么遥远了

