---
title: "RT-AX82U 官改固件"
linkTitle: "RT-AX82U"
type: docs
weight: 50
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_41700，更新日期：2021年06月20日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>
> 官改固件的开发初衷是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。详情FAQ: Q7。
> 
> 所以：**官改固件 = 官方固件 + 为了软件中心进行必要的最小化改动 + 软件中心**

1. 使用官方固件源代码为基础修改，官方固件有的功能官改固件都有，比如AiMesh等；
2. koolshare软件中心支持，RT-AX82U为axhnd.675x平台，兼容hnd/axhnd平台软件中心和所有32位插件。

### <font color="#f57332">三、支持机型</font>
- 本固件仅支持华硕`RT-AX82U`机型，其它机型请勿使用本固件！
- 本固件同样支持 `RT-AX82U高达限量版`，此版本机器请刷`384_9617`及更新版本，固件定制UI将不会丢失。

###  <font color="#f57332">四、更新日志</font>

#### <font color="###00BFFF">386_41700（2021年06月20日）</font>

> 从此版本开始，华硕RT-AX82U官改固件正式进入386大版本，在功能上，该版本主要更新了AiMesh 2.0和Ookla® SPEEDTEST，当然也包含很多其它稳定性、安全性方面的更新。强烈建议大家进行升级！
> 从384固件升级到386固件也是非常顺畅的，升级后不恢复出厂设置也是没问题的。当然稳妥起见，建议有时间的朋友还是做一次恢复出厂设置，然后在干净的配置上重新手动配置一次固件。

1. 同步ASUS最新RT-AX82U官方固件源代码：3.0.0.4.386.41700。
2. 内置软件中心版本更新至1.7.1版本；

#### <font color="###00BFFF">384_9617（2020年07月26日）</font>

1. 同步ASUS最新RT-AX82U代码：GPL\_RT\_AX82U\_30043849617；
2. 关闭固件强制自动更新功能，以免用户更新到ASUS官方固件而失去软件中心功能；
3. 更新内置koolshare软件中心到1.6.1版本；
4. 修复AX82U官改固件作为`AiMesh路由`时，无法为同样是官改固件的AiMesh节点更新固件的问题；
5. 现在AX82U官改固件作为`AiMesh节点`时，其web后台也能正常访问了！

> **针对384\_9617第`5`点更新的说明如下，请仔细阅读：**
> - 华硕对AiMesh节点仅开放了固件更新这一个页面功能，这限制得太多了，但是这也是为了避免用户对节点进行设置造成mesh网络出问题；
> - kooldev将AiMesh节点的web后台访问全部开放了，但是需要提醒大家请尽量不要改动与AiMesh相关的设定，以免影响AiMesh网络的正常工作；
> - 我们开放AiMesh节点的web后台的访问，主要目的是为了大家能在AiMesh节点中使用软件中心，当然你也可以进行一些固件相关的设定，比如无线区域。
> - 需要注意的是因为AiMesh节点本质上是工作在中继模式，而非NAT模式，所以一些透明代理类的插件在AiMesh节点路由上是无法正常工作的，，比如`xx上网`，`kp`，`迅游加速器`等；
> - 如果你在AiMesh节点中修改了某些系统设置导致AiMesh网络失效，请在开机状态下长按机器后面的`reset`按钮重置你的AiMesh节点路由，然后用主路由重新添加节点；
> - AiMesh节点web后台的访问方式：在AiMesh主路由的【网络地图】页面点击【AiMesh节点】图标，然后在页面右侧会出现目前已经连接的AiMesh节点，点击对应节点机器后，会弹出节点信息，信息中会显示该节点机器的ip地址，比如我的是`192.168.86.78`，然后在浏览器中访问http://192.168.86.78即可访问AiMesh节点路由。

#### <font color="###00BFFF">384_9411（2020年06月29日）</font>
> RT-AX82U官方的第一个固件版本号为：384.9385，此官改固件基于更新的384.9411版本制作~

1. RT-AX82U第一个官改版本，基于华硕GPL代码：`GPL_RT-AX82U_3.0.0.4.384.9411` 制作；
2. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】。
3. 添加koolshare软件中心支持。

