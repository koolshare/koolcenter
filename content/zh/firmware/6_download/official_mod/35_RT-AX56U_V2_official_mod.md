---
title: "RT-AX56U 官改固件"
linkTitle: "RT-AX56U_V2"
type: docs
weight: 40
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_42350，更新日期：2021年06月21日
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
2. koolshare软件中心支持，RT-AX56U_V2为axhnd.675x平台，兼容hnd/axhnd平台软件中心和所有32位插件。

### <font color="#f57332">三、支持机型</font>
本固件仅支持型号为`RT_AX56U_V2`的机型，该机型在华硕官方页面上也会显示为`RT_AX55`，其包含了以下版本：

- RT-AX56U 青春版
- RT-AX56U 热血版
- RT-AX56U 刺客信条黑旗版

<font color="red">**注意：**</font>本固件不支持`RT-AX56U`，具体情况请见下方表格

| 名字              | 机型        | 型号     | USB | FLASH | RAM   | 本固件支持   |
| ----------------- | ----------- | -------- | ------ | ----- | ----- | ------ |
| RT-AX56U          | RT-AX56U    | RT-AX56U | 有     | 256MB | 512MB | **不支持** |
| RT-AX56U 青春版   | RT-AX56U_V2 | RT-AX55  | 无     | 128MB | 256MB | <font color="#33CCFF">**支持**</font> |
| RT-AX56U 热血版   | RT-AX56U_V2 | RT-AX55  | 无     | 128MB | 256MB | <font color="#33CCFF">**支持**</font> |
| RT-AX56U 刺客信条 | RT-AX56U_V2 | RT-AX55  | 无     | 128MB | 256MB | <font color="#33CCFF">**支持**</font> |

###  <font color="#f57332">四、更新日志</font>

#### <font color="#00BFFF">386_42350（2021年06月21日）</font>

> 从此版本开始，华硕RT-AX56U_V2官改固件正式进入386大版本，在功能上，该版本主要更新了AiMesh 2.0和Ookla® SPEEDTEST，当然也包含很多其它稳定性、安全性方面的更新。强烈建议大家进行升级！
> 
> 从384固件升级到386固件也是非常顺畅的，升级后不恢复出厂设置也是没问题的。当然稳妥起见，建议有时间的朋友还是做一次恢复出厂设置，然后在干净的配置上重新手动配置一次固件。
> 
> **注意**：由于固件增加了UU加速器和腾讯网游加速器，固件的内存占用进一步升高！可能会导致一些体积较大的第三方插件无法正常安装！

1. 同步ASUS最新RT-AX56U_V2官方固件源代码：3.0.0.4.386.42350。
2. 内置软件中心版本更新至1.7.1版本；

#### <font color="#00BFFF">384_9822（2020年10月21日）</font>

> 华硕目前官方最新的RT_AX56U_V2固件版本号为：384_9939，而此官改固件基于华硕官方的384_9822源代码制作，而官方的384_9822版本固件存在一些已知问题：
>
> 1. AiMesh功能无法使用
> 2. 固件首页无法显示在线客户端
>
> 这些问题只有等华硕放出了最新的源代码后，官改固件才能同步修复。

1. RT-AX56U_V2第一个官改版本，基于华硕最新GPL代码：`RT-AX56U_V2_30043849822` 制作；
2. 因RT-AX56U_V2的FLASH只有128MB，所以删除一些不必要的文件比如图片等，精简了固件大小；
3. 关闭固件自动更新功能，以免用户更新到华硕官方固件而失去软件中心等功能；
4. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】；
5. 固件首页默认显示CPU、内存、以太网接口的使用状态，而不是无线网络设置和相关信息；
6. 去除华硕固件后台web使用哥特（Gothic）风格字体，因为其显示中文的时候实在太丑；
7. 现在使用RT-AX56U_V2官改固件作为`AiMesh节点`时，其web后台能正常访问了！
8. 添加koolshare软件中心支持，以及插件需要的内核组件、busybox组件、dnsmasq with ipset等。
9. 因为RT-AX56U_V2没有USB接口，所以屏蔽了`aria2`、`易有云`、`易有云2.0`、`虚拟内存`、`usb2jffs`这5个插件。

