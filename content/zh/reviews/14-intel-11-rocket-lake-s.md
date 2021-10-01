
---
title: "14纳米的最终乐章——Intel 第11代酷睿处理器Rocket Lake S评测"
linkTitle: "14纳米的最终乐章——Intel 第11代酷睿处理器Rocket Lake S评测"
author: "御剑江湖"
coverImg: "https://image.koolcenter.com/attachment/forum/202103/30/000621mq7gf47gqglk1g77.png"
date: 2021-07-06 16:49:08
tags: ["TODO"]
categories: ["TODO"]
description: >
  TODO
---

> **一年又一年**

 从2015年的Broadwell起，Intel的14nm工艺已经陪我们走过了整整6个年头。在这6年的时间里发生了许多的事情，10nm工艺难产令数十年的摩尔定律作古、幽灵熔断漏洞让酷睿和至强陷入了一番信任危机、锐龙横空出世性能王座易主，这桩桩件件对Intel来说都不是什么好消息。

 虽然目前Intel依靠10400F、10600KF、10700F这些高性价比的处理器依旧能够在消费级市场占有率保持领先优势，但高端性能已经被Ryzen 5000系列击败，不夸张的说Intel正面临着继奔腾D时代以来最严峻的考验。

 Rocket Lake S是Intel发布的第七代也是最后一代的14nm处理器，也代表着Intel 14nm工艺的最高水准，背负着众多人的希望奔赴战场。这场14nm的谢幕演出究竟是反击的号角，还是沉沦的预兆，让我们一起来看一下



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzE4fDEzOGJhY2MzfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


> **多重亮点的换代**

 这部分内容我曾经在之前的发布新闻中讲到过，下面再领大家复习一下。 桌面级CPU经历了多年的主频大战与核心数大战后进入了一定的瓶颈期，然而近两年IPC这个概念逐渐走进大家的视野。在主频和核心数都难以再继续更进一步的情况下，提高IPC显然是一个既快速又有效的手段。AMD在ZEN2和ZEN3中就是这样做的，而Intel在这方面跟进的却显得慢了一些，Rocket Lake S也是在Skylake之后首次重点提高了IPC的一代，按照先期的宣传是UP TO 19%。实际究竟怎样，下面就要进行测试了



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzE5fDNjODA2OTY4fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


在CPU内核方面采用了与第十代移动版Ice Lake的Sunny Cove更相近的Cypress Cove架构，IPC得到了较大幅度的提升。

在GPU内核方面采用了与第十一代移动版Tiger Lake相同的Xe图形架构，除了图形性能大幅提升以外，还支持原生HDMI2.0视频输出。这对使用高分辨率显示屏的用户来讲是个利好消息。

总的来说Rocket Lake S可以看做是一个用14nm技术实现的Ice Lake CPU + Tiger Lake GPU的高性能集合体，极高成熟度的14nm工艺可以将其推高到一个不可思议的频率，从而提高性能体验



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzIwfGFiOTQxMTBmfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


除了IPC提高以外，Rocket Lake S外围扩展方面也有着不小的提高。不但将CPU内置的PCI-E 控制器升级为GEN4，而且直通CPU 的PCI-E通道数从上一代的16提高到20。也就是说现在我们可以在保留X16全速显卡的同时，还可以拥有一片直通CPU的 PCI-E 4.0高性能SSD接口。

在前几代Intel芯片组中饱受玩家吐槽DMI总线这次也从X4提升到了X8，带宽直接翻倍。下挂高速存储等设备不再像以前一样尴尬

Rocket Lake S支持Resizable BAR可以更好的实现显存与CPU之间的通信，也就是类似之前AMD在RDNA2显卡和ZEN3 CPU上宣传的神秘加成的SAM功能。这其实是PCI-E接口中的一项标准，Intel同样可以实现，当然也支持nVidia显卡

