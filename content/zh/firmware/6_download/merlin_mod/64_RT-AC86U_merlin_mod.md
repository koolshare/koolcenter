---
title: "RT-AC86U 梅林改版固件"
linkTitle: "RT-AC86U"
type: docs
weight: 65
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["梅林改版固件"]
categories: ["固件下载"]
description: >
  最新版本：386.3_2，更新日期：2021年08月07日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

* 注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

* 注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>
1. 梅林改版固件使用梅林固件源代码为基础（[asuswrt-merlin.ng代码](https://github.com/RMerl/asuswrt-merlin.ng)）修改而来；
2. 梅林固件有的功能，梅林改版固件都有，参考此链接：[梅林固件添加的功能](https://github.com/RMerl/asuswrt-merlin.ng/blob/master/README-merlin.txt#L62-L132)；
3. 梅林固件不能使用的功能，梅林改版也不能使用，比如说UU加速器等；
4. 开放RT-AC86U作为AiMesh节点时可以通过IP地址访问其web后台；
5. 固件后台界面优化：字体优化，首页默认显示状态页面；
6. 增加一些软件中心/插件需要用到的功能，如dnsmasq with ipset、base64、一些内核模块支持等；
7. koolshare软件中心支持：[hnd软件中心](https://github.com/koolshare/rogsoft#rogsoft)；

### <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕`RT-AC86U`机型，其它机型请勿使用本固件！

###  <font color="#f57332">四、更新日志</font>

####  <font color="#00BFFF">386.3_2（2021年08月07日）</font>
1. 同步梅林固件代码386.3_2，更新日志见此：[Asuswrt-Merlin 386/NG Changelog](https://www.asuswrt-merlin.net/changelog)；
2. 同步软件中心1.7.5

####  <font color="#00BFFF">386.3_0（2021年07月30日）</font>
1. 同步梅林固件代码386.3_0
2. 同步软件中心1.7.3

####  <font color="#00BFFF">386.2_6（2021年06月17日）</font>
1. 同步梅林固件代码386.2_6

####  <font color="#00BFFF">386.2_4（2021年05月19日）</font>
1. 同步梅林固件代码386.2_4

####  <font color="#00BFFF">386.2_2（2021年04月14日）</font>
1. 同步梅林固件代码386.2_2
2. 同步软件中心1.7.1

####  <font color="#00BFFF">386.2_0（2021年04月07日）</font>
1. 同步梅林固件代码386.2_0
2. 同步软件中心1.7.0

####  <font color="#00BFFF">386.1_2（2021年02月13日）</font>
1. 同步梅林固件代码386.1_2

####  <font color="#00BFFF">386.1_0（2021年01月31日）</font>
>从此版本开始，华硕RT-AC86U梅林改版固件正式进入386大版本，在功能上，该版本主要更新了AiMesh 2.0和Ookla® SPEEDTEST，当然也包含很多其它稳定性、安全性方面的更新。强烈建议大家进行升级！
> 
>从384固件升级到386固件也是非常顺畅的，升级后不恢复出厂设置也是没问题的。当然稳妥起见，建议有时间的朋友还是做一次恢复出厂设置，然后在干净的配置上重新手动配置一次固件。

1. 同步asuswrt-merlin.ng代码386.1_0；
2. 同步软件中心版本1.6.7；
3. 移除了在384改版梅林固件中添加的wireguard功能。

####  <font color="#00BFFF">384.19_0（2020年08月21日）</font>
> <font color="red">**重要事项：**</font>因此版本RT-AC86U的jffs分区结构的改变，刷384.19_0版本之前，请前往【系统管理】- 【恢复/导出/上传设置】页面的【Backup JFFS partition】选项，点击保存按钮，保存整个jffs分区的文件，待固件升级完成后再用备份的jffs分区文件进行恢复。恢复后需要重启一次路由器才能完全恢复正常！
> 如果你没有进行以上操作而进行了刷机，那么只有重新格式化jffs分区重置软件中心才能正常使用！

1. 同步asuswrt-merlin.ng代码384.19_0；
2. 现在当RT-AC86U梅林改版固件作为`AiMesh节点`时，其web后台也能正常访问了！

####  <font color="#00BFFF">384.18_0（2020年07月02日）</font>
1. 同步asuswrt-merlin.ng代码384.18_0
2. 内置软件中心更新到1.6.1

####  <font color="#00BFFF">384.17_0（2020年04月27日）</font>
1. 同步asuswrt-merlin.ng代码384.17_0
2. 如果出现无法刷入的问题，请尝试关闭所有插件、重启路由器后尝试。

####  <font color="#00BFFF">384.16_0（2020年04月16日）</font>
1. 同步asuswrt-merlin.ng代码384.16_0

####  <font color="#00BFFF">384.15_0（2020年03月20日）</font>
1. 同步asuswrt-merlin.ng代码384.15_0
2. 内置软件中心更新到1.5.1

####  <font color="#00BFFF">384.14_0（2019年12月19日）</font>
1. 同步asuswrt-merlin.ng代码384.14_0
2. 固件内置wireguard更新至0.0.20191219版本；

####  <font color="#00BFFF">384.13_1（2019年08月21日）</font>
1. 同步asuswrt-merlin.ng代码384.13_0
2. 注意：此版本梅林固件已经原生支持AiMesh，因此不再需要本改版固件进行解锁支持。另外此AiMesh并不支持在线更新AiMesh节点路由器的固件，需要手动更新。
2. 更新jffsinit.sh，现在全新刷机后会显示内置的软件中心版本号，而不是显示版本为`0.0`
3. 更新内置软件中心到最新

####  <font color="#00BFFF">384.12_0（2019年06月26日）</font>
1. 同步asuswrt-merlin.ng代码384.12_0
2. 为了保持和一些插件的兼容性，将【Wan: Use local caching DNS server as system resolver (default: No)】选项默认更改为"是"。

####  <font color="#00BFFF">384.11_2（2019年05月19日）</font>
1. 同步asuswrt-merlin.ng代码384.11_2

####  <font color="#00BFFF">384.11_0（2019年05月12日）</font>
1. 同步asuswrt-merlin.ng代码384.11_0
2. 同步内置软件中心为最新版本，更新httpdb，修复软件中心崩溃的问题；
3. 内置wireguard更新到最新版本（暂无插件支持）。

####  <font color="#00BFFF">384.10_2（2019年04月05日）</font>
1. 同步asuswrt-merlin.ng代码384.10_2
2. 修复了梅林固件和serverchan插件的冲突；
3. 在固件层面上开放了梅林固件的aimesh功能；

####  <font color="#00BFFF">384.10_0（2019年03月31日）</font>
1. 同步asuswrt-merlin.ng代码384.10_0
2. 添加了`koolshare-reset`命令，用户在ssh或者telnet客户端内输入`koolshare-reset`即可一键重置软件中心，效果等同下文中的：软件中心重置命令，用于软件中心出问题或者需要切换皮肤的用户。
3. 同步[wireguard代码](https://git.zx2c4.com/WireGuard/)为最新（截止2019年3月31日）；

####  <font color="#00BFFF">384.9_0（2019年02月03日）</font>
1. 同步asuswrt-merlin.ng代码384.9
2. 移除原版梅林394.9_0的哥特字体风格，因为显示效果对中文太不友好了！
3. 同步[wireguard代码](https://git.zx2c4.com/WireGuard/)为最新，因为wireguard是内核组建，所以现在都是跟随固件更新；
4. 之前说到的wireguard插件春节前推出，要鸽子一段时间，一是最近比较忙，而是其在博通armv8平台上的运行还有些许问题。

####  <font color="#00BFFF">384.8_2（2018年12月11日）</font>
1. 同步asuswrt-merlin.ng代码384.8_2
2. 网络地图默认显示状态而非5G

#### <font color="#00BFFF">384.8_0（2018年12月03日）</font>
1. 同步asuswrt-merlin.ng代码384.8_0
2. 内核添加wireguard支持，并新增对应管理工具：wg；
3. 同步内置软件中心为最新版本；

#### <font color="#00BFFF">384.7_0（2018年10月10日）</font>
1. 同步asuswrt-merlin.ng代码384.7_0
2. 更新软件中心内置的skipd数据库到最新版本：修复lz4压缩问题，解决因储存一些值导致软件中心崩溃的问题；
3. 同步内置软件中心为最新版本；
4. 注意384.7 merlin固件对ddns和dnsfilter做了较大改动，详情请查看merlin.ng更新日志；

#### <font color="#00BFFF">384.6_0（2018年07月29日）</font>
1. 同步asuswrt-merlin.ng代码384.6_0

#### <font color="#00BFFF">384.5_0（2018年05月14日）</font>
1. 同步asuswrt-merlin.ng代码384.5_0
2. 为避免不必要的问题，此次及以后均提供带cferom的固件版本

#### <font color="#00BFFF">384.4_0（2018年03月17日）</font>
1. 同步asuswrt-merlin.ng代码384.6_0

#### <font color="#00BFFF">382.1_2（2017年12月05日）</font>
1. 同步asuswrt-merlin.ng代码382.1_2

#### <font color="#00BFFF">382.1_1（2017年11月29日）</font>
1. 同步asuswrt-merlin.ng代码382.1_1

#### <font color="#00BFFF">382.1_0（2017年11月13日）</font>
1. 同步asuswrt-merlin.ng代码382.1_0
2. 添加koolshare软件中心支持

### <font color="#f57332">五、刷机步骤</font>

#### <font color="#00BFFF">刷机准备</font>

- 建议下载好固件后，对固件的md5/sha1校验码进行核对，以保证固件完整性；
- 建议刷机全程使用电脑端谷歌Chrome，或者Chromium内核的浏览器进行操作；
- 如果使用了USB2JFFS插件，建议先使用卸载掉USB的挂载后在进行刷机，刷机后再进行挂载。

#### <font color="#00BFFF">固件定义</font>

- `原厂固件`为RT-AC86U华硕官方固件：[RT-AC86U华硕官方固件下载地址](https://www.asus.com.cn/Networking/RT-AC86U/HelpDesk_BIOS/)；
- `官改固件`为koolshare开发组在[此帖](https://koolshare.cn/thread-139965-1-1.html)发布的基于[华硕官方RT-AC86U源代码](https://www.asus.com.cn/Networking/RT-AC86U/HelpDesk_Download/)修改而来的带软件中心的RT-AC86U官改固件，版本号为官方固件版本号后加上`_koolshare`后缀，如RT-AC86U官改固件版本：`3.0.0.4.386_40451_koolshare`。
- `原版梅林固件`为加拿大独立开发者Eric Sauvageau在华硕RT-AC86U官方源码上二次开发的第三方固件，相较华硕官方固件，其区别为：[这些功能](https://github.com/RMerl/asuswrt-merlin.ng/blob/master/README-merlin.txt#L62-L132)，其版本号为`384.x`/`386.x`，如：`384.19`/`386.1`；
- `改版梅林固件`为koolshare开发组在[本贴](https://koolshare.cn/thread-127878-1-1.html)发布的基于梅林固件源码再次开发而来的带软件中心的RT-AC86U梅林改版固件，其版本号和梅林原版固件保持一致，如RT-AC86U官改固件版本：`384.19`/`386.1`。

#### <font color="#00BFFF">刷机术语</font>

> 为消除小白在刷机过程中的疑惑，下面列出一下华硕/梅林固件刷机的基本术语及我自己的解释，希望对大家有所帮助。如果你对下面的内容已经比较清楚，那么可以跳过这部分直接进入到刷机流程。

1. **固件双清**：双清就是要清除：1. nvram配置，2：JFFS分区文件。固件的很多设置都是储存在nvram中，例如拨号方式、拨号上网帐号密码、无线网络设置等；固件的很多文件是储存在JFFS分区的，例如流量分析储存的流量数据，SSL证书，UU加速器程序等。一般同类型固件互刷不需要进行双清，不同类型固件互刷视情况要进行双清，以保证路由器刷机后处于最佳工作状态。<font color="#FF00CC">如何双清路由器：</font>进入【系统管理 】–【 恢复/导出/上传设置】，勾选恢复按钮旁的选择框，然后点击恢复按钮。
2. **恢复出厂**：恢复出厂就是清除固件的nvram配置，但是不清除JFFS分区文件。这样流量分析、SSL证书等文件并不会丢失。值得注意的是很多朋友有用【导出设置】来备份固件配置的习惯，而在刷固件，特别是不同类型固件互刷的情况下，是不适用使用备份的配置来恢复刚刚进行了恢复出厂的机器的，因为这样就相当于你什么也没恢复。所以请一定不要使用以前备份的配置来恢复刚刷机后，又进行过恢复出厂的路由器。使用【导出设置】备份的配置文件，一般进行了一些设置导致路由器出了问题，将路由器恢复到原厂默认值后，再用备份配置进行恢复，使用备份配置前后，路由器都是同一个版本。<font color="#FF00CC">如何恢复出厂：</font>进入【系统管理 】–【 恢复/导出/上传设置】，点击恢复按钮，记住不要勾选恢复按钮右侧的选择框！！
3. **格式化JFFS**：格式化JFFS就是对JFFS分区进行格式化，这样会删除JFFS分区中储存的所有文件，而不影响路由器的其它配置。在梅林改版固件中，因为软件中心就是储存在JFFS分区中的，所以格式化JFFS可以快速的清除当前JFFS分区中的软件中心文件，从而实现软件中心的重置。当然，格式化JFFS，也会删除固件在JFFS分区中存放的一些文件，如SSL证书、流量分析数据等。如果你只想重置软件中心，而不伤害其它JFFS分区中的文件，你可以参考下文【重要命令】中的【软件中心重置】或【删除软件中心】。<font color="#FF00CC">如何格式化JFFS：</font>在梅林/梅林改版固件中，在【系统管理】–【 系统设置】内勾选`Format JFFS partition at next boot`（中文意思就是：下次重启的时候格式化JFFS分区），然后点击`应用本页面设置`，成功后点击顶部`重启`按钮重启路由器。路由器重启过程中就会对JFFS分区进行格式化，重启完成后，`Format JFFS partition at next boot`将自动变为否，以免下次路由器重启的时候，JFFS分区再次被格式化。
4. **JFFS挂载状态**：通过SSH连接到路由器后台后输入命令（如果不知道如何使用SSH执行命令，可以参考下文【重要命令】中的【如何使用SSH】）：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。当然，在梅林/梅林改版固件中，只需要进入【Tools - Sysinfo】页面，在JFFS一栏即可看到JFFS挂载状态，如果成功挂载，将会显示JFFS已用容量和总容量，如果没有挂在，则会显示*umounted*字样。因为软件中心是储存在JFFS中的，所以如果软件中心进入后是空白页面，一般来说JFFS分区的挂载就出现了问题。遇到这种情况，可以参考下文FAQ中的【Q3：刷机后软件中心一片空白】来尝试解决。
5. **JFFS分区备份/还原**：使用梅林/梅林改版固件的朋友，可能知道梅林固件相对于华硕官方固件，多了JFFS分区备份/还原功能，其本质就是将JFFS分区内的所有文件进行打包，然后在需要的时候进行还原。此功能在某些时候会特别管用，比如某个版本固件升级后，JFFS分区容量被缩小了，这会导致储存在JFFS分区靠后的文件块被强行清除，从而导致JFFS分区内文件丢失、文件损坏。而使用JFFS分区备份/还原功能，在每次固件升级前先备份一次JFFS分区内容，在固件升级后，如果JFFS分区内容出现丢失、损坏等，再用备份进行还原即可规避上面的问题。当然如果是梅林改版固件的话，只进行还原还是不够的，因为刚还原后，软件中心相关程序虽然还原了，但是其进程还没有启动，此时重启一次路由器，才能让软件中心在还原后正常工作。

#### <font color="#00BFFF">开始刷机</font>
因为救援模式的存在，所以华硕路由器刷机是刷不死的，只要刷机过程中有灯亮，那么出现任何无法启动的问题都是能救得活的。所以不论你当前处在什么类型固件、什么固件版本下，都可以尝试一步刷到位：直接刷机到最新的`386改版梅林`固件！如果能正常通过刷机，成功后进行一次固件双清，达到干净刷机的效果。如果不能通过刷机，救援模式也是分分钟能搞定的事情！所以请不要被下面写得非常详细的刷机流程吓到。

当然，也可以将刷机做到很细致，那么根据你现在的固件，用下面A - E的操作来对号入座把！虽然细致刷机过程也可能发生意外，但是请记住三大法宝：重启、重置、救援模式。

#### <font color="#00BFFF">A. 原厂固件 → 改版梅林固件：</font>

> 原厂固件和原版梅林固件/改版梅林固件在一些默认配置上有所不同，虽然刷机后不用恢复出厂设置也能正常工作，但是建议有时间朋友刷机完成后双清一次路由双清后全部手动配置，不要用以前的备份配置。

1. 在`原厂固件`固件升级页面下直接上传.w 后缀的`改版梅林固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成（刷机完成后可以不恢复出产设置，当然恢复一次更好）；
3. 刷机完成在【系统管理 】–【 系统设置】内勾选：`Format JFFS partition at next boot` 和 `Enable JFFS custom scripts and configs` 然后点击`应用本页面设置`，成功后点击顶部`重启`按钮重启路由器；
4. 重启后进入web后台时先设置路由器，将路由器连上网络，然后进入软件中心，如果软件中心一片空白，不要着急，先软重启（使用顶部重启按钮）一次路由器即可出现软件中心，如果软件中心仍然空白，参见FAQ：Q4的解决办法。
5. 如果进入软件中心后正常，将软件中心更新到最新版本（如果有）后即完成全部刷机，之后你可以对路由器固件进行其它喜好的设置，或者在软件中心安装插件等操作。

#### <font color="#00BFFF">B. 原版梅林固件 → 改版梅林固件：</font>

1. 在`原版梅林固件`固件升级页面下直接上传.w 后缀的`改版梅林固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成（刷机完成后可以不恢复出产设置，当然恢复一次更好）；
3. 刷机完成在【系统管理 】–【 系统设置】内勾选：`Format JFFS partition at next boot` 和 `Enable JFFS custom scripts and configs` 然后点击`应用本页面设置`，成功后点击顶部`重启`按钮重启路由器；
4. 重启后进入web后台时先设置路由器，将路由器连上网络，然后进入软件中心，如果软件中心一片空白，不要着急，先软重启（使用顶部重启按钮）一次路由器即可出现软件中心，如果软件中心仍然空白，参见FAQ：Q4的解决办法。
5. 如果进入软件中心后正常，将软件中心更新到最新版本（如果有）后即完成全部刷机，之后你可以对路由器固件进行其它喜好的设置，或者在软件中心安装插件等操作。


#### <font color="#00BFFF">C. 官改固件 → 改版梅林固件：</font>

> 官改固件和原版梅林固件/改版梅林固件在一些默认配置上有所不同，虽然刷机后不用恢复出厂设置也能正常工作，但是建议有时间朋友刷机完成后双清一次路由双清后全部手动配置，不要用以前的备份配置。

**1. 刷机后刷双清**
1. 在`官改固件`固件升级页面下直接上传.w 后缀的`改版梅林固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成；
3. 刷机完成后对路由器进行一次`双清`，并全部手动配置路由器；
4. 双清完成后进入路由器web后台，在【系统管理 】–【 系统设置】内勾选：`Format JFFS partition at next boot` 和 `Enable JFFS custom scripts and configs` 然后点击`应用本页面设置`，成功后点击顶部`重启`按钮重启路由器；
5. 重启后进入web后台时先设置路由器，将路由器连上网络，然后进入软件中心，如果软件中心一片空白，不要着急，先软重启（使用顶部重启按钮）一次路由器即可出现软件中心，如果软件中心仍然空白，参见FAQ：Q4的解决办法。
6. 如果进入软件中心后正常，将软件中心更新到最新版本（如果有）后即完成全部刷机，之后你可以对路由器固件进行其它喜好的设置，或者在软件中心安装插件等操作。

**2. 刷机后刷不双清**
1. 在`官改固件`固件升级页面下直接上传.w 后缀的`改版梅林固件`文件；
2. 刷机完成后会自动重启，此时刷机完成；
3. 刷机后如果【系统管理 】–【 系统设置】内的`Enable JFFS custom scripts and configs`选项为否，需要将其勾选为是，然后点击`应用本页面设置`即可；
4. 以上步骤完成后，固件中的软件中心和所有插件都会得到保留。如果是`384官改固件`刷`386改版梅林固件`，某些需要离线安装的插件需要覆盖安装一次（最好覆盖安装最新版本），该插件才能正常工作！

#### <font color="#00BFFF">D. 改版梅林固件 → 改版梅林固件</font>

1. 在`改版梅林固件`升级页面下直接上传.w 后缀的`改版梅林固件`文件，刷机完成后机器会自动重启；
2. 请阅读你刷的固件版本的更新日志，看是否有附加刷机说明（如恢复出厂，双清，格式化JFFS等），如果没有任何要求，刷机完成后可以不恢复出厂设置；
3. 刷机完成后，固件中的软件中心和所有插件都会得到保留；
4. 以上步骤完成后，固件中的软件中心和所有插件都会得到保留；
5. 如果刷机后软件中心页面一片空白，建议再手动软重启（使用顶部重启按钮）一次路由器，如果仍然空白，参见FAQ：Q4。

#### <font color="#00BFFF">E. 改版梅林固件 → 官改固件</font>

> 原版梅林固件/改版梅林固件与官改固件在一些默认配置上有所不同，虽然刷机后不用恢复出厂设置也能正常工作，但是建议有时间朋友刷机完成后双清一次路由，双清后全部手动配置，不要用以前的备份配置。

**1. 刷机后刷双清**

1. 在`改版梅林固件`固件升级页面下直接上传.w 后缀的`官改固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成；
3. 刷机完成后对路由器进行一次`双清`，并全部手动配置路由器；
4. 双清完成后进入路由器web后台，将路由器连上网络，然后进入软件中心，如果软件中心一片空白，不要着急，先软重启（使用顶部重启按钮）一次路由器即可出现软件中心，如果软件中心仍然空白，参见FAQ：Q4的解决办法。
5. 如果进入软件中心后正常，将软件中心更新到最新版本（如果有）后即完成全部刷机，之后你可以对路由器固件进行其它喜好的设置，或者在软件中心安装插件等操作。

**2. 刷机后刷不双清**

1. 在`改版梅林固件`固件升级页面下直接上传.w 后缀的`官改固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成；
3. 刷机完成后，固件中的软件中心和所有插件都会得到保留，如果是`386改版梅林固件`刷`384官改固件`，某些需要离线安装的插件需要覆盖安装一次（最好覆盖安装最新版本），该插件才能正常工作！

#### <font color="#00BFFF">F. 改版梅林固件 → 原厂固件/原版梅林固件</font>

> 从改版梅林固件刷为原厂固件/原版梅林固件后建议做一次双清操作，以清除jffs分区里残留的一些软件中心相关文件。不过即使不进行双清操作，也不会影响刷回原厂固件路由器的正常工作，你甚至可以立即再刷回改版梅林固件，软件中心的所有插件和配置都将得到保留，并且正常工作。

1. 在`改版梅林固件`升级页面下直接上传.w 后缀的`原厂固件`/`原版梅林固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成；
3. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
4. 如需彻底清空jffs里的文件残留，需要再执行一次双清操作；
5. 如果不想双清后重新设置路由器，可以参见后文【<font color="#f57332">重要命令</font>】中的【<font color="#DC143C">清空jffs空间</font>】或者【<font color="#DC143C">删除软件中心</font>】。

### <font color="#f57332">六、注意事项：</font>
1. 刷机后如果界面显示不正常，请使用组合键`ctrl + F5`强制清空浏览器缓存后重试；
2. 强烈建议使用chrome浏览器或者chromium内核的浏览器，以保持最佳兼容性；
3. 请勿使用不同版本固件备份的路由器设置来恢复当前路由器。

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2019年12月1日

**Q1：RT-AC86U改版梅林和官改固件比较有什么区别，哪个好用，哪个更稳定？**

**A1：** 改版梅林固件基于梅林固件修改，官改固件基于官方固件修改。两者都是在基础固件代码上以添加软件中心为目的。相比官改固件，梅林改版固件有更多的功能和bug修复，而官改固件更新较快。好用程度差别不大，稳定性来说也基本无差，选哪个固件基于个人喜好即可。

**Q2：我离线安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。

1. 本贴的RT-AX86U属于axhnd.675x平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
2. 目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd软件中心](https://github.com/koolshare/rogsoft)，[qca软件中心](https://github.com/koolshare/qca)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！具体可以参考：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)；
3. 对于第三方作者开发的插件，除非作者明确表示其支持hnd/axhnd/axhnd.675平台，不然请不要随意安装！不然因为可能没有遵循开发规范，安装后无法使用，甚至给路由器带来问题！
4. 为了论坛和固件未来更好的发展，koolshare软件中心也会针对一些特殊的插件在离线安装上有所限制。

**Q3：软件中心一直显示更新中怎么办/不显示版本号怎么办？**

**A3：** 此问题可能由多种原因导致，请尝试下面的方法：

1. 访问https://rogsoft.ddnsto.com/，请确保你访问此网站的时候使用的是连接到该路由器下的客户端，如果显示`Hello to everyone`字样，表示你的路由下的本地网络访问软件中心服务器没有问题；如果不显示上述字样，则可能是是网络方面的问题。
2. 情况1，路由器本地网络故障：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`ping rogsoft.ddnsto.com`，看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定后再试；如果能解析ip地址当时无法ping通，可能是本地网络问题或者软件中心服务器正在维护。
3. 情况2，路由器本地网络故障：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`curl -sS4L https://rogsoft.ddnsto.com/|grep Hello`，如果显示了两行内容都包含`Hello to everyone`字样，表明路由器访问软件中心web服务器没有问题；如果没有以上显示，可能是本地网络问题或者软件中心服务器正在维护。
4. 情况3，服务器网络故障：这有可能是koolshare软件中心服务器维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
5. 如果排除了以上网络故障，那么可能是程序运行方面的问题。可以进行以下操作：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep -w httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考下文：重要命令里的==重启软件中心==以解决httpdb没有运行的问题。
6. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考下文：重要命令里的软件中心重置。
7. 还有一种较为常见的情况，在刷机过程中，jffs分区中存放的软件中心相关文件在刷机过程/路由器断电/重启过程中被破坏了，如果被破坏的文件正好是httpdb、软件中心数据库等关键文件，也会导致软件中心一直显示更新中的情况。虽然部分情况下，替换损坏的文件可以修复此问题，但是由于无法知晓是否有其它的文件损坏，所以这种情况下建议对路由器进行双清操作，双清完成后，路由器jffs分区内的软件中心相关文件会得到重建，然后在此基础上手动安装插件并手动配置，切记不要使用以前的jffs分区备份来进行恢复！
8. 最后，最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==RT-AX86U查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：刷机后软件中心一片空白**

**A4：** 按照下面的顺序依次尝试：

1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`，最后的数字9会根据机型/平台的不同而不同。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载TUF-AX3000的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心，然后应该就能看到软件中心页面了。

**Q5：Rmerl发布了最新的RT-AC86U梅林固件，为什么此贴还不更新梅林改版固件啊？**

**A6：** 新梅林改版固件的发布涉及大到大量的源代码合并工作，期间还涉及到一些编译、测试、回炉等工作，不过一般来说梅林原版固件更新后1天-1周内，就会完成编译和测试工作。

**Q6：我的xxx固件无线有问题，能否修复？**

**A6：** 无线问题无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：RT-AC86U现在还需要挂载虚拟内存吗？**

**A7：** 随着华硕对固件的不断更新，现在已经越来越完善和稳定，大多数时候都可以摆脱虚拟内存了。不过这里还是建议大家都使用虚拟内存，因为虽然86U使用了512M的内存，但是实际上只有430M可用内存，有82M被博通硬件占用了。加上固件使用了glibc库，对于嵌入式设备来说还是太重了，glibc的软件体积较大，内存占用较多，最终导致实际在界面上看到剩余200多M的剩余内存。挂载虚拟内存后大多数情况下都看不到虚拟内存的使用，但是系统的稳定性会大大增强，特别是对一些golang语言写的程序的运行会有很大改善。虚拟内存的制作与开启，建议使用86U软件中心提供的`虚拟内存插件`，U盘插2.0和3.0接口均可，建议512MB虚拟内存即可。

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方（Asuswrt）和梅林（Asuswrt-RMerl）的一些功能更新，也会包含ASUS官方和梅林的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本梅林改版固件进行更新的，所以是强烈建议升级到最新版本koolshare梅林改版固件的。另外已经刷过koolshare梅林改版固件的，升级到最新koolshare梅林改版固件，如果没有特殊说明，是不需要做恢复出厂设置等操作的，所有的插件和设置都会得到保留。

**Q9：华硕GT-AC2900路由器硬件和RT-AC86U几乎一样，固件通刷吗？**

**A9**：不通刷！不通刷！不通刷！虽然在硬件上一样，但是不同机器有不同的cfe设定，固件是能对不同机型进行识别的，即使你给RT-AC86U上传GT-AC2900固件或者反之，都是没有办法刷进去的！

### <font color="#f57332">八、重要命令</font>
以下操作需要使用支持SSH协议的软件，连接到路由器后台进行操作，如果不会使用，可以参考下面步骤：

1. **启用SSH：** 在路由器后台的【系统管理】-【系统设置】里，将【启用 SSH】更改为`LAN only`，将端口号设置为`22`或者其它数字，点击页面下方【应用本页面设置】保存更改；
2. **登录SSH：** 下载SSH软件，如putty（[官方绿色版putty 0.74下载地址](https://the.earth.li/~sgtatham/putty/0.74/w64/putty.exe)），运行后在Host Name（or IP address）处输入路由器的局域网IP地址，如：`192.168.50.1`或者`router.asus.com`，端口为上一步中【SSH 端口】中的端口，如果没有更改，则为`22`，点击【Open】，如果有弹出Putty Security Alert，点击【是】；在界面的`login as`后面输入`路由器的登录帐号`后回车，然后在 password: 提示符后输入`路由器登录密码`后回车（记住：输入密码的时候不会有任何显示，输入完成后直接回车即可），完成登录。
3. **键入命令：** 键入命令时建议将系统输入法切换为英文，也可以复制命令后使用右键即可粘贴命令，粘贴完毕后按回车即可执行命令。

#### <font color="#00BFFF">1. 软件中心重置</font>

- 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，直接在ssh客户端内运行下面的程序即可。

```bash
koolshare-reset
```

#### <font color="#00BFFF">2. 清空JFFS空间</font>

- 注意，此操作会删除jffs分区内的所有文件，包括但不限于：软件中心、安装的证书、TrafficAnalyzer的数据库、自定义的设备图标等
```bash
kill -9 $(pidof skipd)
cd /jffs && rm -r .[a-zA-Z_]* *
reboot
```

#### <font color="#00BFFF">3. 删除软件中心</font>

- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件；
- 如果是在**官改固件**下删除软件中心，路由器重启后软件中心会重新初始化为最初状态。
```bash
kill -9 $(pidof skipd)
cd /jffs && rm -rf .asusrouter .koolshare db ksdb config/* etc/profile
reboot
```

#### <font color="#00BFFF">4. 重启软件中心</font>

- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
sh /koolshare/perp/perp.sh
```

#### <font color="#00BFFF">5. RT-AC86U查询坏块命令</font>
- 先重启一次路由器，再输入以下命令进行查询，返回信息的行数即为坏块的数量
```bash
dmesg |grep "bad block"
```

### <font color="#f57332">九、固件下载</font>

- 以下固件下载服务器由海波云[Hypo.cn](https://www.hypo.cn/?from=ksbbs) 友情赞助！

#### <font color="#DC143C"> **386.3_2**</font>

MD5: 209D5241222D6539E0B14A46D27B3403

SHA1: 3FF70AF85947E1A544EF07C96571A398E72C8920

下载链接：[RT-AC86U_386.3_2](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.3_2_cferom_ubi_ca3f6fc_koolshare.w)

#### <font color="#DC143C"> **386.3_0**</font>

MD5: 3E0524E124838200F2937203C28F37A3

SHA1: A759EAA6239EA03FDBBC1732CAA0B2915F25D2C2

下载链接：[RT-AC86U_386.3_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.3_0_cferom_ubi_31c92d0_koolshare.w)

#### <font color="#DC143C"> **386.2_6**</font>

MD5: 42CDCF0C4067BD1E6D14CF179FA635FA

SHA1: 87D81FB01E3BB1E1E837B85191885339071D21BA

下载链接：[RT-AC86U_386.2_6](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.2_6_cferom_ubi_b5aa6f4_koolshare.w)

#### <font color="#DC143C"> **386.2_4**</font>

MD5: D5BDDA0894A4AE8AC2E2B8219DE6E3F8

SHA1: 19CB62F8A9BE51021D6329E575DBE4EFC4F6CF71

下载链接：[RT-AC86U_386.2_4](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.2_4_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.2_2**</font>

MD5: 924B4CB4E0E5D1B66074C277C33FAB3F

SHA1: B88515C98B727E702CCF92AD471F4F969A76C16C

下载链接：[RT-AC86U_386.2_2_cferom_ubi_koolshare.w](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.2_2_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.2_0**</font>

MD5: F9C550E68B2C0635AEC05422CCEE8C34

SHA1: D186EAFFE5923008983EA58BF6D097BD5F8E7120

下载链接：[RT-AC86U_386.2_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.2_0_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.1_2**</font>

MD5: 586D354F85F0F126EDB89249D7D4A37D

SHA1: 6DDC7685B129F5E6037FBD655523BED00838AF4A

下载链接：[RT-AC86U_386.1_2](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.1_2_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.1_0**</font>

MD5: 586D354F85F0F126EDB89249D7D4A37D

SHA1: 01FA448CD57D0C146AED8D483C9BB38CC3D70FB1

下载链接：[RT-AC86U_386.1_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/RT-AC86U/RT-AC86U_386.1_0_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **384.19_0**</font>

MD5: A7D269D59718C11239BDE30BA1D57F98

SHA1: AB6BB897B559DBF99180836B4C969DC5E39C7462

下载链接：[RT-AC86U_384.19_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.19_0/RT-AC86U_384.19_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.18_0**</font>

MD5: A5BEB0C090DD2A4148519060DA7D9152

SHA1: B86990F3272D836F1DE3DD3DC93826B3EF6774EE

下载链接：[RT-AC86U_384.18_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.18_0/RT-AC86U_384.18_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.17_0**</font>

MD5: 82C6E00EBA8CBB1CBAAAB07A100116FC

SHA1: 11C0E0D013ADDCF38DC78C767A46234E5BB90386

下载链接：[RT-AC86U_384.17_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.17_0/RT-AC86U_384.17_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.16_0**</font>

MD5: B8445688FB26DD0640C59A436BBE194D

SHA1: 074F7279F1DE79D289D4D47F17EBA340CDB2F38F

下载链接：[RT-AC86U_384.16_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.16_0/RT-AC86U_384.16_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.15_0**</font>

MD5: 40983753BAE4639936D0251D8E8DA490

SHA1: 7E4C90E8F22E547AA5AB9FE681212FCCCBF1EB11

下载链接：[RT-AC86U_384.15_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.15_0/RT-AC86U_384.15_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.14_0**</font>

MD5: 1D40542191C757A1D4701F37340F3F6E

SHA1: 856EB5E8CECEA835BB04438F2E2148BEF9756236

下载链接：[RT-AC86U_384.14_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.14_0/RT-AC86U_384.14_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.13_1**</font>

MD5: EBDCE8EB8B0E8EF5E96FB4D10F561B3B

SHA1: 867FE9B58ED02F2C5D1F8E825FE630384233FBB5

下载链接：[RT-AC86U_384.13_1](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.13_1/RT-AC86U_384.13_1_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.12_0**</font>

MD5: 310FE492E955A1060F19C43914C9BD95

SHA1: 6FE246AA29737B2D8A8A896A473F2608883C3CD9

下载链接：[RT-AC86U_384.12_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.12_0/RT-AC86U_384.12_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.11_2**</font>

MD5: 88882109E03C9319B7F09B7C0DC9C7C1

SHA1: 2031FB03A481DE3FEC14689A5F435D3A3956838A

下载链接：[RT-AC86U_384.11_2](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.11_2/RT-AC86U_384.11_2_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.11_0**</font>

MD5: E2256AB26BCCB9CD022ADD472B5E50BD

SHA1: 7605A8D7924DBFA6593A1B80360F0AF4169DEDFC

下载链接：[RT-AC86U_384.11_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.11_0/RT-AC86U_384.11_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.10_2**</font>

MD5: 7B7AD42C538811A3F14589FCC4985887

SHA1: 98F8A59573F3C3A680CDCA308F3877182C0236A9

下载链接：[RT-AC86U_384.10_2](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.10_2/RT-AC86U_384.10_2_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.10_0**</font>

MD5: 5835B03E3C6ACC911F2360FC305F5047

SHA1: E8487880D605E5D93F794B47DB00691549A361CE

下载链接：[RT-AC86U_384.10_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.10_0/RT-AC86U_384.10_0_cferom_ubi-koolsahre.w)

#### <font color="#DC143C"> **384.9_0**</font>

MD5: 6897B70983E944260BD9DCCC0F2E5D1A

SHA1: 7BF76484705A32C17DF662AD933FF30D301CB8AF

下载链接：[RT-AC86U_384.9_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.9_0/RT-AC86U_384.9_0_cferom_ubi-koolsahre-wg.w)

#### <font color="#DC143C"> **384.8_2**</font>

MD5: C8BF3A085202A11822F5957307EDA8FD

SHA1: 0FF4AC6522331A2F7233252665F8C472E43939B2

下载链接：[RT-AC86U_384.8_2](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.8_2/RT-AC86U_384.8_2_cferom_ubi-koolsahre.w)

#### <font color="#DC143C"> **384.8_0**</font>

MD5: 707C2978243F7A480DBFA4994FF4C853

SHA1: 632466E2D7D5E7C160F6939D565589E900C6464A

下载链接：[RT-AC86U_384.8_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.8_0/RT-AC86U_384.8_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.7_0**</font>

MD5: 91A19286CB5F4DD17C93A3196651B5F1

SHA1: 40BA092771AC7F2C452A9AC3E1B8F4354D49A1D8

下载链接：[RT-AC86U_384.7_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.7_0/RT-AC86U_384.7_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.6_0**</font>

MD5: 26C887303BC62FD807B21F89E5005091

SHA1: 4A141590F6B3D268D68A81C265791829E17E0444

下载链接：[RT-AC86U_384.6_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.6_0/RT-AC86U_384.6_0_cferom_ubi-koolshare.w)

#### <font color="#DC143C"> **384.5_0**</font>

MD5: 38B3DEFFEF236DC985D7DD62F0C1C7C6

SHA1: 62F7306EE903DC27A2306BD1A0229C99EFC474B1

下载链接：[RT-AC86U_384.5_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.5_0/RT-AC86U_384.5_0_cferom_ubi-update1.w)

#### <font color="#DC143C"> **384.4_0**</font>

MD5: 82D191A33CEBE58E034E5C64BD6A3C2E

SHA1: 09F7FFD94A9EF0C453DB92765209C72951E92591

下载链接：[RT-AC86U_384.4_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/384.4_0/RT-AC86U_384.4_0_ubi-koolshare.w)

#### <font color="#DC143C"> **382.1_2**</font>

MD5: AA945C19C24D260FDB2765E9F9E6A26B

SHA1: 774F939F380A52FBDA867AC74814A5CB5324460A

下载链接：[RT-AC86U_382.1_2](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/382.1_2/RT-AC86U_382.1_2_ubi-koolshare.w)

#### <font color="#DC143C"> **382.1_1**</font>

MD5: 33F30B6A2E61B6CD7553B0B3320ACF09

SHA1: 2411EBD15607C7C85D2D912D99256BB32C4BA8FC

下载链接：[RT-AC86U_382.1_1](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/382.1_1/RT-AC86U_382.1_1_ubi-koolshare.w)

#### <font color="#DC143C"> **382.1_0**</font>

MD5: 53B29C08553D236269D72313B8860039

SHA1: CFE609B6029881660F86438E7C73104973D6E7CF

下载链接：[RT-AC86U_382.1_0](http://fw.koolcenter.com/Koolshare_RMerl_New_Gen_384/RT-AC86U/382.1_0/RT-AC86U_382.1_0_ubi-koolshare.w)
[/hide]



