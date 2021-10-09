---
title: "GT-AC2900 官改固件"
linkTitle: "GT-AC2900"
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

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>
> 
> 注意：GT-AC2900的华硕官方固件是红色的ROG皮肤，而GT-AC2900的梅林固件/梅林改版固件是ASUSWRT皮肤。
> 

1. 梅林改版固件使用梅林固件源代码为基础（[asuswrt-merlin.ng代码](https://github.com/RMerl/asuswrt-merlin.ng)）修改而来；
2. 梅林固件有的功能，梅林改版固件都有，参考此链接：[梅林固件添加的功能](https://github.com/RMerl/asuswrt-merlin.ng/blob/master/README-merlin.txt#L62-L132)；
3. 梅林固件不能使用的功能，梅林改版也不能使用，比如说UU加速器等；
4. 开放GT-AC2900作为AiMesh节点时可以通过IP地址访问其web后台；
5. 固件后台界面优化：字体优化，首页默认显示状态页面；
6. 增加一些软件中心/插件需要用到的功能，如dnsmasq with ipset、base64、一些内核模块支持等；
7. koolshare软件中心支持：[hnd软件中心](https://github.com/koolshare/rogsoft#rogsoft)；

### <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕`GT-AC2900`机型，其它机型请勿使用本固件！
- RT-AC86U虽然和GT-AC2900硬件类似，但是因其CFE不同不能通刷！

### <font color="#f57332">四、更新日志</font>

####  <font color="#00BFFF">386.3_2（2021年08月07日）</font>
1. 同步梅林固件代码386.3_2，更新日志见此：[Asuswrt-Merlin 386/NG Changelog](https://www.asuswrt-merlin.net/changelog)；
2. 同步软件中心1.7.5

####  <font color="#00BFFF">386.3_0（2021年07月30日）</font>
1. 同步梅林固件代码386.3_0，更新日志见此：[Asuswrt-Merlin 386/NG Changelog](https://www.asuswrt-merlin.net/changelog)；
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
1. GT-AC2900第一个梅林改版版本，基于梅林代码386.1_0制作；
2. 添加koolshare软件中心支持，以及软件中心支持相关的开机脚本、内核模块等支持；

### <font color="#f57332">五、刷机步骤</font>

#### <font color="#00BFFF">刷机准备</font>

- 建议下载好固件后，对固件的md5/sha1校验码进行核对，以保证固件完整性；
- 建议刷机全程使用电脑端谷歌Chrome，或者Chromium内核的浏览器进行操作；
- 如果使用了USB2JFFS插件，建议先使用卸载掉USB的挂载后在进行刷机，刷机后再进行挂载。

#### <font color="#00BFFF">固件定义</font>

- `原厂固件`为GT-AC2900华硕官方固件：[GT-AC2900华硕官方固件下载地址](https://www.asus.com.cn/Networking/ROG-Rapture-GT-AC2900/)；
- `原版梅林固件`为加拿大独立开发者Eric Sauvageau在华硕GT-AC2900官方源码上二次开发的第三方固件，相较华硕官方固件，其区别为：[这些功能](https://github.com/RMerl/asuswrt-merlin.ng/blob/master/README-merlin.txt#L62-L132)，其版本号为`386.x`，如：`386.1`；
- `改版梅林固件`为koolshare开发组在[本贴](https://koolshare.cn/thread-191639-1-1.html)发布的基于梅林固件源码再次开发而来的带软件中心的GT-AC2900梅林改版固件，其版本号和梅林原版固件保持一致，如GT-AC2900官改固件版本：`386.1`。

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

#### <font color="###00BFFF">A. 原厂固件 → 改版梅林固件</font>

> 原厂固件和原版梅林固件/改版梅林固件在一些默认配置上有所不同，虽然刷机后不用恢复出厂设置也能正常工作，但是建议有时间朋友刷机完成后双清一次路由双清后全部手动配置，不要用以前的备份配置。

1. 在`原厂固件`固件升级页面下直接上传.w 后缀的`改版梅林固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成（刷机完成后可以不恢复出产设置，当然恢复一次更好）；
3. 刷机完成在【系统管理 】–【 系统设置】内勾选：`Format JFFS partition at next boot` 和 `Enable JFFS custom scripts and configs` 然后点击`应用本页面设置`，成功后点击顶部`重启`按钮重启路由器；
4. 重启后进入web后台时先设置路由器，将路由器连上网络，然后进入软件中心，如果软件中心一片空白，不要着急，先软重启（使用顶部重启按钮）一次路由器即可出现软件中心，如果软件中心仍然空白，参见FAQ：Q3的解决办法。
5. 如果进入软件中心后正常，将软件中心更新到最新版本（如果有）后即完成全部刷机，之后你可以对路由器固件进行其它喜好的设置，或者在软件中心安装插件等操作。

#### <font color="###00BFFF">B. 原版梅林固件 → 改版梅林固件：</font>

1. 在`原版梅林固件`固件升级页面下直接上传.w 后缀的`改版梅林固件`文件；
2. 成功上传固件后，路由器会自动重启，此时刷机完成（刷机完成后可以不恢复出产设置，当然恢复一次更好）；
3. 刷机完成在【系统管理 】–【 系统设置】内勾选：`Format JFFS partition at next boot` 和 `Enable JFFS custom scripts and configs` 然后点击`应用本页面设置`，成功后点击顶部`重启`按钮重启路由器；
4. 重启后进入web后台时先设置路由器，将路由器连上网络，然后进入软件中心，如果软件中心一片空白，不要着急，先软重启（使用顶部重启按钮）一次路由器即可出现软件中心，如果软件中心仍然空白，参见FAQ：Q3的解决办法。
5. 如果进入软件中心后正常，将软件中心更新到最新版本（如果有）后即完成全部刷机，之后你可以对路由器固件进行其它喜好的设置，或者在软件中心安装插件等操作。

#### <font color="###00BFFF">C. 改版梅林固件 → 改版梅林固件</font>

1. 在`改版梅林固件`升级页面下直接上传.w 后缀的`改版梅林固件`文件，刷机完成后机器会自动重启；
2. 请阅读你刷的固件版本的更新日志，看是否有附加刷机说明（如恢复出厂，双清，格式化JFFS等），如果没有任何要求，刷机完成后可以不恢复出厂设置；
3. 刷机完成后，固件中的软件中心和所有插件都会得到保留；
4. 以上步骤完成后，固件中的软件中心和所有插件都会得到保留；
5. 如果刷机后软件中心页面一片空白，建议再手动软重启（使用顶部重启按钮）一次路由器，如果仍然空白，参见FAQ：Q3。

#### <font color="###00BFFF">D. 改版梅林固件 → 原厂固件/原版梅林固件</font>

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

---

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2021年01月31日

**Q1：我离线安装第三方xxx插件失败怎么办？**

**A1：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。

1. 本贴的GT-AC2900属于axhnd.675x平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
2. 目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd软件中心](https://github.com/koolshare/rogsoft)，[qca软件中心](https://github.com/koolshare/qca)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！具体可以参考：[koolshare几个版本的软件中心区别](https://github.com/koolshare/rogsoft#koolshare几个版本的软件中心区别)；
3. 对于第三方作者开发的插件，除非作者明确表示其支持hnd/axhnd/axhnd.675平台，不然请不要随意安装！不然因为可能没有遵循开发规范，安装后无法使用，甚至给路由器带来问题！
4. 为了论坛和固件未来更好的发展，koolshare软件中心也会针对一些特殊的插件在离线安装上有所限制。

**Q2：软件中心一直显示更新中怎么办？**

**A2：** 此问题可能由多种原因导致，请尝试下面的方法：

1. 访问https://rogsoft.ddnsto.com/，请确保你访问此网站的时候使用的是连接到该路由器下的客户端，如果显示`Hello to everyone`字样，表示你的路由下的本地网络访问软件中心服务器没有问题；如果不显示上述字样，则可能是是网络方面的问题。
2. 情况1，路由器本地网络故障：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`ping rogsoft.ddnsto.com`，看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定后再试；如果能解析ip地址当时无法ping通，可能是本地网络问题或者软件中心服务器正在维护。
3. 情况2，路由器本地网络故障：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器，输入命令：`curl -sS4L https://rogsoft.ddnsto.com/|grep Hello`，如果显示了两行内容都包含`Hello to everyone`字样，表明路由器访问软件中心web服务器没有问题；如果没有以上显示，可能是本地网络问题或者软件中心服务器正在维护。
4. 情况3，服务器网络故障：这有可能是koolshare软件中心服务器维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
5. 如果排除了以上网络故障，那么可能是程序运行方面的问题。可以进行以下操作：开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep -w httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考下文：重要命令里的==重启软件中心==以解决httpdb没有运行的问题。
6. 开启路由器SSH功能后，通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考下文：重要命令里的软件中心重置。
7. 还有一种较为常见的情况，在刷机过程中，jffs分区中存放的软件中心相关文件在刷机过程/路由器断电/重启过程中被破坏了，如果被破坏的文件正好是httpdb、软件中心数据库等关键文件，也会导致软件中心一直显示更新中的情况。虽然部分情况下，替换损坏的文件可以修复此问题，但是由于无法知晓是否有其它的文件损坏，所以这种情况下建议对路由器进行双清操作，双清完成后，路由器jffs分区内的软件中心相关文件会得到重建，然后在此基础上手动安装插件并手动配置，切记不要使用以前的jffs分区备份来进行恢复！
8. 最后，最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==GT-AC2900查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q3：刷机后软件中心一片空白**

**A3：** 按照下面的顺序依次尝试：

1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`，最后的数字9会根据机型/平台的不同而不同。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载TUF-AX3000的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心，然后应该就能看到软件中心页面了。

**Q4：Rmerl发布了最新的GT-AC2900梅林固件，为什么此贴还不更新梅林改版固件啊？**

**A4：** 新梅林改版固件的发布涉及大到大量的源代码合并工作，期间还涉及到一些编译、测试、回炉等工作，不过一般来说梅林原版固件更新后1天-1周内，就会完成编译和测试工作。

**Q5：我的xxx固件无线有问题，能否修复？**

**A5：** 无线问题无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q6：可不可给固件以增加xxx功能？**

**A6**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q7：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A7：** 非常建议升级！最新的固件版本不仅有来自ASUS官方（asuswrt）和梅林（asuswrt-merlin）的一些功能更新，也会包含ASUS官方和梅林的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本梅林改版固件进行更新的，所以是强烈建议升级到最新版本koolshare梅林改版固件的。另外已经刷过koolshare梅林改版固件的，升级到最新koolshare梅林改版固件，一般来说没有特殊说明，是不需要做恢复出厂设置等操作的，所有的插件都会得到保留。

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

#### <font color="###00BFFF">5. GT-AC2900查询坏块命令</font>

- 先重启一次路由器，再输入以下命令进行查询，返回信息的行数即为坏块的数量
```bash
dmesg |grep "bad block"
```

### <font color="#f57332">九、固件下载</font>

- 以下固件下载服务器由海波云[Hypo.cn](https://www.hypo.cn/?from=ksbbs) 友情赞助！

#### <font color="#DC143C"> **386.3_2**</font>

MD5: 1EAD88D902DE0AE593C9F7A1534E3044

SHA1: A691ADEC81A057B0D209E1D3894942123685181E

下载链接：[GT-AC2900_386.3_2_cferom_ubi_ca3f6fc_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.3_2_cferom_ubi_ca3f6fc_koolshare.w)

#### <font color="#DC143C"> **386.3_0**</font>

MD5: 153F51549968ADE966375C4F3D3C11A7

SHA1: AE223616A9CAF85957647A32BD765378DEA828DB

下载链接：[GT-AC2900_386.3_0_cferom_ubi_31c92d0_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.3_0_cferom_ubi_31c92d0_koolshare.w)

#### <font color="#DC143C"> **386.2_6**</font>

MD5: 280975823123B1154283F22661D1CF16

SHA1: E8EE0EE8386C23F5AD4E5AF36A7726EF72826F22

下载链接：[GT-AC2900_386.2_6_cferom_ubi_b5aa6f4_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.2_6_cferom_ubi_b5aa6f4_koolshare.w)

#### <font color="#DC143C"> **386.2_4**</font>

MD5: F54D375F3C5DBE2B835BA1DF5A784D70

SHA1: D0EEC4D215F1E7BAB3345714C77C4F30CDDB0B2A

下载链接：[GT-AC2900_386.2_4_cferom_ubi_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.2_4_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.2_2**</font>

MD5: 1B1A3D8B792DF173FE44AE8A96445CC5

SHA1: 4E1EA4745BA7B315EE309E7E69CFF8721CA63F35

下载链接：[GT-AC2900_386.2_2_cferom_ubi_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.2_2_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.2_0**</font>

MD5: 1BE676882602DE99E4FD0F459E8D010D

SHA1: 4E1EA4745BA7B315EE309E7E69CFF8721CA63F35

下载链接：[GT-AC2900_386.2_0_cferom_ubi_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.2_0_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.1_2**</font>

MD5: 64056D9FBE3B4891A54C81855FEC9BBD

SHA1: 763843A346375C61CC08B39406EEF412D0F81E19

下载链接：[GT-AC2900_386.1_2_cferom_ubi_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.1_2_cferom_ubi_koolshare.w)

#### <font color="#DC143C"> **386.1_0**</font>

MD5: D1454E94BB9867106B940BD99A5DC6A9

SHA1: DB6CBFB7B71AE6AA8AF18492D891B1E842854E77

下载链接：[GT-AC2900_386.1_0_cferom_ubi_koolshare.w](https://fw.koolcenter.com/Koolshare_RMerl_New_Gen_386/GT-AC2900/GT-AC2900_386.1_0_cferom_ubi_koolshare.w)

