---
title: "TUF-AX3000 华硕官改固件"
linkTitle: "TUF-AX3000"
type: docs
weight: 10
toc_hide: false
hide_summary: false
date: 2021-09-11
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_41700，更新日期：2021年04月09日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>

1. 使用官方固件源代码为基础修改，官方固件有的功能官改固件都有，比如Aimesh等；

2. koolshare软件中心支持，支持TUF-AX3000独有的橙色皮肤；

3. TUF-AX3000为axhnd.675x平台，兼容hnd/axhnd平台软件中心和所有32位插件。

###  <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕TUF-AX3000机型。

- RT-AX58U、RT-AX3000、RT-AX82U虽然硬件和TUF-AX3000一样，但是固件不通刷。


###  <font color="#f57332">四、更新日志</font>

####  <font color="##00BFFF">386_41700（2021年04月09日）</font>

> 从此版本开始，华硕TUF-AX3000官改固件正式进入386大版本，在功能上，该版本主要更新了AiMesh 2.0和Ookla® SPEEDTEST，当然也包含很多其它稳定性、安全性方面的更新。强烈建议大家进行升级！
> 
> 注意-1：由于TUF-AX3000为橙色TUF主题UI，而华硕单方面在386_41700固件中并未AiMesh2.0功能推出TUF UI，所以AiMesh2.0页面仍然都显示的但是ASUSWRT风格UI。
> 
> 注意-2：TUF-AX3000的SpeedTest功能是有问题的，其web后台【Adaptive QoS 网络监控家】页面并没有【网络速度】标签页访问入口，只能都通过直接访问 http://router.asus.com/Advanced_FirmwareUpgrade_Content.asp 才能使用，且访问都需要更改iframe元素internetSpeed_iframe的高度点才能都正常显示测速界面！
> 
> 从384固件升级到386固件也是非常顺畅的，升级后不恢复出厂设置也是没问题的。当然稳妥起见，建议有时间的朋友还是做一次恢复出厂设置，然后在干净的配置上重新手动配置一次固件。

1. 同步ASUS最新GT-AC5300代码：3.0.0.4.386.41700；
2. 内置软件中心版本更新至1.7.1版本；

####  <font color="##00BFFF"> 384_9923（2020年10月26日）</font>

> 此版本TUF-AX3000支持刺客模式，开启后即可实现完整的5G Wi-Fi6 4T4R。
> 
> 刺客模式的开关等效于在无线网络高级设置中启用澳大利亚。

1. 同步TUF-AX3000固件代码：GPL_TUF_AX3000_30043849923；
2. 更改软件中心数据库文件夹：jffs/db → jffs/ksdb
3. 内置软件中心版本更新至1.6.4版本；
4. 修复在使用ipset-7.6的时候出现问题，导致部分插件无法使用的问题

####  <font color="##00BFFF"> 384_9190（2020年08月27日）</font>

1. 同步TUF-AX3000固件代码：GPL_TUF_AX3000_30043849190；
2. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】;
3. ipset 6.3.1升级为ipset 7.6版本；
4. 内置软件中心版本更新至1.6.1版本；
5. 修复TUF-AX3000官改固件作为`AiMesh路由`时，无法为同样是官改固件的AiMesh节点更新固件的问题；
6. 现在TUF-AX3000官改固件作为`AiMesh节点`时，其web后台也能正常访问了！

