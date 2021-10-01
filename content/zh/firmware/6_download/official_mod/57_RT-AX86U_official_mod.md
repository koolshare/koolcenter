---
title: "RT-AX86U 官改固件[384]"
linkTitle: "RT-AX86U [384]"
type: docs
weight: 57
toc_hide: true
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：384_9318；更新日期：2020年11月27日； <font color="red">状态：停止维护，建议使用386官改固件</font>
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

**重要的事情说三遍**

<font color="#DC143C">注意3：如果你的RT-AX86U的2.5G网卡不是博通BCM54991，请不要刷384版本的官改固件！</font>

<font color="#DC143C">注意3：如果你的RT-AX86U的2.5G网卡不是博通BCM54991，请不要刷384版本的官改固件！</font>

<font color="#DC143C">注意3：如果你的RT-AX86U的2.5G网卡不是博通BCM54991，请不要刷384版本的官改固件！</font>

**如何检测RT-AX86U 2.5G网卡**：软件中心下载并使用cfe工具箱即可检测！

### <font color="#f57332">二、固件特色</font>

> 官改固件的开发初衷是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。详情FAQ: Q7。
> 
> 所以：**官改固件 = 官方固件 + 为了软件中心进行必要的最小化改动 + 软件中心**

1. 使用官方固件源代码为基础修改，官方固件有的功能官改固件都有，比如AiMesh等；
2. koolshare软件中心支持，RT-AX86U为axhnd.675x平台，兼容hnd/axhnd平台软件中心和所有插件。

### <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕`RT-AX86U`机型，其它机型请勿使用本固件！
- 本固件同样支持 `RT-AX86U高达限量版`，此版本机器请刷`384_9262`及更新版本，固件定制UI将不会丢失。
- 如果你的RT-AX86U出厂固件是386版本，请不要刷384版本的官改固件！

### <font color="#f57332">四、更新日志</font>

#### <font color="###00BFFF">384_9318（2020年11月27日）</font>

> 此版本中（384\_9318），华硕官方修复了RT-AX86U的【Traffic Analyzer 流量分析】等其他上个固件有明显bug的地方，并且加入了UU加速器。当然还有其它的一些安全、稳定性方面的更新。这个版本的固件也许是最后一两个RT-AX86U的384版本的固件了，不久以后，RT-AX86U将进入386版本，一起期待吧~

1. 同步ASUS最新RT-AX86U代码：GPL_RT_AX86U_30043849318；
2. 更新内置koolshare软件中心到1.6.5版本；

#### <font color="###00BFFF">384_9262（2020年07月26日）</font>

> - 此版本中（384\_9262），华硕官方修复了RT-AX86U的链路聚合问题，不过华硕384\_9262版本官方固件中存在的其它问题，在384\_9262\_koolshare可能仍然会存在，比如【Traffic Analyzer 流量分析】功能不显示流量统计的问题。这些问题等待华硕修复后，本帖会同步更新其修复。

1. 同步ASUS最新RT-AX86U代码：GPL_RT_AX86U_30043849262；
2. 关闭固件强制自动更新功能，以免用户更新到ASUS官方固件而失去软件中心功能；
3. 更新内置koolshare软件中心到1.6.1版本；
4. 修复AX86U官改固件作为`AiMesh路由`时，无法为同样是官改固件的AiMesh节点更新固件的问题；
5. 现在AX86U官改固件作为`AiMesh节点`时，其web后台也能正常访问了！

> **针对384_9262第`5`点更新的说明如下，请仔细阅读：**
> - 华硕对AiMesh节点仅开放了固件更新这一个页面功能，这限制得太多了，但是这也是为了避免用户对节点进行设置造成mesh网络出问题；
> - kooldev将AiMesh节点的web后台访问全部开放了，但是需要提醒大家请尽量不要改动与AiMesh相关的设定，以免影响AiMesh网络的正常工作；
> - 我们开放AiMesh节点的web后台的访问，主要目的是为了大家能在AiMesh节点中使用软件中心，当然你也可以进行一些固件相关的设定，比如无线区域。
> - 需要注意的是因为AiMesh节点本质上是工作在中继模式，而非NAT模式，所以一些透明代理类的插件在AiMesh节点路由上是无法正常工作的，比如xxxx，kp等；
> - 如果你在AiMesh节点中修改了某些系统设置导致AiMesh网络失效，请在开机状态下长按机器后面的`reset`按钮重置你的AiMesh节点路由，然后用主路由重新添加节点；
> - AiMesh节点web后台的访问方式：在AiMesh主路由的【网络地图】页面点击【AiMesh节点】图标，然后在页面右侧会出现目前已经连接的AiMesh节点，点击对应节点机器后，会弹出节点信息，信息中会显示该节点机器的ip地址，比如我的是`192.168.82.126`，然后在浏览器中访问http://192.168.82.126即可访问AiMesh节点路由。