Rocket Lake S并没有像移动版那样在CPU中集成雷电控制器，所以想要使用雷电4还是需要Z590芯片组来进行转接



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzIxfDQyOGE5Y2QxfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


       关于500系列芯片组，由于Z590先期已经上市，大家可能已经有所了解。主要的特点是集成USB 3.2 GEN 2x2，也就是20Gbps速度的USB接口。集成2.5G以太网MAC等特性。

       而此次与Rocket Lake S发布同时，Intel还向外界透露，B560和H570芯片组将得到一项重大福利——内存可超频。以往无论是CPU还是内存的超频都是Z级别芯片组的专利，此次Intel将内存超频功能下放至B560和H570系列，但CPU超频并未下放。这无疑又提升了这两款中端芯片组的吸引力



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzIyfDFmZWNjYWY4fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


> 主流测试平台

 送测的包装与零售版相去甚远，从正面看上去和Intel第11代处理器的LOGO蛮像的



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzA0fDBmZGYxNWE1fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 此次我们收到的送测CPU是I9-11900K和I5-11600K



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzA1fDk0NTU3NjcwfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 这两颗CPU无论是顶盖还是背面电容分布都没有什么区别，根据经验我们可以判断I5-11600K是由I9-11900K屏蔽而来的



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzA2fDNjZTk3Njk5fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)




![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzA3fDgyZTBkZmNkfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 而I9-11900K和上一代的I9-10900K就有了显著区别，I9-11900K的顶盖面积要更大



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzA4fGI2ODNhMjNhfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 接口同为LGA1200，同时兼容Intel Z490和Z590主板，不过由于供电和BIOS限制部分B460主板一下主板不支持11代处理器



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzA5fDk3MzE4NjY3fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 I9-11900K的顶盖不止体积变大了，外形也有了一定的变化，采用了三层的阶梯式设计



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzEwfGM3MDIzMmMxfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 I9-11900K的基板比I9-10900K要稍微厚一点点



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzExfDExYjY0ZjIwfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 这次的测试平台以华硕的组件为基础搭建，其中11700K在另一位编辑那里，虽然我也把测试结果整合过来了，但测试平台不同所以仅供参考



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzEyfDI1ZDVhYjUyfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 这是来自本次测试的组件合照



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzE0fGJlZWQxM2M2fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 11900K安装在M13H上



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzEzfDc1YjhhZjNjfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 为了方便更换多颗CPU来测试，所以采用裸机安装



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzE1fGEyYTI0MWMzfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


> **Intel Adaptive Boost Technology——开启全核心5G时代**

      睿频加速（Turbo Boost）技术是Intel最常用的自动提频技术，从第一代酷睿i系列处理器问世以来已经经历了十几个年头。经过时间的推移，睿频加速技术也在不断的进化。从初期Bloomfield的1.0，Sandy Bridge的2.0到Skylake-X的Turbo Boost Max 3.0。CPU的睿频频率终于在I7-8086K的时候摸到了单核心5GHz

直到上一代Comet Lake S中，Intel又推出了Thermal Velocity Boost(TVB)来辅助Turbo Boost来进一步提高主频。但是由于Thermal Velocity Boost(TVB)只能提高0.1GHz主频，而且提频的条件比较苛刻，需要温度小于70度才可以生效，这使得实际应用中Thermal Velocity Boost的效果并没有想象中的那么给力。

Intel Adaptive Boost Technology(ABT)技术克服了Thermal Velocity Boost(TVB)的一些缺点，比如温度墙从70度提高到100度，最大睿频幅度也从0.1提高到0.4，从而使得处理器的主频能够更上一层楼



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NjkxfGM2ODkzOTZmfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 这项技术目前是I9-11900K/KF独占，只有我们的散热系统和主板供电够强大，Intel Adaptive Boost Technology技术能够将I9-11900K/KF的全核心睿频提高到5.1GHz这种不可思议的高度。而这项功能的开关在华硕主板中默认是关闭状态，我们需要手动将其打开



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NjkyfGQ1MjExMmY0fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在关闭ABT时，I9-11900K在执行AIDA64 Stress FPU拷机时全核心主频为4.8GHz。根据上面的规格示意图可知此时Turbo Boost 2.0技术将全核心推高到4.7Ghz，而在利民Frozen MAGIC 360 SCENIC水冷的压制下整体核心温度在60度左右，此时Thermal Velocity Boost(TVB)技术生效，将主频在TB2.0的基础上再推高0.1达到4.8GHz



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0Njk0fGRhYTBmYTcyfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 而在开启ABT之后，AIDA64 Stress FPU拷机的全核心主频达到5.1GHz。值得注意的是拷机温度持续稳定在80度左右，当然这很大一部分是要归功于利民Frozen MAGIC 360 SCENIC的强大散热能力，但依旧不可忽视ABT技术的强大。因为我那颗同为8核心的I9-9900K在手动超频至全核心5.1GHz主频之后无论用何种散热系统都难以阻止他在拷机的时候冲上100度。ABT技术智能化地自适应调整电压曲线，远比我们手动超频来的更精准，带来温度和功耗也更低



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NjkzfGVmYWYyMDk2fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)




