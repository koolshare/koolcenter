---
title: "RT-AC86U 官改固件"
linkTitle: "RT-AC86U"
type: docs
weight: 40
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_40451，更新日期：2021年01月14日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>
> 官改固件的开发初衷是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。
>
> 所以：**官改固件 = 官方固件 + 为了软件中心进行必要的最小化改动 + 软件中心**

1. 使用官方固件源代码为基础修改，官方固件有的功能官改固件都有，比如AiMesh等；
2. koolshare软件中心支持，RT-AC86U为hnd平台，兼容hnd/axhnd/axhnd.675x平台软件中心和所有插件。

### <font color="#f57332">三、支持机型</font>

本固件仅支持型号为`RT-AC86U`的机型，其它机型请勿刷本固件

###  <font color="#f57332">四、更新日志</font>


###  <font color="#00BFFF"> 386_41634（2021年04月10日）</font>

1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.386.41634。
2. 内置软件中心版本更新至1.7.1版本；

####  <font color="#00BFFF"> 386_40451（2021年01月14日）</font>

> - 从此版本开始，华硕RT-AC86U固件正式进入386大版本，在功能上，该版本主要更新了AiMesh 2.0和Ookla® SPEEDTEST，当然也包含很多其它稳定性、安全性方面的更新。强烈建议大家进行升级！
> - 从384固件升级到386固件也是非常顺畅的，升级后不恢复出厂设置也是没问题的。当然稳妥起见，建议有时间的朋友还是做一次恢复出厂设置，然后在干净的配置上重新手动配置一次固件。

1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.386.40451。
2. 内置软件中心版本更新至1.6.7版本；

####  <font color="#00BFFF"> 384_82072（2020年10月12日）</font>