#### <font color="###00BFFF">384_9173_r1（2020年06月03日）</font>
> 384_9173_r1为384_9173的小幅更新版本，刷机后固件版本号仍然显示384_9173不变 。判断更新是否成功可以看【外部网络(WAN)】-【互联网连接】处是否多了NAT Type的选项。
> 其它华硕384_9173版本官方固件中存在的问题，在koolshare 384_9173_r1可能仍然会存在，比如【网络监控家 Adaptive QoS】功能不显示客户端网速等问题。这些问题等待华硕修复后，本帖会同步跟进。

1. 添加fullcone NAT支持，功能位于【外部网络(WAN)】-【互联网连接】-【NAT Type】；
2. 修复华硕AiCloud 2.0无法使用的问题；
3. 修复RT-AX86U官改固件软件中心环境变量问题；
4. ipset 6.3.1升级为ipset 7.6版本；

#### <font color="###00BFFF">384_9173（2020年05月22日）</font>
> 根据调查，RT-AX86U第一批出货的自带固件384_9106版本，并且可以更新到最新官方384_9173版本（华硕RT-AX86U第一个官方release版本），此次官改固件推出的就是384_9173官方固件对应的官改固件。相比于上个版本（384_8256）的官改固件：
> 1. 384_9173版本支持链路聚合功能。
> 2. 384_9173版本wifi改区支持澳大利亚。
> 3. 384_9173版本支持手游加速功能和OPEN NAT功能（仍然没有UU加速器）。
> 
> **建议：**
> 1. `384_8256官改固件`刷`384_9173官改固件`后，恢复出厂设置一次，并全部重新手动配置。
> 2. `384_xxxx官方固件`刷`384_9173官改固件`后，恢复出厂设置一次，并全部重新手动配置。

1. RT-AX86U第2个官改版本，同步华硕GPL代码：`GPL_RT-AX86U_3.0.0.4.384.9173` ；
2. 修复适配第一个官改版本（384_8256）中的一些小问题；

#### <font color="###00BFFF">384_8256（2020年05月13日）</font>
> RT-AX86U第一批出货的自带固件可能比384.8256版本更加新，主要有以下区别：
> 1. 384_8256版本不带链路聚合功能，同步更新源码后可支持。
> 2. 384_8256版本wifi改区仅支持中国和美国，同步更新源码后可支持澳大利亚。
> 3. 384_8256版本的日志详细程度会更细，如果看到很多kernel开头的日志，请别惊慌，这是正常的。
> 4. 刷完384_8256后，如果AiMesh功能消失，需要重置路由器才能出现。
> 5. 不论是此版本的官改固件还是目前最新的官方固件（384_9173），都不支持UU加速器！不排除以后会支持。
> 
> 以上问题基本不影响日常使用，如果在意，可以等下次官改固件更新。如果有新的问题，你也可以加入AX86U固件交流群反馈更多问题。

1. RT-AX86U第一个官改版本，基于华硕GPL代码：`GPL_RT-AX86U_3.0.0.4.384.8256` 制作；
2. 添加koolshare软件中心支持，以及软件中心支持相关的开机脚本支持等；

### <font color="#f57332">五、刷机步骤</font>