![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzI1fGY2M2NmYjQ5fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 而在PCMARK 10的测试过程中，11900K的单核心频率也能长期保持在5.3Ghz上



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzQxfGQxYjVmNzNmfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 高主频带来高跑分也是必然的事情了，在Cinebench R23的测试中开启ABT比关闭ABT要高了差不多1000分



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0Njk1fDU2MWY3MGJkfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)




![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzIzfDVjNjU4YzA1fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


> **内存控制器的新玩法**

 在先前的发布新闻中我曾经提到了关于Rocket Lake S内存控制器的相关话题，这一代的内存控制器有着两种运行状态：

- GEAR 1——同频模式，即内存控制器与内存频率比例为1：1
- GEAR 2——分频模式，即内存控制器与内存频率比例为1：2


 从理论上看来，显而易见GEAR 1的内存控制器频率更高，性能应该更好；而GEAR 2的内存控制器频率低，即使在内存控制器体质偏弱的情况下也不会对内存的超频带来瓶颈

 在最新版的GPU-Z 1.95中已经可以看到内存控制器频率这个参数了，当然是要搭配Rocket Lake S处理器才看得到



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0Njk4fGUxZTk4YjQ0fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在华硕M13H的BIOS中我们也可以找到相关的设置，值得一提的是按照Intel原本的说法是DDR-3200以上频率的GEAR1模式是I9独享的，但实际在安装I5-11600K的测试过程中也可以选择GEAR1，但是搭配10代处理器时该选项是隐藏状态



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0Njk2fDUyMWU5NzhkfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在选择1：1或是1：2的时候都会造成一些内存频率无法选择，比如我们无法在1：2的前提下选择DDR4-3600的内存频率



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0Njk3fGFiOTI3ZWI0fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 不过这个新型的内存控制器的表现还比较迷。我最开始测试平台使用一对B-DIE的幻光戟，测试跑在GEAR2 DDR-4000C17可以通过各种测试。后来想测试GEAR1模式，但同样的内存参数在GEAR1下无法点亮，无论把CL放款到19还是把频率降低为3600都无效。于是我更换为一对科赋的BoltX系列内存海力士CJR颗粒，这次3600频率GEAR1可以点亮，但更高的GEAR1不行了

 虽然最终没有能够将两种内存控制器和内存频率统一，但通过3600GEAR1和4000GEAR2的对比也能看得出来，虽然4000GEAR2因为内存频率更高得到了更好的内存带宽表现，但是内存延迟反倒是3600GEAR1更低，而且领先的还挺明显。这说明GEAR1的同频模式在内存延迟方面有个更好的表现



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0Njk5fGI0M2Y1OTczfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 总的来说这代内存控制器的可玩性很高，但是由于精力所限我没有更多的时间去仔细研究，更多玩法有待玩家开发了

> **力挽狂澜的理论测试**

 终于到了期待的跑分环节，虽然跑分并不完全代表性能优劣，但至少可以给大家一个简单明了的比较。其中I7-11700K的成绩来自我们的另外一位编辑夜半点灯，虽然我将成绩做了整合，不过由于测试平台不同所以成绩会有一定出入，仅供大家参考



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzI5fDBmMjNmN2EyfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 先是纯理论测试部分，所有测试中I9-11900K均开启ABT技术，内存工作在4000CL18 GEAR2后面就不再强调了。Cinebench R23的测试中Rocket Lake S显示出了自己IPC的威力。11900K在同为单核心睿频5.3GHz的10900K的对比中，单线程得分领先了20.4%。凭借着这样的IPC优势，在总评中甚至超越了10核心的10900K



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzMxfGM3Mjk3MWM5fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)