### <font color="#f57332">五、刷机步骤（请仔细阅读）：</font>
- 约定`原厂固件`为华硕官方的RT-AX56U_V2固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方RT-AX56U_V2源代码](https://www.asus.com.cn/Networking/RT-AX55/HelpDesk_Download/)修改而来的带软件中心的[RT-AX56U_V2官改固件](https://koolshare.cn/thread-188683-1-2.html)。

> - 建议使用chrome浏览器，或者chromium内核的浏览器进行刷机操作。
> - 刷机后如提示手动重启路由器，请等待几分钟后再手动开关电源进行重启。

#### <font color="#00BFFF">A. 原厂 → 官改：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好

1. 在原产固件的固件升级页面下直接上传.w 后缀的RT-AX56U_V2官改固件文件；
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
- FAQ更新日期：2020年10月21日

**Q1：我手动安装第三方xxx插件失败怎么办？**

**A1：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。
1. 本贴的RT-AX56U_V2属于axhnd.675平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
2. 目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd软件中心](https://github.com/koolshare/rogsoft)，[qca软件中心](https://github.com/koolshare/qca)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！具体可以参考：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)；
3. 对于第三方作者开发的插件，除非作者明确表示其支持hnd/axhnd/axhnd.675平台，不然请不要随意安装！不然因为可能没有遵循开发规范，安装后无法使用，甚至给路由器带来问题！
4. 为了论坛和固件未来更好的发展，koolshare软件中心也会针对一些特殊的插件在离线安装上有所限制。

**Q2：软件中心一直显示更新中怎么办？**

**A2：** 此问题也可以有很多变种，比如：软件中心不显示在线版本号，此问题可能由多种原因导致，请尝试下面的方法：
1. 访问[https://rogsoft.ddnsto.com/](https://rogsoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。
   1. 可能是路由器本地网络故障-1：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`ping rogsoft.ddnsto.com`，看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定后再试；如果能解析ip地址当时无法ping通，可能是本地网络问题或者软件中心服务器正在维护。
   2. 可能是路由器本地网络故障-2：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`curl -sS4L https://rogsoft.ddnsto.com/|grep Hello `，如果显示了两行内容都包含`Hello to everyone`字样，表明路由器访问软件中心web服务器没有问题；如果没有以上显示，可能是本地网络问题或者软件中心服务器正在维护。
   3. 可能是软件中心服务器维护：建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep -w httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考下文：重要命令里的==重启软件中心==。
3. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考下文：重要命令里的==软件中心重置==。
4. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==RT-AX56U_V2查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q3：软件中心页面一片空白**

**A3：** 按照下面的顺序依次尝试：
1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载RT-AX56U_V2的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心。然后基本上就能看到软件中心页面了。

**Q4：华硕发了RT-AX56U_V2新固件，为什么此帖还不更新官改固件啊？**

**A4**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到6个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q5：我的RT-AX56U_V2固件无线有问题，能否修复？**

**A5**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q6：可不可给固件以增加xxx功能？**

**A6**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的。

**Q7：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A7：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

### <font color="#f57332">八、重要命令</font>

以下操作需要使用支持SSH协议的软件，连接到路由器后台进行操作，如果不会使用，可以参考下面步骤：
1. **启用SSH：** 在路由器后台的【系统管理】-【系统设置】里，将【启用 SSH】更改为`LAN only`，将端口号设置为`22`或者其它数字，点击页面下方【应用本页面设置】保存更改；
2. **登录SSH：** 下载SSH软件，如putty（[官方绿色版putty 0.74下载地址](https://the.earth.li/~sgtatham/putty/0.74/w64/putty.exe)），运行后在Host Name（or IP address）处输入路由器的局域网IP地址，如：`192.168.50.1`或者`router.asus.com`，端口为上一步中【SSH 端口】中的端口，如果没有更改，则为`22`，点击【Open】，如果有弹出Putty Security Alert，点击【是】；在界面的`login as`后面输入`路由器的登录帐号`后回车，然后在 password: 提示符后输入`路由器登录密码`后回车（记住：输入密码的时候不会有任何显示，输入完成后直接回车即可），完成登录。
3. **键入命令：** 键入命令时建议将系统输入法切换为英文，也可以复制命令后使用右键即可粘贴命令，粘贴完毕后按回车即可执行命令。

#### <font color="###00BFFF">1. 软件中心重置</font>

- 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，直接在ssh客户端内运行下面的程序即可。

```bash
koolshare-reset
```

#### <font color="###00BFFF">2. 清空JFFS空间</font>
- 注意，此操作会删除jffs分区内的==所有文件==，包括但不限于：软件中心、SSL证书、自定义的设备图标等；
- 命令运行完毕后路由器会自动重启；
- 如果是在**官改固件**下清空JFFS空间，路由器重启后软件中心会重新初始化为最初状态；
```bash
kill -9 $(pidof skipd)
rm -r .[a-zA-Z_]* *
reboot
```

#### <font color="###00BFFF">3. 删除软件中心</font>
- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件。
- 如果是在**官改固件**下删除软件中心，路由器重启后软件中心会重新初始化为最初状态；
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db /jffs/ksdb /jffs/config/* /jffs/etc/profile
reboot
```

#### <font color="###00BFFF">4. 重启软件中心</font>
- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
sh /koolshare/perp/perp.sh
```

#### <font color="###00BFFF">5. RT_AX56U查询坏块命令</font>
- hnd/axhnd机型上查询坏块的方法已经不适用于axhnd.675x平台
- axhnd.675x平台查询坏块的命令如下（运行以下命令，返回数字即为坏块数量）：

```bash
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

#### <font color="#DC143C"> **386_42350**</font>

MD5: 0A5DC8344FBA0AB56A4EC2A69A1CEACD

SHA1: 2833FE210CA0BE7306886DFB88ECABA8787FD858

下载链接：[RT-AX55_386_42350](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX56U_V2/RT-AX56U_V2_386_42350_koolshare_cferom_puresqubi_0c76f7c.w)

#### <font color="#DC143C"> **384_9822**</font>

MD5: C4037DDE39ACEDF742AFC301BAABBFBE

SHA1: 1650001532F0695A62773C71C476FEC5C4789E47

下载链接：[RT-AX55_384_9822](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX56U_V2/RT-AX56U_V2_384_9822_koolshare_cferom_pureubi.w)

[/hide]