### <font color="#f57332">五、刷机步骤</font>
- 约定`原厂固件`为华硕官方的RT-AX82U固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方RT-AX82U源代码](https://www.asus.com/Networking/RT-AX82U/HelpDesk_Download/)修改而来的带软件中心的[官改固件](https://koolshare.cn/thread-181845-1-1.html)。
#### <font color="###00BFFF">A. 原厂 刷 官改：</font>
1. 在原产固件的固件升级页面下直接上传.w 后缀的RT-AX82U官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### <font color="###00BFFF">B. 官改 刷 官改：</font>
1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.w 后缀的官改固件文件即可（如无特殊说明，刷机完成后不用恢复出产设置）；
2. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="###00BFFF">C. 官改 刷 原厂</font>
1. 在官改固件升级页面下直接上传.w 后缀的原产固件文件（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如果需要彻底恢复，执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框）；或者参见后文【<font color="#f57332">**重要命令/操作**</font>】中的【<font color="#DC143C">**清空jffs空间**</font>】或者【<font color="#DC143C">**删除软件中心**</font>】。

### <font color="#f57332">六、注意事项：</font>
1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（cttrl + F5）后重试；
2. 强烈建议使用chrome浏览器或者chrome内核的浏览器，以保持最佳兼容性；
3. 恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。
4. 由于固件来自官改，jffs分区是默认开启的，没有格式化软件中心的选项，如果需要重置软件中心（不影响jffs分区其它数据），请登录ssh后运行<font color="#DC143C">**软件中心重置命令**</font>（见下文：重要命令）
5. 如果需要清除jffs分区的所有文件（适用于jffs空间不足），使用ssh软件，登录后运行<font color="#DC143C">**释放jffs空间命令**</font>（见下文：重要命令部分）
6. RT-AX82U的jffs空间只有47MB，如果开启Traffic Analyzer，将会消耗不少空间，请酌情开启；
7. <font color="#DC143C">**请不要使用离线安功能装来安装AM380固件的任何插件，不然肯定会造成问题！！！给RT-AX82U离线安装插件一定要是hnd/axhnd平台的机器的插件（目前包括：RT-AC86U，GT-AC5300，RT-AX88U，GT-AX11000，TUF-AX3000等），详情见下文FAQ：Q3**</font>

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年07月26日

**Q1：我的路由器搜不到wifi信号。**

**A1：** 首先排除网络客户端设备的问题，然后请尝试下面的方法：
1. 论坛常有人推荐将wifi区域切换到澳大利亚地区来改善信号强度，这确实管用，因为澳大利亚区域的最大发射功率要大一些。但是由于每个国家设备支持的信道不同，加上一些终端设备信道支持的限制，就可能会导致某些设备无法搜索到wifi信号。建议：1 在哪个国家就使用哪国的信道设置，2 如果一定要使用澳大利亚，请经信道固定在国内支持的信道范围。
2. 搜不到wifi信号的时候，在路由器管理界面**【无线网络】**-**【一般设置】**中查看到该信号的信道变成了**0**，这首先可能是无意间或者某个未知错误导致该wifi信号被关闭（**【无线网络】**-**【专业设置】**-**【启用无线网络】**处于**否**状态），另一种可能是虽然无线是启用状态，但是当前信道仍然显示为0，遇到此情况建议设置固定信道看是否能解决。如果无论如何都无法解决，建议你走售后渠道更换机器。

**Q2：我手动安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。
1. 目前对于hnd/axhnd/axhnd.675平台：RT-AC86U，GT-AC5300，RT-AX88U，GT-AX11000，RT-AX82U，TUF-AX3000，RT-AX82U这几款机器在本论坛的固件，插件是可以通用的。（具体请见[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)）
2. 除非你要安装的插件作者明确表示他的插件可以用于hnd/axhnd/axhnd.675平台软件中心，或者插件来源于rogsoft项目内本身的插件，才可以安装！！
3. 具体来说，目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd/axhnd软件中心](https://github.com/koolshare/rogsoft)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！即使他们可能都使用了1.5代软件中心！！具体各个不同平台的软件中心的区别，大家可以参考此处：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)。

**Q3：软件中心一直显示更新中怎么办？**

**A3：** 此问题可能由多种原因导致，请尝试下面的方法：
1. 访问[https://rogsoft.ddnsto.com/](https://rogsoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。<font color="#DC143C">1）</font>：可能是本地网络故障，通过putty、xshell等SSH软件连接路由器后，输入命令：`ping armsoft.ddnsto.com`看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定。<font color="#DC143C">2）</font>：也可能是软件中心服务器正在维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考<font color="#DC143C">**重启软件中心命令**</font>（见下文：重要命令部分）。
3. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考<font color="#DC143C">**软件中心重置方法**</font>（见下文：重要命令部分）。
4. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考参考<font color="#DC143C">**RT-AX82U查询坏块命令**</font>（见下文：重要命令部分）。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：刷机后软件中心一片空白**

**A4：** 按照下面的顺序依次尝试：
1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载RT-AX82U的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock8 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：**重要命令**里的软件中心重置命令，来重置一次软件中心。然后基本上就能看到软件中心页面了。

**Q5：华硕发了RT-AX82U固件，为什么此帖还不更新官改固件啊？**

**A5**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的xxx固件无线有问题，能否修复？**

**A6**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：可不可给固件以增加xxx功能？**

**A7**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

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
#### <font color="###00BFFF">5. RT-AX82U查询坏块命令</font>
- hnd/axhnd机型上查询坏块的方法已经不适用于axhnd.675x平台
- axhnd.675x平台查询坏块的命令如下（适用于`RT-AX86U`、`RT-AX82U`、`TUF-AX3000`等axhnd.675x平台机型）：
```bash
# 运行以下命令，返回数字即为坏块数量
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

#### <font color="#DC143C"> **386_41700**</font>

MD5: 15BB4E0972F2A81C4FF2DD0634D57930

SHA1: 4097CA62F960BFF76898BCDB8BC436FA564CF903

下载链接：[RT-AX82U_386_41700](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/RT-AX82U/RT-AX82U_386_41700_koolshare_cferom_pureubi_f004e11.w)

#### <font color="#DC143C"> **384_9617**</font>

MD5: AA64E6A3787DDBAA08D9D8FC7F23CB6B

SHA1: 4097CA62F960BFF76898BCDB8BC436FA564CF903

下载链接：[RT-AX82U_384_9617](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/RT-AX82U/RT-AX82U_384_9617_koolshare_cferom_pureubi.w)

#### <font color="#DC143C"> **384_9411**</font>

MD5: 52AA492474661466455F9B19269931E0

SHA1: 67DCC477EE8925560B0E29D1DEA61F35BB039BCD

下载链接：[RT-AX82U_384_9411](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/RT-AX82U/RT-AX82U_384_9411_koolshare_cferom_pureubi.w)
[/hide]

