---
title: "RT-AX89X 官改固件"
linkTitle: "RT-AX89X [高通]"
type: docs
weight: 1
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_23012，更新日期：2021年07月28日
---

---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

---

### <font color="#f57332">〇、前言</font>
华硕RT-AX89X是华硕高端路由里唯一的一款以高通SoC为基础的机器，其搭载了性能强劲、工艺先进的高通IPQ8074 SoC，官方名全称为：IPQ8074 Wi-Fi Access Point SoC，是集CPU、Wi-Fi、网络交换、电源管理芯片为一体的SoC，SoC中的的CPU为四核 ARM Cortex A53，14 nm FinFET工艺，主频2.2GHz。RT-AX89X同时搭载了QCN5024 2.4G无线芯片，可提供4个802.11ax空间流，在AX模式下最高速率为1150Mbps，双QCN5054 5G无线芯片，一起可以可以实现80MHz频宽下8个空间流，或者160MHz频宽下4个空间流，在AX协议下，最高速率为4804Mbps。

如此高规格且性能强劲的路由器，现在终于迎来了其首个第三方固件：`koolshare官改固件`！koolshare固件的最大特点：软件中心，也可以在高通机型RT-AX89X上使用了！当然，一如既往的，koolshare官改固件和软件中心是免费提供的。

下面是我对RT-AX89X进行固件开发的时候，整理的一些信息：
1. RT-AX89X固件平台为qca-ipq806x，其采用的是uclibc作为c库，所以这次固件体积会比华硕hnd/axhnd/axhnd,675x机型的固件小很多，运行程序时对内存占用也会少一些。
2. 虽然IPQ8074为四核ARM Cortex A53，是armv8架构，但是RT-AX89X的固件内核是32位的，所以其固件内显示armv7l。
3. RT-AX89X的jffs分区大小为125.3M，仍然挂载在/jffs目录，但是分区格式不是jffs2，而是ubifs，这应该是华硕第一款jffs分区采用ubifs格式。
4. 因为采用的高通平台，所以固件里既没有博通的vlanctl，也没有以前的robocfg工具来实现简易的VLAN配置，所以软件中心中心中【上海IPTV】暂时没法移植过来
5. RT-AX89X的WiFi区域只有3个：亚洲、澳大利亚、默认值，测试得知发现澳大利亚和亚洲均为30dbm的发射功率，不过亚洲地区是全信道，澳大利亚的信达和默认值一样。亚洲地区5G选149信道功率为30dbm，选36信道则为23dbm，澳大利亚地区不管是36信道还是149信道，都能达到30dbm的功率。RT-AX89X有如此功率，所以【wifi boost】插件也就不需要了。
6. 至于【servcerchan微信推送】【routerhook】【pushplus】插件，因为高通平台很多参数的获取都和博通不一样了，所以还涉及到不少的修改工作，所以这个插件暂时还没有上架（384_82800）。
7. 其它的一些插件，比如迅游加速，花生壳内网版，这些还需要开发插件的厂家进行进一步的二进制适配后才能运行在RT-AX89X上。

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>
> 官改固件的开发初衷是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。
> 
> 所以：**官改固件 = 官方固件 + 为了软件中心进行必要的最小化改动 + 软件中心**