> **针对384\_9190第`6`点更新的说明如下，请仔细阅读：**
>
> - 华硕对AiMesh节点仅开放了固件更新这一个页面功能，这限制得太多了，但是这也是为了避免用户对节点进行设置造成mesh网络出问题；
> - kooldev将AiMesh节点的web后台访问全部开放了，但是需要提醒大家请尽量不要改动与AiMesh相关的设定，以免影响AiMesh网络的正常工作；
> - 我们开放AiMesh节点的web后台的访问，主要目的是为了大家能在AiMesh节点中使用软件中心，当然你也可以进行一些固件相关的设定，比如无线区域。
> - 需要注意的是因为AiMesh节点本质上是工作在中继模式，而非NAT模式，所以一些透明代理类的插件在AiMesh节点路由上是无法正常工作的，比如`xx上网`，`kp`，`迅游加速器`等；
> - 如果你在AiMesh节点中修改了某些系统设置导致AiMesh网络失效，请在开机状态下长按机器后面的`reset`按钮重置你的AiMesh节点路由，然后用主路由重新添加节点；
> - AiMesh节点web后台的访问方式：在AiMesh主路由的【网络地图】页面点击【AiMesh节点】图标，然后在页面右侧会出现目前已经连接的AiMesh节点，点击对应节点机器后，会弹出节点信息，信息中会显示该节点机器的ip地址，比如我的是`192.168.30.78`，然后在浏览器中访问http://192.168.30.78即可访问AiMesh节点路由。

####  <font color="##00BFFF"> 384_8137（2020年04月12日）</font>
1. 同TUF-AX3000固件代码：GPL_TUF_AX3000_30043848137；
2. hnd/axhnd软件中心支持，软件中心和插件支持TUF橙色皮肤；

### <font color="#f57332">五、刷机步骤</font>

#### <font color="#00BFFF">刷机准备</font>

- 建议下载好固件后，对固件的md5/sha1校验码进行核对，以保证固件完整性；
- 建议刷机全程使用电脑端谷歌Chrome，或者Chromium内核的浏览器进行操作；
- 如果使用了USB2JFFS插件，建议先使用卸载掉USB的挂载后在进行刷机，刷机后再进行挂载。

#### <font color="#00BFFF">固件定义</font>

