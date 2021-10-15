---
title: "GT-AC5300 华硕官改固件"
linkTitle: "GT-AC5300"
type: docs
weight: 20
toc_hide: false
hide_summary: false
date: 2021-09-29
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_41793，更新日期：2021年02月06日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">〇、写在前面</font>

不知不觉，对华硕GT-AC5300官改固件的维护已经进入第四个年头了！

GT-AC5300是我制作的第一个华硕官改固件，当时我还在学生时代，记得当初制作的时候花了非常多的时间在各个细节上进行调整，比如对ROG风格的UI进行适配、对方向代理httpd能在华硕路由器上稳定工作进行的一系列测试、和小宝一起改进了skipdbv2，将其升级为skipdbv3...等等。

现在随着GT-AC5300固件的更新，固件大版本已经从382，经历384，更新到了386。而软件中心也从当初的1.0.0更新到了现在的1.8.1。

当然我自己也从学生时代毕业，到现在已经参加工作2年多了。现在也需要为了工作、家庭、生活等而奔波了，维护固件/软件中心作为自己的业余，时间肯定会少了一些，但是只要我有时间和精力，就会一直坚持更新下去的。

当然一如既往，我们的固件是免费提供的！

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>

1. 使用[GT-AC5300华硕官方固件源代码](https://www.asus.com.cn/Networking/ROG-Rapture-GT-AC5300/HelpDesk_Download/)为基础修改而来；
2. 官方固件有的功能，改版固件都有，如UU加速器、SpeedTest、AiMesh2.0等；
3. 开放GT-AC5300作为AiMesh节点时可以通过IP地址访问其web后台；
4. 固件后台界面优化：字体优化，网路地图页面显示状态页面；
5. 增加一些软件中心/插件需要用到的功能，如dnsmasq with ipset、base64、一些内核模块支持等；
6. koolshare软件中心支持：[hnd软件中心](https://github.com/koolshare/rogsoft#rogsoft)，软件中心和插件均支持GT-AC5300的ROG红色风格UI。

### <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕`GT-AC5300`机型，其它机型请勿使用本固件！


###  <font color="#f57332">四、更新日志</font>

#### <font color="###00BFFF">386_41793（2021年02月06日）</font>

> 从此版本开始，华硕GT-AC5300固件正式进入386大版本，在功能上，该版本主要更新了AiMesh 2.0和Ookla® SPEEDTEST（注意：GT-AC5300的SpeedTest功能在电竞加速选项卡里），当然也包含很多其它稳定性、安全性方面的更新。强烈建议大家进行升级！
> 
> 从384固件升级到386固件也是非常顺畅的，升级后不恢复出厂设置也是没问题的。当然稳妥起见，建议有时间的朋友还是做一次恢复出厂设置，然后在干净的配置上重新手动配置一次固件。

1. 同步ASUS最新GT-AC5300代码：3.0.0.4.386.41793。
2. 内置软件中心版本更新至1.6.7版本；

#### <font color="###00BFFF">384_82037（2020年12月17日）</font>
> 低于384_82037的官改固件刷入此版本，建议进行一次双清（即恢复出厂设置的时候同时勾选恢复按钮旁边的选择框），然后固件全部手动设置，插件全部重新安装。

1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.82037；
2. 更新内置koolshare软件中心到1.6.6版本；

#### <font color="###00BFFF">384_81974（2020年07月28日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.81974；
2. 更新内置koolshare软件中心到1.6.1版本；
3. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】。
4. curl回滚到ASUS版本：7.67.0
5. 现在GT-AC5300官改固件作为`AiMesh节点`时，其web后台也能正常访问了！

> **针对384\_9617第`5`点更新的说明如下，请仔细阅读：**
> - 华硕对AiMesh节点仅开放了固件更新这一个页面功能，这限制得太多了，但是这也是为了避免用户对节点进行设置造成mesh网络出问题；
> - kooldev将AiMesh节点的web后台访问全部开放了，但是需要提醒大家请尽量不要改动与AiMesh相关的设定，以免影响AiMesh网络的正常工作；
> - 我们开放AiMesh节点的web后台的访问，主要目的是为了大家能在AiMesh节点中使用软件中心，当然你也可以进行一些固件相关的设定，比如无线区域。
> - 需要注意的是因为AiMesh节点本质上是工作在中继模式，而非NAT模式，所以一些透明代理类的插件在AiMesh节点路由上是无法正常工作的，比如xxxx，kp等；
> - 如果你在AiMesh节点中修改了某些系统设置导致AiMesh网络失效，请在开机状态下长按机器后面的`reset`按钮重置你的AiMesh节点路由，然后用主路由重新添加节点；
> - AiMesh节点web后台的访问方式：在AiMesh主路由的【网络地图】页面点击【AiMesh节点】图标，然后在页面右侧会出现目前已经连接的AiMesh节点，点击对应节点机器后，会弹出节点信息，信息中会显示该节点机器的ip地址，比如我的是`192.168.2.78`，然后在浏览器中访问http://192.168.2.78即可访问AiMesh节点路由。

####  <font color="###00BFFF"> 384_81695（2020年04月27日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.81695；
	- 此版本固件是华硕再次时隔5个月放出的，其中涉及很多功能更新和安全更新，强烈建议升级；
2. 现在【Dashboard】页面中`网络ping`和`ping偏差`会默认显示www.baidu.com的ping状态；
3. 更新内置软件中心到最新1.5.5版本；
4. curl更新到7.69.1。

####  <font color="###00BFFF"> 384_81099（2019年11月30日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.81099；
	- 此版本固件是华硕时隔5个月放出的版本，其中涉及很多功能更新和安全更新，强烈建议升级；
	- 此版本固件支持UU加速器，但是不保证其和某不可描述插件的兼容性。
2. 回滚华硕对主界面侧边栏字体和图标的更改，回滚到45717版本的外观（因为华硕改得实在太丑了），不影响任何功能；
3. 更改【网络地图】为登录后默认页面，而不是【Dash board】页面；
4. 固件内置wireguard更新至0.0.20191127版本；
5. 更新内置软件中心到最新1.4.7版本；

####  <font color="###00BFFF"> 384_45717（2019年06月28日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.45717，此版本有几个重要的安全更新，强烈建议升级！
2. 同步内置软件中心为最新版本。

#### <font color="###00BFFF">384_45713（2019年05月07日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.45713。
2. 同步内置软件中心为最新版本。
3. 内置wireguard更新到最新版本（暂无插件支持）。

####  <font color="###00BFFF"> 384_45149（2018年12月24日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.45149，包含大量的安全性更新和稳定性修复，因此建议使用官改的朋友尽快升级到这个版本。
2. 因为华硕这次的更新为Alexa和IFTTT 更新了新功能，其中部分功能会与Server酱插件冲突导致无法上网，现在暂时没有找到更好的兼容方案前，移除了这次华硕为IFTTT 更新的客户端上线通知的功能。
3. 内核添加原生的wireguard支持，并且添加wg管理工具，现在用户可以自己在路由器内手动配置wireguard，配置方法参见wireguard官网。不会配置的可以等wireguard插件，目前已经完工60%，预计春节前放出。
4. 更新了内置的软件中心，并且添加了`koolshare-reset`命令，用户在ssh或者telnet客户端内输入`koolshare-reset`即可一键重置软件中心，效果等同下文中的：软件中心重置命令，用于软件中心出问题的、或者需要切换皮肤的用户。
5. 关闭了384.45149官方固件中新增的固件强制自动更新功能，因为这可能会导致官改用户被自动升级回官方固件。

#### <font color="###00BFFF">384_32799（2018年09月14日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.32799。
2. 修复一个官方固件自带的bug，该bug会导致ebtables和ipsec无法启动，现在可以正常启动了。
3. 现在网络地图页面右侧默认显示状态标签页（CPU，RAM，以太网接口），而不是现实某个wifi接口的状态。
4. 对网络地图页面右侧状态栏的错位进行了一些微调，现在显示更和谐一些。
5. 修复Dashboard中网络ping和ping偏差不显示曲线的问题，默认使用www.baidu.com作为ping数据获取的网址，如需更改，请自行更改nvram中的`ping_website`值。

#### <font color="###00BFFF">384_32738（2018年09月14日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.32738
2. 更新软件中心内置的skipd数据库到最新版本：修复lz4压缩问题，解决因储存一些值导致软件中心崩溃的问题
3. 同步内置软件中心为最新版本

#### <font color="###00BFFF">384_21140（2018年07月31日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.21140

#### <font color="###00BFFF">384_20648（2018年04月13日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.20648

#### <font color="###00BFFF">384_20308（2018年02月26日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.384.20308
2. 2018年2月27日 01:07:58，更新384_20308第二版，修复软件中心更新失败，插件下载失败21045。

#### <font color="###00BFFF">382_15984（2017年12月31日）</font>
1. 同步ASUS最新GT-AC5300代码：GPL of ASUS ROG Rapture GT-AC5300 for firmware 3.0.0.4.382.15984
2. 添加ipset支持
3. 添加dnsmasq ipset支持，dnsmasq conf-dir，dnsmasq postconf支持
4. 添加开机启动脚本支持：wan-start，nat-start，post-mount支持
5. curl添加socks5代理支持
6. busybox添加base64支持（不可描述订阅会用到），netstat -p支持等
7. 添加koolshare软件中心支持

### <font color="#f57332">五、刷机步骤</font>

- 约定`原厂固件`为华硕GT-AC5300官方固件：[GT-AC5300华硕官方固件下载地址](https://www.asus.com.cn/Networking/ROG-Rapture-GT-AC5300/HelpDesk_BIOS/)；
- 约定`官改固件`为koolshare开发组在[本贴](https://koolshare.cn/thread-130902-1-1.html)发布的基于[华硕官方GT-AC5300源代码](https://www.asus.com.cn/Networking/ROG-Rapture-GT-AC5300/HelpDesk_Download/)修改而来的带软件中心的官改固件，版本号为官方固件版本号后加上`_koolshare`后缀，如GT-AC5300官改固件版本：`3.0.0.4.386_41793_koolshare`。

> - 刷机建议使用chrome浏览器，或者chromium内核的浏览器进行刷机操作。
> - 刷机后如提示手动重启路由器，请等待几分钟后再手动开关电源进行重启。
> - 跨大版本刷机，如`384 → 386`或`386 → 384`，建议刷机完成后做一次固件双清操作；
> - 刷官改固件后如果软件中心页面一片空白，建议再手动重启一次路由器，如果仍然空白，参见FAQ：Q4。

#### <font color="###00BFFF">A. 原厂 → 官改：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好。

1. 在原产固件的固件升级页面下直接上传.w 后缀的RT-AX68U官改固件文件；
2. 刷机完成后会路由器会自动重启，此时刷机完成（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### <font color="###00BFFF">B. 官改 → 官改：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置。

1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.w 后缀的官改固件文件即可；
2. 刷机完成后会路由器会自动重启，此时刷机完成（如无特殊说明，刷机完成后不用恢复出产设置）；
3. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="###00BFFF">C. 官改 → 原厂</font>

> 从官改刷为原厂后建议做一次双清操作，以清除jffs分区里残留的一些软件中心相关文件。即使不进行双清操作，也不会影响刷回官方固件路由器的正常工作，你甚至可以立即再刷回官改固件，软件中心的所有插件和配置都将得到保留。

1. 在官改固件升级页面下直接上传.w 后缀的原厂固件文件；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如需彻底清空jffs里的文件残留，需要再执行一次双清操作：<font color="#DC143C">勾选恢复按钮旁的选择框，然后点击恢复按钮</font>；
4. 如果不想双清后重新设置路由器，可以参见后文【<font color="#f57332">重要命令</font>】中的【<font color="#DC143C">清空jffs空间</font>】或者【<font color="#DC143C">删除软件中心</font>】。

### <font color="#f57332">六、注意事项：</font>
1. 刷机后如果界面显示不正常，请使用组合键`ctrl + F5`强制清空浏览器缓存后重试；
2. 强烈建议使用chrome浏览器或者chromium内核的浏览器，以保持最佳兼容性；
3. 单纯的恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框；

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2021年01月06日

**Q1**：GT-AC5300为什么没有ML改版固件。

**A1**：见[ML固件原作者回答第一条](https://www.snbforums.com/threads/faq-read-me-first-before-posting-a-question.47153/)；因为没有ML固件，所以就没有ML改版固件。基于同样的原因，才有了koolshare官改固件。

**Q2：我离线安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。

1. 本贴的RT-AX68U属于axhnd.675x平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
2. 目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd软件中心](https://github.com/koolshare/rogsoft)，[qca软件中心](https://github.com/koolshare/qca)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！具体可以参考：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)；
3. 对于第三方作者开发的插件，除非作者明确表示其支持hnd/axhnd/axhnd.675平台，不然请不要随意安装！不然因为可能没有遵循开发规范，安装后无法使用，甚至给路由器带来问题！
4. 为了论坛和固件未来更好的发展，koolshare软件中心也会针对一些特殊的插件在离线安装上有所限制。

**Q3：软件中心一直显示更新中怎么办？**

**A3：** 此问题可能由多种原因导致，请尝试下面的方法：

1. 访问https://rogsoft.ddnsto.com/，请确保你访问此网站的时候使用的是连接到该路由器下的客户端，如果显示`Hello to everyone`字样，表示你的路由下的本地网络访问软件中心服务器没有问题；如果不显示上述字样，则可能是是网络方面的问题。
2. 情况1，路由器本地网络故障：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`ping rogsoft.ddnsto.com`，看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定后再试；如果能解析ip地址当时无法ping通，可能是本地网络问题或者软件中心服务器正在维护。
3. 情况2，路由器本地网络故障：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`curl -sS4L https://rogsoft.ddnsto.com/|grep Hello`，如果显示了两行内容都包含`Hello to everyone`字样，表明路由器访问软件中心web服务器没有问题；如果没有以上显示，可能是本地网络问题或者软件中心服务器正在维护。
4. 情况3，服务器网络故障：这有可能是koolshare软件中心服务器维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
5. 如果排除了以上网络故障，那么可能是程序运行方面的问题。可以进行以下操作：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep -w httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考下文：重要命令里的==重启软件中心==以解决httpdb没有运行的问题。
6. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考下文：重要命令里的软件中心重置。
7. 还有一种较为常见的情况，在刷机过程中，jffs分区中存放的软件中心相关文件在刷机过程/路由器断电/重启过程中被破坏了，如果被破坏的文件正好是httpdb、软件中心数据库等关键文件，也会导致软件中心一直显示更新中的情况。虽然部分情况下，替换损坏的文件可以修复此问题，但是由于无法知晓是否有其它的文件损坏，所以这种情况下建议对路由器进行双清操作，双清完成后，路由器jffs分区内的软件中心相关文件会得到重建，然后在此基础上手动安装插件并手动配置，切记不要使用以前的jffs分区备份来进行恢复！
8. 最后，最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==GT-AC5300查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：刷机后软件中心一片空白**

**A4：** 按照下面的顺序依次尝试：

1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`，最后的数字9会根据机型/平台的不同而不同。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载TUF-AX3000的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心，然后应该就能看到软件中心页面了。

**Q5：华硕发了GT-AC5300固件，为什么此帖还不更新官改固件啊？**

**A5：** 官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的xxx版本固件无线有问题，能否修复？**

**A6**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：可不可给固件以增加xxx功能？**

**A7**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

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

- 注意，此操作会删除jffs分区内的所有文件，包括但不限于：软件中心、安装的证书、TrafficAnalyzer的数据库、自定义的设备图标等
```bash
kill -9 $(pidof skipd)
cd /jffs && rm -r .[a-zA-Z_]* *
reboot
```

#### <font color="###00BFFF">3. 删除软件中心</font>

- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件；
- 如果是在**官改固件**下删除软件中心，路由器重启后软件中心会重新初始化为最初状态。
```bash
kill -9 $(pidof skipd)
cd /jffs && rm -rf .asusrouter .koolshare db ksdb config/* etc/profile
reboot
```

#### <font color="###00BFFF">4. 重启软件中心</font>

- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
sh /koolshare/perp/perp.sh
```

#### <font color="###00BFFF">5. GT-AC5300查询坏块命令</font>
- 先重启一次路由器，再输入以下命令进行查询，返回信息的行数即为坏块的数量
```bash
dmesg |grep "bad block"
```

### <font color="#f57332">九、固件下载</font>

#### <font color="#DC143C"> **386_41793**</font>

MD5: 647C4A65457E069F312E69FE43449F89

SHA1: 400CD4764CD372B06DB15FA08E893C711C3CF006

下载链接：[GT-AC5300_386_41793_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_386_41793_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_82037**</font>

MD5: 73A43DD8B933E61C5B74E2A58E01ADB0

SHA1: 9A4A923BA214784ED3EF4F09C5C47458BB80B34F

下载链接：[GT-AC5300_384_82037_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_82037_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_81974**</font>

MD5: 6F6F36C8D794CA89E368688D3659239B

SHA1: 01EF97B7E92B86996F9D736DF6FD2F1CBFEAB436

下载链接：[GT-AC5300_384_81974_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_81974_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_81695**</font>

MD5: F9F54B1A67E8A9BFB3630D962B33DF2F

SHA1: 909873057484B692559443805F84E60914C4C06C

下载链接：[GT-AC5300_384_81695_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_81695_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_81099**</font>

MD5: C6D85EE3B7A522AF1CB994977B4C5C0E

SHA1: DEB534DD2FE097B3F4EBD9E601D11EC97B34722E

下载链接：[GT-AC5300_384_81099_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_81099_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_45717**</font>

MD5: AA66291AC8A8840A8276F82819224465

SHA1: 3190350A0A8A648C0FD33F7AFFC5CB19A543B62F

下载链接：[GT-AC5300_384_45717_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_45717_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_45713**</font>

MD5: C1EBEAB8E960881A04B5B7B6699D3575

SHA1: 153A4F6DCCA5A8D7E5413EF411DBAEB223086056

下载链接：[GT-AC5300_384_45713_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_45713_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_45149**</font>

MD5: FB8E3D5109D36652017821D6C2048CA5

SHA1: 92446D7A953CA1BD95611C1A1B0A9EFDB54958B1

下载链接：[GT-AC5300_384_45149_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_45149_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_32799**</font>

MD5: FB8E3D5109D36652017821D6C2048CA5

SHA1: 92446D7A953CA1BD95611C1A1B0A9EFDB54958B1

下载链接：[GT-AC5300_384_32799_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_32799_koolshare_cferom_ubi.w)


#### <font color="#DC143C"> **384_32738**</font>

MD5: 748E590FD4FBCA5177C3997561E907FA

SHA1: 39617F822EE70DBE1113766184ED65786714692C

下载链接：[GT-AC5300_384_32738_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_32738_koolshare_cferom_ubi.w)


#### <font color="#DC143C"> **384_21140**</font>

MD5: 955B454BBC97A118EAC5D2995CDE8C50

SHA1: 2CD0F1F181983591710F71B0334ED24BEBE727F8

下载链接：[GT-AC5300_384_21140_koolshare_cferom_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_21140_koolshare_cferom_ubi.w)


#### <font color="#DC143C"> **384_20648**</font>

MD5: 2525239107DC9E430DF7D23709ACB6D8

SHA1: 581C729FEC30D1297D87BC0C490BCE522BF43424

下载链接：[GT-AC5300_384_20648_koolshare_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_20648_koolshare_ubi.w)


#### <font color="#DC143C"> **384_20308**</font>

MD5: 71A8ADF68C4EAB71EF3F31A73462A847

SHA1: C0C787C6FADD205D436EEA7BA62DF88FCA6E5AFB

下载链接：[GT-AC5300_384_20308_koolshare_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_384_20308_koolshare_ubi.w)

#### <font color="#DC143C"> **382_15984**</font>

MD5: 6BB7BEE9C09BC75EE6925CA539E3C10C

SHA1: 804EE5AD4C95E43377C3ADEA5D5ED7FF56F3BF3B

下载链接：[GT-AC5300_382_15984_koolshare_ubi.w](http://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/GT-AC5300/GT-AC5300_382_15984_koolshare_ubi.w)