- 约定`原厂固件`为华硕官方的RT-AX86U固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于[华硕官方RT-AX86U源代码](https://www.asus.com/Networking/RT-AX86U/HelpDesk_Download/)修改而来的带软件中心的[官改固件](https://koolshare.cn/thread-181845-1-1.html)。

#### <font color="#00BFFF">A. 原厂 刷 官改：</font>
1. 在原产固件的固件升级页面下直接上传.w 后缀的RT-AX86U官改固件文件；
2. 刷机完成后会自动重启，此时刷机完成（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
3. 重启后先将路由器连上网络，然后进入软件中心将软件中心更新到最新版本。

#### <font color="#00BFFF">B. 官改 刷 官改：</font>
1. 在本帖下载并刷过官改固件的，在固件升级页面下直接上传.w 后缀的官改固件文件即可（如无特殊说明，刷机完成后不用恢复出产设置）；
2. 刷机后所有已经安装的插件都会被保留，不会受到影响。

#### <font color="#00BFFF">C. 官改 刷 原厂</font>
1. 在官改固件升级页面下直接上传.w 后缀的原产固件文件（如无特殊说明，刷机完成后不用恢复出产设置，当然恢复一次更好）；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如果需要彻底恢复，执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框）；或者参见后文【<font color="#f57332">**重要命令/操作**</font>】中的【<font color="#DC143C">**清空jffs空间**</font>】或者【<font color="#DC143C">**删除软件中心**</font>】。

### <font color="#f57332">六、注意事项：</font>

1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（cttrl + F5）后重试；
2. 强烈建议使用chrome浏览器或者chrome内核的浏览器，以保持最佳兼容性；
3. 恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。
4. 由于固件来自官改，jffs分区是默认开启的，没有格式化软件中心的选项，如果需要重置软件中心（不影响jffs分区其它数据），请登录ssh后运行<font color="#DC143C">**软件中心重置命令**</font>（见下文：重要命令）
5. RT-AX86U的jffs空间只有47MB，如果开启Traffic Analyzer，将会消耗不少空间，请酌情开启；

### <font color="#f57332">七、FAQ</font>

- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年11月27日

**Q1：我的路由器搜不到wifi信号。**

**A1：**首先排除网络客户端设备的问题，然后请尝试下面的方法：
1. 论坛常有人推荐将wifi区域切换到澳大利亚地区来改善信号强度，这确实管用，因为澳大利亚区域的最大发射功率要大一些。但是由于每个国家设备支持的信道不同，加上一些终端设备信道支持的限制，就可能会导致某些设备无法搜索到wifi信号。建议：1 在哪个国家就使用哪国的信道设置，2 如果一定要使用澳大利亚，请经信道固定在国内支持的信道范围。
2. 搜不到wifi信号的时候，在路由器管理界面 **【无线网络】** - **【一般设置】** 中查看到该信号的信道变成了**0**，这首先可能是无意间或者某个未知错误导致该wifi信号被关闭（ **【无线网络】** - **【专业设置】** - **【启用无线网络】** 处于 **否** 状态），另一种可能是虽然无线是启用状态，但是当前信道仍然显示为0，遇到此情况建议设置固定信道看是否能解决。如果无论如何都无法解决，建议你走售后渠道更换机器。

**Q2：我手动安装第三方xxx插件失败怎么办？**

**A2：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。
1. 目前对于armv8机型（hnd/axhnd/axhnd.675平台）：RT-AC86U，GT-AC5300，RT-AX88U，GT-AX11000，TUF-AX3000，RT-AX86U，这几款机器在本论坛的固件，插件是可以通用的。
2. 除非你要安装的插件作者明确表示他的插件可以用于hnd/axhnd/axhnd.675平台）平台软件中心，或者插件来源于rogsoft项目内本身的插件，才可以安装！！
3. 具体来说，目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd/axhnd软件中心](https://github.com/koolshare/rogsoft)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！即使他们可能都使用了1.5代软件中心！！具体各个不同平台的软件中心的区别，大家可以参考此处：[koolshare几个版本的软件中心区别](https://github.com/koolshare/armsoft/blob/master/README.md#koolshare%E5%87%A0%E4%B8%AA%E7%89%88%E6%9C%AC%E7%9A%84%E8%BD%AF%E4%BB%B6%E4%B8%AD%E5%BF%83%E5%8C%BA%E5%88%AB)。

**Q3：软件中心一直显示更新中怎么办？**

**A3：**此问题可能由多种原因导致，请尝试下面的方法：

1. 访问[https://rogsoft.ddnsto.com/](https://rogsoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。<font color="#DC143C">1）</font>：可能是本地网络故障，通过putty、xshell等SSH软件连接路由器后，输入命令：`ping armsoft.ddnsto.com`看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定。<font color="#DC143C">2）</font>：也可能是软件中心服务器正在维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考<font color="#DC143C">**重启软件中心命令**</font>（见下文：重要命令部分）。
3. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考<font color="#DC143C">**软件中心重置方法**</font>（见下文：重要命令部分）。
4. 如果以上步骤尝试完后不行，那么检查下【Tools】-【Sysinfo】的【JFFS】一栏，看是否是显示`unmounted`，如果显示`unmounted`，表明jffs分区未成功挂载，此时请尝试对路由器进行双清操作（恢复出厂+格式化jffs分区），并尝试多次重启，如果最后成功挂载，将会显示jffs分区的使用容量信息。
5. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考参考<font color="#DC143C">**RT-AX86U查询坏块命令**</font>（见下文：重要命令部分）。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q4：刷机后软件中心一片空白**

**A4：**按照下面的顺序依次尝试：
1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载RT-AX86U的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock8 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：**重要命令**里的软件中心重置命令，来重置一次软件中心。然后基本上就能看到软件中心页面了。

**Q5：华硕发了RT-AX86U固件，为什么此帖还不更新官改固件啊？**

**A5**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的xxx固件无线有问题，能否修复？**

**A6**：无线问题基本无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：可不可给固件以增加xxx功能？**

**A7**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：**
非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

### <font color="#f57332">八、重要命令</font>

#### <font color="#00BFFF">1. 软件中心重置命令</font>

- 直接在ssh客户端内运行`koolshare-reset`命令即可。

#### <font color="#00BFFF">2. 清空jffs空间</font>
- 注意，此操作会删除jffs分区内的所有文件，包括但不限于：软件中心、安装的证书、TrafficAnalyzer的数据库、自定义的设备图标等
```bash
kill -9 $(pidof skipd)
rm -r .[a-zA-Z_]* *
reboot
```

#### <font color="#00BFFF">3. 删除软件中心</font>
- 适用于**官改固件**刷回**原厂固件**，需要删除留在jffs分区内软件中心，而不删除其它文件。
- 如果是在**官改固件**下删除软件中心，重启路由，路由会自动重新安装软件中心。
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

#### <font color="#00BFFF">5. RT-AX86U查询坏块命令</font>
- hnd/axhnd机型上查询坏块的方法已经不适用于axhnd.675x平台
- axhnd.675x平台查询坏块的命令如下（运行以下命令，返回数字即为坏块数量）：
```bash
# 运行以下命令，返回数字即为坏块数量
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

#### <font color="#DC143C"> **384_9318**</font>

MD5: 8180BB6B3AAF40529A55F35B53FBAC1B

SHA1: 9F7C1FB8B9599E2F92F180B3B57035B55883055D

下载链接：[RT-AX86U_384_9318_koolshare_cferom_pureubi_20201127.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX86U/RT-AX86U_384_9318_koolshare_cferom_pureubi_20201127.w)

#### <font color="#DC143C"> **384_9262**</font>

MD5: FEC7E48ADD3E8B6F74755225C8447E95

SHA1: 3D70F2521533DDFC64DBBF210D3F7DF66DA04971

下载链接：[RT-AX86U_384_9262_koolshare_cferom_pureubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX86U/RT-AX86U_384_9262_koolshare_cferom_pureubi.w)

#### <font color="#DC143C"> **384_9173_r1**</font>

MD5: FEC7E48ADD3E8B6F74755225C8447E95

SHA1: 3D70F2521533DDFC64DBBF210D3F7DF66DA04971

下载链接：[RT-AX86U_384_9173_koolshare_cferom_pureubi_r1.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX86U/RT-AX86U_384_9173_koolshare_cferom_pureubi_r1.w)

#### <font color="#DC143C"> **384_9173**</font>

MD5: B27B6E1B6CE490E707857F996113C4DE

SHA1: 0BE7D12222023A4F9848B58ED560E157CD742482

下载链接：[RT-AX86U_384_9173_koolshare_cferom_pureubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX86U/RT-AX86U_384_9173_koolshare_cferom_pureubi.w)

#### <font color="#DC143C"> **384_8256**</font>

MD5: 558F9D8ED7A4230C6C53745C9FE9342E

SHA1: B18760F879DFDB10D2B444B80776BE94B7ACB3A4

下载链接：[RT-AX86U_384_8256_koolshare_cferom_pureubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/RT-AX86U/RT-AX86U_384_8256_koolshare_cferom_pureubi.w)