- 约定`原厂固件`为华硕官方的TUF-AX3000固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方TUF-AX3000源代码](https://www.asus.com.cn/Networking/TUF-GAMING-AX3000/HelpDesk/)修改而来的带koolshare软件中心的[官改固件](https://koolshare.cn/thread-179968-1-1.html)，版本号为官方固件版本号后加上`_koolshare`后缀，如固件版本：`3.0.0.4.386_41700_koolshare`。

#### <font color="#00BFFF">刷机术语</font>

> 为消除小白在刷机过程中的疑惑，下面列出一下华硕/ML固件刷机的基本术语及我自己的解释，希望对大家有所帮助。如果你对下面的内容已经比较清楚，那么可以跳过这部分直接进入到刷机流程。

1. **固件双清**：双清就是要清除：1. nvram配置，2：JFFS分区文件。固件的很多设置都是储存在nvram中，例如拨号方式、拨号上网帐号密码、无线网络设置等；固件的很多文件是储存在JFFS分区的，例如流量分析储存的流量数据，SSL证书，UU加速器程序等。一般同类型固件互刷不需要进行双清，不同类型固件互刷视情况要进行双清，以保证路由器刷机后处于最佳工作状态。<font color="#FF00CC">如何双清路由器：</font>进入【系统管理 】–【 恢复/导出/上传设置】，勾选恢复按钮旁的选择框，然后点击恢复按钮。
2. **恢复出厂**：恢复出厂就是清除固件的nvram配置，但是不清除JFFS分区文件。这样流量分析、SSL证书等文件并不会丢失。值得注意的是很多朋友有用【导出设置】来备份固件配置的习惯，而在刷固件，特别是不同类型固件互刷的情况下，是不适用使用备份的配置来恢复刚刚进行了恢复出厂的机器的，因为这样就相当于你什么也没恢复。所以请一定不要使用以前备份的配置来恢复刚刷机后，又进行过恢复出厂的路由器。使用【导出设置】备份的配置文件，一般进行了一些设置导致路由器出了问题，将路由器恢复到原厂默认值后，再用备份配置进行恢复，使用备份配置前后，路由器都是同一个版本。<font color="#FF00CC">如何恢复出厂：</font>进入【系统管理 】–【 恢复/导出/上传设置】，点击恢复按钮，记住不要勾选恢复按钮右侧的选择框！！
3. **JFFS挂载状态**：通过SSH连接到路由器后台后输入命令（如果不知道如何使用SSH执行命令，可以参考下文【重要命令】中的【如何使用SSH】）：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。因为软件中心是储存在JFFS中的，所以如果软件中心进入后是空白页面，一般来说JFFS分区的挂载就出现了问题。遇到这种情况，可以参考下文FAQ中的【Q3：刷机后软件中心一片空白】来尝试解决。

#### <font color="#00BFFF">A. 原厂 → 官改：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好

1. 在原产固件的固件升级页面下直接上传.w 后缀的TUF-AX3000官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### <font color="#00BFFF">B. 官改 → 官改：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置

1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.w 后缀的官改固件文件即可!
2. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="#00BFFF">C. 官改 → 原厂</font>

> 如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好

1. 在官改固件升级页面下直接上传.w 后缀的华硕原厂固件文件；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如果需要彻底清空jffs分区里的软件中心文件残留，需要再执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框）

### <font color="#f57332">六、注意事项：</font>

1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（ctrl + F5）后重试；

2. 强烈建议使用Chrome浏览器或者Chromium内核的浏览器，以保持最佳兼容性；

3. 单纯的恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。

4. 由官改固件的JFFS分区是默认开启的，没有格式化jffs分区的选项，如果需要重置软件中心，请参考下文：重要命令里的==软件中心重置==


### <font color="#f57332">七、FAQ</font>

- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年10月25日

**Q1：TUF-AX3000和RT-AX3000、RT-AX58U、RT-AX82U是一样的吗？固件通用吗**

**A1：** 这四款机器硬件上基本是一样的，但是软件和固件上是不一样的，RT-AX3000、RT-AX58U可以刷同一个固件，TUF-AX3000只能刷TUF-AX3000的固件，RT-AX82U只能刷RT-AX82U的固件，这是机器cfe限制的。

**Q2：我手动安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。

1. 本贴的TUF-AX3000属于axhnd.675平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
2. 目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd软件中心](https://github.com/koolshare/rogsoft)，[qca软件中心](https://github.com/koolshare/qca)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！具体可以参考：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)；
3. 对于第三方作者开发的插件，除非作者明确表示其支持hnd/axhnd/axhnd.675平台，不然请不要随意安装！不然因为可能没有遵循开发规范，安装后无法使用，甚至给路由器带来问题！
4. 为了论坛和固件未来更好的发展，koolshare软件中心也会针对一些特殊的插件在离线安装上有所限制。

**Q3：软件中心一直显示更新中怎么办？**

**A3：** 此问题也可以有很多变种，比如：软件中心不显示在线版本号，此问题可能由多种原因导致，请尝试下面的方法：

1. 访问[https://rogsoft.ddnsto.com/](https://rogsoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。
   1. 可能是路由器本地网络故障-1：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`ping rogsoft.ddnsto.com`，看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定后再试；如果能解析ip地址当时无法ping通，可能是本地网络问题或者软件中心服务器正在维护。
   2. 可能是路由器本地网络故障-2：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`curl -sS4L https://rogsoft.ddnsto.com/|grep Hello `，如果显示了两行内容都包含`Hello to everyone`字样，表明路由器访问软件中心web服务器没有问题；如果没有以上显示，可能是本地网络问题或者软件中心服务器正在维护。
   3. 可能是软件中心服务器维护：建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep -w httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考下文：重要命令里的==重启软件中心==。
3. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考下文：重要命令里的==软件中心重置==。
4. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==TUF-AX3000查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：软件中心页面一片空白**

**A4：** 按照下面的顺序依次尝试：

1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载TUF-AX3000的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心。然后基本上就能看到软件中心页面了。

**Q5：华硕发了TUF-AX3000最新固件，为什么此贴还不更新官改固件啊？**

**A5**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的xxx固件无线有问题，能否修复？**

**A6**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：可不可给固件以增加xxx功能？**

**A7**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的。

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

### <font color="#f57332">八、重要命令</font>
> 以下操作需要使用支持SSH协议的软件，连接到路由器后台进行操作，如果不会使用，可以参考下面步骤：
>
> 1. **启用SSH：**在路由器后台的【系统管理】-【系统设置】里，将【启用 SSH】更改为`LAN only`，将端口号设置为`22`或者其它数字，点击页面下方【应用本页面设置】保存更改；
> 2. **登录SSH：**下载SSH软件，如putty（[官方绿色版putty 0.74下载地址](https://the.earth.li/~sgtatham/putty/0.74/w64/putty.exe)），运行后在Host Name（or IP address）处输入路由器的局域网IP地址，如：`192.168.50.1`或者`router.asus.com`，端口为上一步中【SSH 端口】中的端口，如果没有更改，则为`22`，点击【Open】，如果有弹出Putty Security Alert，点击【是】；在界面的`login as`后面输入`路由器的登录帐号`后回车，然后在 password: 提示符后输入`路由器登录密码`后回车（记住：输入密码的时候不会有任何显示，输入完成后直接回车即可），完成登录。
> 3. **键入命令：**键入命令时建议将系统输入法切换为英文，也可以复制命令后使用右键即可粘贴命令，粘贴完毕后按回车即可执行命令。

#### <font color="##00BFFF">1. 软件中心重置</font>

- 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，直接在ssh客户端内运行下面的程序即可。

```bash
koolshare-reset
```

#### <font color="##00BFFF">2. 清空JFFS空间</font>

- 注意，此操作会删除jffs分区内的==所有文件==，包括但不限于：软件中心、SSL证书、自定义的设备图标等；
- 命令运行完毕后路由器会自动重启；
- 如果是在**官改固件**下清空JFFS空间，路由器重启后软件中心会重新初始化为最初状态；
```bash
kill -9 $(pidof skipd)
rm -r .[a-zA-Z_]* *
reboot
```

#### <font color="##00BFFF">3. 删除软件中心</font>
- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件。
- 如果是在**官改固件**下删除软件中心，路由器重启后软件中心会重新初始化为最初状态；
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db /jffs/ksdb /jffs/config/* /jffs/etc/profile
reboot
```

#### <font color="##00BFFF">4. 重启软件中心</font>
- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
sh /koolshare/perp/perp.sh
```

#### <font color="##00BFFF">5. TUF-AX3000查询坏块命令</font>

- hnd/axhnd机型上查询坏块的方法已经不适用于axhnd.675x平台
- axhnd.675x平台查询坏块的命令如下（运行以下命令，返回数字即为坏块数量）：

```bash
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

- 以下固件下载服务器由海波云[Hypo.cn](https://www.hypo.cn/?from=ksbbs) 友情赞助！

#### <font color="#DC143C"> **386_41700**</font>

MD5: 1188418CD391E46B57BAB3F9CF535B6E

SHA1: 7442B34AAA7668295190BDFDA19985B647922CAB

下载链接：[TUF-AX3000_386_41700_koolshare_cferom_pureubi.w](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/TUF-AX3000/TUF-AX3000_386_41700_koolshare_cferom_pureubi.w)


#### <font color="#DC143C"> **384_9923**</font>

MD5: 3028697E3A55176F0DEA5353A65EF046

SHA1: 50A42FF506EAC25C57E3F066689686D015A1E78C

下载链接：[TUF-AX3000_384_9923_koolshare_cferom_pureubi.w](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/TUF-AX3000/TUF-AX3000_384_9923_koolshare_cferom_pureubi.w)

#### <font color="#DC143C"> **384_9190**</font>

MD5: 4005F5A8D16C097F0623EEDC70D0E962

SHA1: 22A17CCDEB047A6566816A7D766B370634DAA07E

下载链接：[TUF-AX3000_384_9190_koolshare_cferom_pureubi.w](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/TUF-AX3000/TUF-AX3000_384_9190_koolshare_cferom_pureubi.w)

#### <font color="#DC143C"> **384_8137**</font>

MD5: 12F62AC210B72E91E3BB281752FA1E3B

SHA1: 28B4A8DFBD2F365165932595878E4357C9135321

下载链接：[TUF-AX3000_384_8137_koolshare_cferom_pureubi.w](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/TUF-AX3000/TUF-AX3000_384_8137_koolshare_cferom_pureubi.w)