![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzI3fDQ2YWRlMDRmfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 CPU-Z的情况与Cinebench R23类似，11900K的单线程成绩超过了700分，这也是我所见到的首个默认情况下单线程超过700分的CPU。单线程领先上一代的10900K幅度为18.1%，也基本符合前期宣传。与此同时我发现我手里这颗R7 5800X的跑分偏低，我尝试更新了BIOS和开启PBO，但始终未能再提高分数，目前我只能认为是我手中这颗5800X的体质较弱无法自动BOOST到一个更高的频率



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzMwfGFkNjQ3ZDcwfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)




![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzI4fDIzYjJlZGY4fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在wPrime 的1024M位运算测试中Rocket lake的领先幅度变小了一点，11900K领先10900K 13.6%



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzMyfDIyYjc4N2RjfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在WinRAR的测试中11900K没有显示出优势，反倒是被5800X超过了



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzMzfDg2MzI3ODRlfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在7zip测试中11900K的单线程恢复了领先，领先10900K约为8%



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzM1fDMxYWYxNDBkfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在SiSoftware Sandra的测试考验的更多是多线程整体效能。在多媒体处理器子项中，在拥有AVX512指令集的加成下，8核心的11900K大幅领先于10核心的10900K。可见内置的指令集一旦触发，那优势并不是多几个核心能够弥补的。而算术处理器子项目还是核心最多的10900K占据上风



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzM2fDkyNmZkZWNkfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 vray benchmark的测试，8核的11900K战胜了10核的10900K，11700K的成绩和5800X差不多



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzM3fDRkMDEwZWVmfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 PCMARK 10的日常应用环节，除了两款10代处理器的网页浏览得分偏低以外，其余CPU差距不大



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzM4fDE2YjI3YWQyfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在使用Microsoft Edge浏览器进行WebXPRT3网页测试，结果和PCMARK10的网页浏览子项目一致，11900K和5800X要明显领先于其他对手



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzM5fDliZGQ5YmJjfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 在3DMARK的物理测试中，8打10的好戏再次上演



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzQwfGFhMTU3M2MxfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 满载功耗方面分成两部分，一部分是软件从传感器读取的CPU功耗，另一部分是通过雷神电源直接读取的整机功耗。Rocket Lake S的功耗比想象中的要低，不过相比5800X的功耗控制还是有一定差距。开启和关闭ABT的11900K简直像是两个东西，开启之后功耗直接瞬间飙升100W。这些功耗带来大约0.3G全核心主频的提升，值不值得就见仁见智了



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzU5fDYwZTI3NDI4fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


> **守护最佳游戏CPU之名**

 游戏是上一代Comet Lake S面对Ryzen 5000系列时为数不多还能保持领先优势的项目，在看到上面理论测试中11900K出色的表现，我们对他的游戏性能也产生了浓厚的兴趣。可惜目前我手上最好的显卡就是STRIX RTX 3070 O8G了，我是真的买不到3080了T\_T....

 正因为显卡偏弱了一点，所以我将游戏的测试分辨率降低为1080P，这样能尽量减少显卡所造成的瓶颈。另外由于夜半点灯的手上没有对应的显卡，所以游戏测试部分缺少11700K的数据 Resizable BAR需要CPU、主板和显卡同时支持，目前大部分显卡的BIOS还没有更新此项功能，所以我这里也并没有能够开启这项技术，GPU-Z的最新版本也可以识别这项功能是否开启



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzYxfGFhOTA2YjI1fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 首先是《战争机器5》，这也是Intel前期在RocketLake宣传中重点提到的一款游戏



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzQyfDYzZjY5MTczfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 1080P最高画质的战争机器，11900K在搭配RTX3070的情况下领先上一代10900K大约4%，如果搭配RTX3080想必差距会更大一些



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzQzfDViMWUzOTM1fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 接下来是《古墓丽影：暗影》，这款游戏经常被用来测试，因为在1080P的分辨率下这款游戏对于CPU的要求比较高，能够突出不同处理器之间的差异



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzUzfGFiYWI0MGJhfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 这次11900K领先的10900K的幅度并不大，不过领先对手5800X差不多10%的水平



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzUyfGYxYzdhZWJmfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 接下来是《地平线：零之曙光》



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzU1fGI3ZDk2Njc1fDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 11900K领先10900K大约4%，领先5800X约8%



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzU0fGZlYmY2MTdifDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 这些3A游戏作品对主频和IPC的敏感程度要高于核心数，11900K在多数游戏测试中还是要比多两个核心的10900K要好一些，Intel持续巩固着自己最强游戏处理器的地位

> **PCI-E 4.0—— 4K IOPS的百万里程碑**

 在先前做980PRO SSD测试的时候我曾经提到过，根据以往的经验AMD Ryzen的存储性能要略弱于Intel，所以980PRO在X570上没能达到标称的100万IOPS。这次Intel的PCI-E 4.0终于登场，我也拿回了两片PCI-E 4.0的顶级SSD。三星980 PRO 1TB用来测试IOPS，影驰 HOF EXTREME 2TB来测试吞吐量



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzAwfDI0YzNhMGJlfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 为了测试I9-11900K的存储性能，需要让影驰SSD达到最大吞吐量，所以测试跨度设定为10GB，没有超过影驰 HOF EXTREME SSD 2TB的缓存范围



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzAyfGJmMzgwMzJhfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 IOMETER的图区和写入都在7000MBPS左右，已经接近PCI-E 4.0 X4的理论上限



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzAxfDc3OGFhMWZhfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 而在随机性能方面，三星980PRO再次给了我们惊喜。在QD=32，Thread=16的随机测试中，读写双双突破百万



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzAzfGZiMjU4OTYxfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)


 无论是980PRO还是HOF EXTREME，这样的高性能SSD在Rocket Lake S平台上都能够得到完美的发挥。虽然Intel的PCI-E 4.0来的比竞争对手晚了差不多两年，但却有着一点后来居上的意思

