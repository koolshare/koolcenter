---
title: "ZenWiFi AX6600 官改固件"
linkTitle: "ZenWiFi AX6600"
type: docs
weight: 70
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_25524，更新日期：2020年09月17日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件主要特色</font>
> 官改固件的开发初衷是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。
> 
> 所以：**官改固件 = 官方固件 + 为了软件中心进行必要的最小化改动 + 软件中心**

1. 使用官方固件源代码为基础修改，官方固件有的功能官改固件都有，比如AiMesh等；
2. koolshare软件中心支持，ZenWiFi AX6600为axhnd.675x平台，兼容hnd/axhnd平台软件中心和所有32位插件。

### <font color="#f57332">三、支持机型</font>
> `ZenWiFi AX` 、`ZenWiFi AX (XT8)`、`ZenWiFi AX6600`、`灵耀 AX6600`、`RT-AX95Q`这几个名字代表的都是这一个路由器，大概情况如下：
> 
> - `ZenWiFi AX` 是目前386_25524版本固件左上角显示的名字；
> - `ZenWiFi AX (XT8) `是华硕英文/全球官方网站上该机型的名字，在固件名中也可能见到这个名称；
> - `ZenWiFi AX6600`是华硕中文官网上该机型的名字；
> - `灵耀AX6600`是其中文名，狗东x宝上会看到该名字，刷[386-RC2 beta](https://koolshare.cn/thread-187638-1-1.html)固件后左上角显示该名字；
> - `RT-AX95Q`是路由器内部/GPL代码中该机型的代号，在固件名中也可能见到这个名称；

> 一个路由5个名字，我已经晕了。所以为了本帖方便称呼，本帖主要使用`ZenWiFi AX6600`这个名字，也有可能会使用`RT-AX95Q`。

- 本固件仅支持华硕`ZenWiFi AX6600`机型，其它机型请勿使用本固件！

###  <font color="#f57332">四、更新日志</font>

#### <font color="##00BFFF">386_25524（2020年09月17日）</font>
1. ZenWiFi AX6600第一个官改版本，基于华硕最新GPL代码：`GPL_ZenWIFI_XT8_300438625524` 制作；
2. 关闭固件自动更新功能，以免用户更新到华硕官方固件而失去软件中心等功能；
3. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】；
4. 固件首页默认显示CPU、内存、以太网接口的使用状态，而不是无线网络设置和相关信息；
5. 去除华硕固件后台web使用哥特（Gothic）风格字体，因为其显示中文的时候实在太丑；
6. 现在使用ZenWiFi AX6600官改固件作为`AiMesh节点`时，其web后台能正常访问了！
7. 添加koolshare软件中心支持，以及插件需要的必要的内核组件和busybox组件。

### <font color="#f57332">五、刷机步骤（请仔细阅读）：</font>
- 约定`原厂固件`为华硕官方的ZenWiFi AX6600固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方ZenWiFi AX6600源代码](https://www.asus.com.cn/Networking/ZenWiFi-AX6600/HelpDesk_Download/)修改而来的带软件中心的[官改固件](https://koolshare.cn/thread-187704-1-1.html)。

> - ZenWiFi AX6600 刷机时，节点和路由最好保持一致的版本号，建议先刷`AiMesh节点`，再刷`AiMesh路由`。
> - 如果AiMesh节点是官方固件，AiMesh路由是对应版本的koolshare改版固件，也是没问题的。
> - 如果刷了ZenWiFi AX6600 beta固件，比如[386-RC2 beta](https://koolshare.cn/thread-187638-1-1.html)，再刷回ks官改固件后，建议做一次恢复出厂设置。

#### <font color="##00BFFF">A. 原厂 刷 官改：</font>
1. 在原产固件的固件升级页面下直接上传.w 后缀的ZenWiFi AX6600官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### <font color="##00BFFF">B. 官改 刷 官改：</font>
1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.w 后缀的官改固件文件即可（如无特殊说明，刷机完成后不用恢复出产设置）；
2. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="##00BFFF">C. 官改 刷 原厂</font>
1. 在官改固件升级页面下直接上传.w 后缀的原产固件文件（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如果需要彻底清空jffs分区里的软件中心文件残留，需要再执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框）；或者参见后文【<font color="#f57332">**重要命令/操作**</font>】中的【<font color="#DC143C">**清空jffs空间**</font>】或者【<font color="#DC143C">**删除软件中心**</font>】。

### <font color="#f57332">六、注意事项：</font>
1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（ctrl + F5）后重试；
2. 强烈建议使用Chrome浏览器或者Chromium内核的浏览器，以保持最佳兼容性；
3. 单纯的恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。
4. 由于固件来自官改，jffs分区是默认开启的，没有格式化jffs分区的选项，如果需要重置软件中心（不影响jffs分区其它数据），请登录ssh后运行<font color="#DC143C">**软件中心重置命令**</font>（见下文：重要命令）
5. 如果需要清除jffs分区的所有文件（适用于jffs空间不足），使用ssh软件，登录后运行<font color="#DC143C">**释放jffs空间命令**</font>（见下文：重要命令部分）
6. ZenWiFi AX6600的jffs空间只有47MB，如果开启Traffic Analyzer，将会消耗不少空间，请酌情开启；
7. <font color="#DC143C">**请不要使用离线安功能装来安装AM380固件的任何插件，不然肯定会造成问题！！！给ZenWiFi AX6600离线安装插件一定要是hnd/axhnd平台的机器的插件（目前包括：RT-AC86U、GT-AC5300、RT-AX88U、GT-AX11000、TUF-AX3000、ZenWiFi AX6600、ZenWiFi_XD4等），详情见下文FAQ：Q2**</font>

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年09月17日

**Q1：我的路由器搜不到wifi信号。**

**A1：** 首先排除网络客户端设备的问题，然后请尝试下面的方法：
1. 论坛常有人推荐将wifi区域切换到其它地区来改善信号强度，但是由于每个国家设备支持的信道不同，加上一些终端设备信道支持的限制，就可能会导致某些设备无法搜索到wifi信号。建议：1 在哪个国家就使用哪国的信道设置，2 如果一定要更改WiFi地区，可以使用澳大利亚，因为澳大利亚地区的信道和中国是一样的。
2. 搜不到wifi信号的时候，在路由器管理界面**【无线网络】**-**【一般设置】**中查看到该信号的信道变成了**0**，这首先可能是无意间或者某个未知错误导致该wifi信号被关闭（**【无线网络】**-**【专业设置】**-**【启用无线网络】**处于**否**状态），另一种可能是虽然无线是启用状态，但是当前信道仍然显示为0，遇到此情况建议设置固定信道看是否能解决。如果无论如何都无法解决，建议你走售后渠道更换机器。

**Q2：我手动安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。
1. 目前对于hnd/axhnd/axhnd.675平台的机型：RT-AC86U，GT-AC5300，RT-AX88U，GT-AX11000，RT-AX86U，TUF-AX3000，RT-AX82U、ZenWiFi AX6600/RT-AX95Q、ZenWiFi\_XT4/RT-AX56_XT4这几款机器在本论坛的固件，插件是可以通用的。（具体请见[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)）
2. 除非你要安装的插件作者明确表示他的插件可以用于hnd/axhnd/axhnd.675平台软件中心，或者插件来源于rogsoft项目内本身的插件，才可以安装！！
3. 具体来说，目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd/axhnd软件中心](https://github.com/koolshare/rogsoft)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！即使他们可能都使用了1.5代软件中心！！具体各个不同平台的软件中心的区别，大家可以参考此处：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)。

**Q3：软件中心一直显示更新中怎么办？**

**A3：** 此问题可能由多种原因导致，请尝试下面的方法：
1. 访问[https://rogsoft.ddnsto.com/](https://rogsoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。<font color="#DC143C">1）</font>：可能是本地网络故障，通过putty、xshell等SSH软件连接路由器后，输入命令：`ping armsoft.ddnsto.com`看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定。<font color="#DC143C">2）</font>：也可能是软件中心服务器正在维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考<font color="#DC143C">**重启软件中心命令**</font>（见下文：重要命令部分）。
3. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考<font color="#DC143C">**软件中心重置方法**</font>（见下文：重要命令部分）。
4. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考参考<font color="#DC143C">**ZenWiFi AX6600查询坏块命令**</font>（见下文：重要命令部分）。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：刷机后软件中心一片空白**

**A4：** 按照下面的顺序依次尝试：
1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载ZenWiFi AX6600的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：**重要命令**里的软件中心重置命令，来重置一次软件中心。然后基本上就能看到软件中心页面了。

**Q5：华硕发了ZenWiFi AX6600固件，为什么此帖还不更新官改固件啊？**

**A5**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的xxx固件无线有问题，能否修复？**

**A6**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：可不可给固件以增加xxx功能？**

**A7**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

### <font color="#f57332">八、重要命令</font>
#### <font color="##00BFFF">1. 软件中心重置命令</font>

- 直接在ssh客户端内运行`koolshare-reset`命令即可。

#### <font color="##00BFFF">2. 释放jffs空间</font>
- 注意，此操作会删除jffs分区内的所有文件，包括但不限于：软件中心、安装的证书、TrafficAnalyzer的数据库、自定义的设备图标等
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/.sys /jffs/.wtfast /jffs/*
reboot
```

#### <font color="##00BFFF">3. 删除软件中心</font>
- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件。
- 如果是在**官改固件**下删除软件中心，重启路由，路由会自动重新安装软件中心。
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db /jffs/config/* /jffs/etc/profile
reboot
```

#### <font color="##00BFFF">4. 重启软件中心</font>
- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
cd /koolshare/perp
sh perp.sh stop
sh perp.sh start
```

#### <font color="##00BFFF">5. ZenWiFi AX6600查询坏块命令</font>
- hnd/axhnd机型上查询坏块的方法已经不适用于axhnd.675x平台
- axhnd.675x平台查询坏块的命令如下（适用于`RT-AX86U`、`RT-AX82U`、`TUF-AX3000`、`ZenWiFi AX6600`、`ZenWiFi_XD4`等axhnd.675x平台机型）：
```bash
# 运行以下命令，返回数字即为坏块数量
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

#### <font color="#DC143C"> **386_25524**</font>

MD5: BBFA6E7043FA68C56D43E40DD7D6FECB

SHA1: 4360C7DEA2D14B2C9A5A37EFD651B6AB2D81EE27

下载链接：[RT-AX95Q_386_25524_koolshare_cferom_pureubi.w](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/ZenWiFi_AX6600/T-AX95Q_386_25524_koolshare_cferom_pureubi.w)