1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.82072。
2. 去除更多哥特（Gothic）风格字体，因为其显示中文的时候字体发虚，实在太丑；
3. 内置软件中心更新至1.6.4，添加实时日志、提升插件安装/卸载速度！详情见： [软件中心更新日志](https://github.com/koolshare/rogsoft/blob/master/softcenter/Changelog.txt) 
4. 现在使用RT-AC86U官改固件作为`AiMesh节点`时，其web后台能正常访问了！
5. 更改软件中心数据库文件夹：jffs/db → jffs/ksdb;

> **针对RT-AC86U 384_82072第`4`点更新的说明如下，请仔细阅读：**
> - 华硕对AiMesh节点仅开放了固件更新这一个页面功能，这限制得太多了，但是这也是为了避免用户对节点进行设置造成mesh网络出问题；
> - kooldev将AiMesh节点的web后台访问全部开放了，但是需要提醒大家请尽量不要改动与AiMesh相关的设定，以免影响AiMesh网络的正常工作；
> - 我们开放AiMesh节点的web后台的访问，主要目的是为了大家能在AiMesh节点中使用软件中心，当然你也可以进行一些固件相关的设定，比如无线区域。
> - 需要注意的是因为AiMesh节点本质上是工作在中继模式，而非NAT模式，所以一些透明代理类的插件在AiMesh节点路由上是无法正常工作的，比如xxxx，kp等；
> - 如果你在AiMesh节点中修改了某些系统设置导致AiMesh网络失效，请在开机状态下长按机器后面的`reset`按钮重置你的AiMesh节点路由，然后用主路由重新添加节点；
> - AiMesh节点web后台的访问方式：在AiMesh主路由的【网络地图】页面点击【AiMesh节点】图标，然后在页面右侧会出现目前已经连接的AiMesh节点，点击对应节点机器后，会弹出节点信息，信息中会显示该节点机器的ip地址，比如我的是`192.168.86.126`，然后在浏览器中访问http://192.168.86.126即可访问AiMesh节点路由。

####  <font color="#00BFFF"> 384_81918（2020年06月21日）</font>

1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.81918。
2. 重大变动：此版本固件UI由ROG UI更换为ASUSWRT UI，骚红皮肤，再见。
3. 更新内置软件中心到最新1.6.0版本；
4. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】。

####  <font color="#00BFFF"> 384_81352（2020年04月24日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.81352。
2. 更新内置软件中心到最新1.5.5版本；

####  <font color="#00BFFF"> 384_81351（2019年11月23日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.81351。
2. **好消息**：此版本华硕更新了ASUS DDNS的Let's Encrypt证书申请，从使用80端口网页验证更换成了使用acme.sh，并用DNS记录进行验证。所以现在大家可以在DDNS配置页面配置DDNS的同时申请到证书了！（如果申请失败，可以关掉不可描述之类的，多尝试几次）

####  <font color="#00BFFF"> 384_81049（2019年10月31日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.81049，此版本有几个重要的安全更新，强烈建议升级！
2. 回滚华硕对主界面侧边栏字体和图标的更改，回滚到45717版本的外观（因为华硕改得实在太丑了）；
4. 固件内置wireguard更新至0.0.20191012版本；
5. 更新内置软件中心到最新1.4.7版本；

####  <font color="#00BFFF"> 384_45717（2019年06月27日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.45717，此版本有几个重要的安全更新，强烈建议升级！
2. 同步内置软件中心为最新版本。
3. 把本帖的内容和排版更新了下，添加了FAQ部分，请大家关注~

####  <font color="#00BFFF"> 384_45713（2019年04月26日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.45713;
2. 同步内置软件中心为最新版本。

####  <font color="#00BFFF"> 384_45149（2018年11月12日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.45149，包含大量的安全性更新和稳定性修复，因此建议使用官改的朋友尽快升级到这个版本。
2. 因为华硕这次的更新为Alexa和IFTTT 更新了新功能，其中部分功能会与Server酱插件冲突导致无法上网，现在暂时没有找到更好的兼容方案前，移除了这次华硕为IFTTT 更新的客户端上线通知的功能。
3. 内核添加原生的wireguard支持，并且添加wg管理工具，现在用户可以自己在路由器内手动配置wireguard，配置方法参见wireguard官网。不会配置的可以等wireguard插件，目前已经完工60%，预计春节前放出。
4. 更新了内置的软件中心，并且添加了`koolshare-reset`命令，用户在ssh或者telnet客户端内输入`koolshare-reset`即可一键重置软件中心，效果等同下文中的：软件中心重置命令，用于软件中心出问题的、或者需要切换皮肤的用户。
5. 关闭了384.45149官方固件中新增的固件强制自动更新功能，因为这可能会导致官改用户被自动升级回官方固件。
6. 网络地图首页更改为默认显示路由器状态，而不是wifi 接口状态。

#### <font color="#00BFFF">384_32799（2018年11月12日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.32799；
2. 修复一个官方固件自带的bug，该bug会导致ebtables和ipsec无法启动，现在可以正常启动了。

#### <font color="#00BFFF">384_32797（2018年09月14日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.32797；
2. 更新软件中心内置的skipd数据库到最新版本：修复lz4压缩问题，解决因储存一些值导致软件中心崩溃的问题；
3. 同步内置软件中心为最新版本。

#### <font color="#00BFFF">384_21140（2018年07月31日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.21140。

#### <font color="#00BFFF">384_21045（2018年07月29日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.21045。

#### <font color="#00BFFF">384_20648（2018年05月18日）</font>
1. 同步ASUS最新RT-AC86U代码：GPL of ASUS RT-AC86U for firmware 3.0.0.4.384.20648；
2. 移植ROG皮肤；
3. 添加软件中心支持。

### <font color="#f57332">四、刷机步骤</font>
- 约定`原厂固件`为华硕官方的RT-AC86U固件。
- 约定`原版ML`为国外RMerl大神基于华硕官方固件源代码修改而来的[ML固件](https://asuswrt.lostrealm.ca/)
- 约定`改版ML`为koolshare开发组在发布的的基于[ML固件](https://github.com/RMerl/asuswrt-ML.ng)修改而来的带软件中心的[ML改版固件](http://koolshare.cn/thread-127878-1-1.html)；
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方RT-AC86U源代码](https://www.asus.com.cn/Networking/RT-AC86U/HelpDesk_Download/)修改而来的带软件中心的[官改固件](http://koolshare.cn/thread-139965-1-1.html)。

#### <font color="#00BFFF">A. 原厂固件/原版ML → 官改：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好！

1. 在原产固件/原版ML固件升级页面下直接上传.w 后缀的TUF-AX3000官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### <font color="#00BFFF">B. 官改固件 → 官改固件：</font>

> 如无特殊说明，刷机完成后不用恢复出产设置！

1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.w 后缀的官改固件文件即可!
2. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="#00BFFF">C. 改版ML → 官改固件：</font>

> 如无特殊说明，刷机完成后不用恢复出厂设置，当然恢复一次更好！

1. 在改版ML固件升级页面直接上传.w后缀的本帖提供的官改固件，路由自动重启后刷机完成；
2. 如果你刷低于384_81918版本的官改固件，请参考下文重要命令里的==软件中心重置==，才能将皮肤从asuswrt风格切换为rog风格；
3. 如果你刷高于/等于384_81918版本的官改固件，则不需要对软件中心进行重置。

#### <font color="#00BFFF">D. 官改固件 → 改版ML：</font>

> 如无特殊说明，刷机完成后不用恢复出厂设置，当然恢复一次更好！

1. 在官改固件升级页面下直接上传.w后缀的[改版ML固件](http://koolshare.cn/thread-127878-1-1.html)，路由自动重启后刷机完成；
2. 如果你从低于384_81918版本的官改固件刷改版ML固件，请参考下文重要命令里的==软件中心重置==，才能将皮肤从rog风格切换为asuswrt风格；
3. 如果你从高于/等于384_81918版本的官改固件刷改版ML固件，则不需要对软件中心进行重置。

#### <font color="#00BFFF">E. 官改固件 → 原厂固件：</font>

> 从官改固件刷回原厂固件，以下第3点或第4点操作，请选择一个来操作。当然你也可以不进行这个操作，让软件中心文件保留在官方固件的JFFS分区，以后你刷回官改固件，软件中心就会恢复成上次官改的状态。

1. 在官改固件升级页面下直接上传.w 后缀的华硕原厂固件文件；
2. 刷机完成后固件恢复为官方固件，但是JFFS分区仍然会保留有一些软件中心相关文件；
3. 你可以参考下文重要命令里的==删除软件中心==，将JFFS内残留的软件中心文件删除；
4. 也可以执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框），这样也将清空JFFS内除软件中心外的其它文件

### <font color="#f57332">五、注意事项：</font>

1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（ctrl + F5）后重试；
2. 强烈建议使用Chrome浏览器或者Chromium内核的浏览器，以保持最佳兼容性；
3. 单纯的恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。
4. 由官改固件的JFFS分区是默认开启的，没有格式化jffs分区的选项，如果需要重置软件中心，请参考下文：重要命令里的==软件中心重置==
5. 86U的jffs空间只有47M，如果开启Traffic Analyzer功能，将会消耗不少jffs空间，论坛里已经出现不少jffs空间被Traffic Analyzer的数据爆掉jffs空间的例子，所以此功能请酌情开启；

### <font color="#f57332">六、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年10月25日

**Q1：RT-AC86U改版ML和官改固件比较有什么区别，哪个好用，哪个更稳定？**

**A1：** 改版ML固件基于ML固件修改，官改固件基于官方固件修改。两者都是在基础固件代码上以添加软件中心为目的。相比官改固件，ML改版固件有更多的功能和bug修复，而官改固件更新较快。好用程度差别不大，稳定性来说也基本无差，选哪个固件基于个人喜好即可。

**Q2：我手动安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。

1. 本贴的RT-AC86U属于hnd平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
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
4. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==RT-AC86U查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：软件中心页面一片空白**

**A4：** 按照下面的顺序依次尝试：

1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载RT-AC86U的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心。然后基本上就能看到软件中心页面了。

**Q5：华硕发了RT-AC86U最新固件，为什么此贴还不更新官改固件啊？**

**A5**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的xxx固件无线有问题，能否修复？**

**A6**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：RT-AC86U现在还需要挂载虚拟内存吗？**

**A7**：随着华硕对固件的不断更新，现在已经越来越完善和稳定，大多数时候都可以摆脱虚拟内存了。不过这里还是建议大家都使用虚拟内存，因为虽然86U使用了512M的内存，但是实际上只有430M可用内存，有82M被博通硬件占用了。加上固件使用了glibc库，对于嵌入式设备来说还是太重了，glibc的软件体积较大，内存占用较多，最终导致实际在界面上看到剩余200多M的剩余内存。挂载虚拟内存后大多数情况下都看不到虚拟内存的使用，但是系统的稳定性会大大增强，，特别是对一些golang语言写的程序的运行会有很大改善。虚拟内存的制作与开启，建议使用86U软件中心提供的`虚拟内存插件`，U盘插2.0和3.0接口均可，建议512M虚拟内存即可。

**Q8：我现在已经是384.xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如果没有特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件和设置都会得到保留。

**Q9：华硕GT-AC2900路由器硬件和RT-AC86U几乎一样，固件通刷吗？**

**A9**：不通刷！不通刷！不通刷！虽然在硬件上一样，但是不同机器有不同的cfe设定，固件是能对不同机型进行识别的，即使你给RT-AC86U上传GT-AC2900固件或者反之，都是没有办法刷进去的！

**Q10：可以为RT-AC86U官改固件添加xxx功能不？**

**A10**：一般来说我都会拒绝。首先，本固件秉持最大化保留官方固件功能的基础上添加软件中心，为大家带来原生的体验；其次，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q11：RT-AC86U官改固件以后还会坚持更新吗？**

**A11**：之前给RT-AC86U做官改固件的初衷是因为其ML固件不支持AiMesh功能，现在ML固件已经支持了AiMesh功能，所以从这点上来看，已经没有必要跟进RT-AC86U的官改固件了。目前只要我还有时间和精力，会保持RT-AC86U做官改固件的更新，但是也随时有可能在未来的某个版本停止RT-AC86U官改固件的维护更新。

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
- 注意，此操作会删除jffs分区内的**所有文件**，包括但不限于：软件中心、SSL证书、自定义的设备图标等；
- 命令运行完毕后路由器会自动重启；
- 如果是在**官改固件**下清空JFFS空间，路由器重启后软件中心会重新初始化为最初状态；
```bash
kill -9 $(pidof skipd)
cd /jffs && rm -r .[a-zA-Z_]* *
reboot
```
#### <font color="#00BFFF">3. 删除软件中心</font>
- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件。
- 如果是在**官改固件**下删除软件中心，路由器重启后软件中心会重新初始化为最初状态；
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db /jffs/ksdb /jffs/config/* /jffs/etc/profile
reboot
```
#### <font color="#00BFFF">4. 重启软件中心</font>
- 当软件中心相关进程挂掉的时候，此时可以用ssh进入路由器后台，输入以下命令重启软件中心：
```bash
sh /koolshare/perp/perp.sh
```
#### <font color="#00BFFF">5. RT-AC86U查询坏块命令</font>

- 建议先重启一次路由器，再输入以下命令进行查询，返回信息的行数即为坏块的数量

```bash
dmesg |grep "bad block"
```
### <font color="#f57332">九、固件下载</font>

- 以下固件下载服务器由海波云[Hypo.cn](https://www.hypo.cn/?from=ksbbs) 友情赞助！

### <font color="#DC143C"> **386_41634**</font>

MD5: 0926E336655277D1EE33893D3396F287

SHA1: D860ED0434A2F213A7CFDBA20D0B6856FCA330CD

下载链接：[RT-AC86U_386_41634_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_386_41634_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **386_40451**</font>

MD5: 48FFC95537BB926C90BB2992E6D9C421

SHA1: 7BE853AF602B96F25EEA89A29B53936E8E911D07

下载链接：[RT-AC86U_386_40451_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_386_40451_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_82072**</font>

MD5: A405D4688880B176C1C5F32B9F5E3691

SHA1: 738355307BB57054DD152FA7F2B5C4544C5EEFE5

下载链接：[RT-AC86U_384_82072_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_82072_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_81918**</font>

MD5: 7CFF1A892D029D2545B2E76484C8BA35

SHA1: 3BAE06A8F0366EC09D77A2A8F330B6A97678D7D2

下载链接：[RT-AC86U_384_81918_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_81918_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_81352**</font>

MD5: E979B10E86B62413E96E77DE12BEFD96

SHA1: 8F37B117165825BD707DF26D8F20C548718667FE

下载链接：[RT-AC86U_384_81352_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_81352_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_81351**</font>

MD5: D8366EFD87F890C9ECB542A0D93AED5F

SHA1: 4799BCBDC2DA219D75F324D17D9BFDC955A5CBA1

下载链接：[RT-AC86U_384_81351_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_81351_koolshare_cferom_ubi.w)


#### <font color="#DC143C"> **384_81049** </font>
MD5: 0E11EE86A62249B7CE9885C648CCF3B8

SHA1: 0E9875E296D50BA4CCE36E98918D1178BE1A7B85

下载链接：[RT-AC86U_384_81049_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_81049_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_45717**</font>
MD5: 93A397256C2A2C9A4F3368D885EE80FA

SHA1: E366D347E71DC597CAC1B1DA375A560DE614BF93

下载链接：[RT-AC86U_384_45717_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_45717_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_45713**</font>

MD5: 05C5C0DD22C8DD2C10A6BC170BEBB78D

SHA1: E7B9D30BC26E9859D44EF3B2A2E537C45A0946D6

下载链接：[RT-AC86U_384_45713_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_45713_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_45149**</font>
MD5: 1B896670F65402C2850FA3FA8235C332

SHA1: B414B09C9F4FEB08106AE3753C8BCC40E17A4232

下载链接：[RT-AC86U_384_45149_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_45149_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_32799**</font>
MD5: 3E477C01D18CD455362B61DCCBF33652

SHA1: A2C496EE545A94EADAC4CEC3C9B3A381B1B4ABB2

下载链接：[RT-AC86U_384_32799_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_32799_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_32797**</font>
MD5: 59E2B58FC231747F0B02659696E87200

SHA1: 83FBDBC78AD77C76E342DB3F4451459EFC5C9080

下载链接：[RT-AC86U_384_32797_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_32797_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_21140**</font>

MD5: A0A0E59599C99E8119F71D4DE69E967A

SHA1: 450DC89917B14673DE9F10D531CDD9D7B34C579F

下载链接：[RT-AC86U_384_21140_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_21140_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_21045**</font>
MD5: 6F4906163784D670C87AE9C198811CC9

SHA1: F17799E35A62739A21C6E76D4EF2B06037667770

下载链接：[RT-AC86U_384_21045_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_21045_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_20648**</font>

MD5: 718F989E32508B1C5BC911F7D5059DC1

SHA1: EB731886F65CA2AE168F9E2D0DFFC319344A534B

下载链接：[RT-AC86U_384_20648_koolshare_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AC86U/RT-AC86U_384_20648_koolshare_ubi.w)