> **虽有进步但仍需努力**

 综合上面的测试，我们能够看得出来这次Rocket Lake还是有些不少干货的，IPC的提高使得8核打10核的好戏频频上演。同为8核心处理器，11900K还是要好于对手的5800X，这多少为Intel在高端桌面领域挣回了一些颜面。但不要忘了5800X只是Ryzen 5000系列的三当家，上面还有16核和12核的大哥二哥，目前Intel还不能够拿出相应的竞品来与其抗衡

冰冻三尺非一日之寒，AMD也是经过Ryzen系列三代架构的沉淀加上台积电7nm工艺的加成才有了今天的咸鱼翻身。指望着Rocket Lake S一招便能来力挽狂澜是不现实。要想拿回失去的性能王座还任重道远

 不过从Intel对第10和11代处理器的定价策略上来看，Intel是打算走性价比路线了。没有集显的11400F、11600KF这些CPU在大批量上市之后很有可能会直接接替其前辈们的市场定位及价格，这在AMD的走代工路线成本居高不下的时候也是一个不错的切入点

 6年的14nm就此落幕，Intel也在这最终乐章中拿出来了14nm的最高水平。虽然力有未逮但也给人们看到了希望，希望蓝色巨人能够持续努力，为玩家们奉献出更出色的产品



![下载附件](https://image1.koolcenter.com/forum.php?mod=attachment&aid=NDM0NzYwfDkyNDMwZjNlfDE2MzIzOTAxODZ8MHwxOTM4Mjk%3D&nothumb=yes)