1. 使用官方固件源代码为基础修改，官方固件有的功能官改固件都有，比如AiMesh等；
2. koolshare软件中心支持，RT-AX89X为qca-ipq806x平台，软件中心代号为：[qcasoft](https://github.com/koolshare/qcasoft)。

---

### <font color="#f57332">三、支持机型</font>
> - 本固件仅支持华硕`RT-AX89X`机型，其它机型请勿使用本固件！

---

###  <font color="#f57332">三、更新日志</font>

#### <font color="###00BFFF">386_23012（2021年07月28日）</font>

1. 同步ASUS最新RT-AX89X源代码：`GPL_RT_AX89X_300438623012`；
2. 更新内置软件中心为最新版本：1.2.6；

#### <font color="###00BFFF">386_22790（2020年11月30日）</font>
> 华硕RT-AX89X成为第一批大版本从384迈入386的机型，版本号为：386_22790，和RT-AX89X 386公开测试版本RC1比较接近，所以其功能上稍微弱于RC2，目前并没有speedtest网络测速。386版本最重要的特性就是华硕AiMesh升级为AiMesh 2.0，并且有一系列底层组件的更新。

1. 同步ASUS最新RT-AX89X源代码：`GPL_RT_AX89X_300438622790`；
2. 更新内置软件中心为最新版本：1.2.2；

#### <font color="###00BFFF">384_82800（2020年09月29日）</font>
1. RT-AX89X第一个正式发布的官改版本，基于华硕最新GPL代码：`GPL_RT_AX89X_300438482800` 制作；
2. 关闭固件自动更新功能，以免用户更新到华硕官方固件而失去软件中心等功能；
3. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】；
4. 固件首页默认显示CPU、内存、以太网接口的使用状态，而不是无线网络设置和相关信息；
5. 去除华硕固件后台web使用哥特（Gothic）风格字体，因为其显示中文的时候字体严重发虚；
6. 现在使用ZenWiFi AX6600官改固件作为`AiMesh节点`时，其web后台能正常访问了！
7. 添加koolshare软件中心支持，以及插件需要的必要的内核组件和busybox组件等。
8. 移植了hnd软件中心的多数插件，插件使用方法基本不变。

### <font color="#f57332">五、刷机步骤</font>
- 约定`原厂固件`为RT-AX89X华硕官方固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方RT-AX89X源代码](https://www.asus.com.cn/Networking/RT-AX89X/HelpDesk_Download/)修改而来的带软件中心的[RT-AX89X官改固件](https://koolshare.cn/thread-188090-1-2.html)。

#### <font color="###00BFFF">A. 原厂 刷 官改：</font>
1. 在原产固件的固件升级页面下直接上传.trx 后缀的RT-AX89官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成（如无特殊说明，刷机完成后不需要恢复出产设置，当然恢复一次更好）；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本后即可使用。

#### <font color="###00BFFF">B. 官改 刷 官改：</font>
1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.trx后缀的RT-AX89X官改固件文件即可（如无特殊说明，刷机完成后不用恢复出产设置）；
2. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="###00BFFF">C. 官改 刷 原厂</font>
1. 在官改固件升级页面下直接上传.trx 后缀的原产固件文件（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如果需要彻底清空jffs分区里的软件中心文件残留，需要再执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框）；或者参见后文【<font color="#f57332">**重要命令/操作**</font>】中的【<font color="#DC143C">**清空jffs空间**</font>】或者【<font color="#DC143C">**删除软件中心**</font>】。

### <font color="#f57332">六、注意事项：</font>
1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（ctrl + F5）后重试；
2. 强烈建议使用Chrome浏览器或者Chromium内核的浏览器，以保持最佳兼容性；
3. 刷回官方固件后，单纯的恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。
4. 由于固件来自官改，jffs分区是默认开启的，没有格式化jffs分区的选项，如果需要重置软件中心（不影响jffs分区其它数据），请登录ssh后运行<font color="#DC143C">**软件中心重置命令**</font>（见下文：重要命令）
5. 如果需要清除jffs分区的所有文件（适用于jffs空间不足），使用ssh软件，登录后运行<font color="#DC143C">**释放jffs空间命令**</font>（见下文：重要命令部分）
6. <font color="#DC143C">**请不要使用离线安功能装来安装其它软件中心平台的任何插件，不然肯定会造成问题！！！给RT-AX89X离线安装插件一定要是qca平台的机器的插件（目前该平台仅有RT-AX89X一款），详情见下文FAQ：Q1**</font>

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年09月29日

**Q1：我手动安装第三方xxx插件失败怎么办？**

**A1：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。
1. 目前对于qca-ipq806x平台来说，仅有RT-AX89X这一款机型，其它平台的插件是不能安装在RT-AX89X上的。
2. 除非你要安装的插件作者明确表示他的插件可以用于qca-ipq806x平台软件中心，或者插件来源于qcasoft项目内本身的插件，才可以安装！！
3. 具体来说，目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd软件中心](https://github.com/koolshare/rogsoft)，[qca软件中心](https://github.com/koolshare/qcasoft)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！即使他们可能都使用了1.5代软件中心！！具体各个不同平台的软件中心的区别，大家可以参考此处：[koolshare几个版本的软件中心区别](https://github.com/koolshare/qcasoft#koolshare几个版本的软件中心区别)。

**Q2：软件中心一直显示更新中怎么办？**

**A2：** 此问题可能由多种原因导致，请尝试下面的方法：
1. 访问[https://qcasoft.ddnsto.com/](https://qcasoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。<font color="#DC143C">1）</font>：可能是本地网络故障，通过putty、xshell等SSH软件连接路由器后，输入命令：`ping qcasoft.ddnsto.com`看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定。<font color="#DC143C">2）</font>：也可能是软件中心服务器正在维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考<font color="#DC143C">**重启软件中心命令**</font>（见下文：重要命令部分）。
3. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考<font color="#DC143C">**软件中心重置方法**</font>（见下文：重要命令部分）。
4. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考参考<font color="#DC143C">**RT-AX89X查询坏块命令**</font>（见下文：重要命令部分）。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q3：刷机后软件中心一片空白**

**A3：** 按照下面的顺序依次尝试：
1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep /jffs`，如果看到类似`/dev/ubi0_5 on /jffs type ubifs (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/ubi0_5`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载RT-AX89X的jffs分区：`mount -t ubifs -o rw,noatime /dev/ubi0_5 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：**重要命令**里的软件中心重置命令，来重置一次软件中心，如果没有其它问题，那么应该就能看到软件中心页面了。

**Q4：华硕发了RT-AX89X新固件，为什么此帖还不更新官改固件啊？**

**A4**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q5：我的xxx版本固件无线有问题，能否修复？**

**A5**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q6：可不可给固件以增加xxx功能？**

**A6**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q7：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A7：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

### <font color="#f57332">八、重要命令</font>

#### <font color="###00BFFF">1. 软件中心重置命令</font>

- 直接在ssh客户端内运行`koolshare-reset`命令即可。

#### <font color="###00BFFF">2. 释放jffs空间</font>
- 注意，此操作会删除jffs分区内的所有文件，包括但不限于：软件中心、安装的证书、TrafficAnalyzer的数据库、自定义的设备图标等
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/.sys /jffs/.wtfast /jffs/*
reboot
```

#### <font color="###00BFFF">3. 删除软件中心</font>
- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件。
- 如果是在**官改固件**下删除软件中心，重启路由，路由会自动重新安装软件中心。
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db /jffs/config/* /jffs/etc/profile
reboot
```

#### <font color="###00BFFF">4. 重启软件中心</font>
- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
cd /koolshare/perp
sh perp.sh stop
sh perp.sh start
```

#### <font color="###00BFFF">5. RT-AX89X查询坏块命令</font>
- 运行以下命令，返回数字即为坏块数量
```bash
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

#### <font color="#DC143C"> **386_23012**</font>

MD5: 796D23E36967A86FA3ACA8D50570F63C

SHA1: 12BF67A7C1A2FA46D5C414E0447EEDFC53E98BD1

下载链接：[RT-AX89X_386_23012](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX89X/RT-AX89X_386_23012_koolshare.trx)

#### <font color="#DC143C"> **386_22790**</font>
MD5: B24F4D2D2F97CCE4E941830AB1A5CFD4

SHA1: 2E56B3108F449DFF0A0437824B254E57019AAF55

下载链接：[RT-AX89X_386_22790](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX89X/RT-AX89X_386_22790_koolshare.trx)

#### <font color="#DC143C"> **384_82800**</font>
MD5: A170543CC129CA938F982BDA0DEE5D4E

SHA1: 87EDBAD1D2E4E0E19D359C0A4420E8AAF405E417

下载链接：[RT-AX89X_384_82800](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX89X/RT-AX89X_384_82800_koolshare.trx)
