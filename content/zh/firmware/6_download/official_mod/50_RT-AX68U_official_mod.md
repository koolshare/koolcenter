---
title: "RT-AX68U 官改固件"
linkTitle: "RT-AX68U"
type: docs
weight: 50
toc_hide: false
hide_summary: false
date: 2021-10-1
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：386_41947，更新日期：2021年02月05日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>
1. 使用[RT-AX68U华硕官方固件源代码](https://www.asus.com/Networking/RT-AX68U/HelpDesk_Download/)为基础修改而来；
2. 官方固件有的功能，改版固件都有，如UU加速器、AiMesh2.0等；
3. 开放RT-AX68U作为AiMesh节点时可以通过IP地址访问其web后台；
4. 固件后台界面优化：字体优化，首页默认显示状态页面；
5. 增加一些软件中心/插件需要用到的功能，如dnsmasq with ipset、base64、一些内核模块支持等；
6. koolshare软件中心支持：[hnd软件中心](https://github.com/koolshare/rogsoft#rogsoft)；

### <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕`RT-AX68U`机型，其它机型请勿使用本固件！

### <font color="#f57332">四、更新日志</font>

####  <font color="#00BFFF">386_41947（2021年02月5日）</font>

1. 基于华硕GPL代码：`GPL_RT-AX68U_3.0.0.4.386.41947` 制作；
2. 添加koolshare软件中心支持，以及软件中心支持相关的开机脚本、内核模块等支持；

### <font color="#f57332">五、刷机步骤</font>

- 约定`原厂固件`为华硕官方的RT-AX68U固件：[RT-AX68U华硕官方固件下载地址](https://www.asus.com.cn/Networking/RT-AX68U/HelpDesk_BIOS/)；
- 约定`官改固件`为koolshare开发组在[本贴](https://koolshare.cn/thread-191640-1-1.html)发布的基于[华硕官方RT-AX68U源代码](https://www.asus.com/Networking/RT-AX68U/HelpDesk_Download/)修改而来的带软件中心的官改固件，版本号为官方固件版本号后加上`_koolshare`后缀，如RT-AX68U官改固件版本：`3.0.0.4.386_41947_koolshare`。

> - 刷机建议使用chrome浏览器，或者chromium内核的浏览器进行刷机操作。
> - 刷机后如提示手动重启路由器，请等待几分钟后再手动开关电源进行重启。
> - 刷官改固件后如果软件中心页面一片空白，建议再手动重启一次路由器，如果仍然空白，参见FAQ：Q3。

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
- FAQ更新日期：2021年02月3日

**Q1：我离线安装第三方xxx插件失败怎么办？**

**A1：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。

1. 本贴的RT-AX68U属于axhnd.675x平台机型，对于hnd/axhnd/axhnd.675平台机型，使用的是rogsoft软件中心，这些机型的插件是可以通用的，具体请见：[rogsoft机型支持](https://github.com/koolshare/rogsoft#机型支持)；
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
8. 最后，最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，参考下文：重要命令里的==RT-AX68U查询坏块命令==。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q3：刷机后软件中心一片空白**

**A3：** 按照下面的顺序依次尝试：

1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep -w /jffs`，如果看到类似`/dev/mtdblock9 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为`/dev/mtdblock9`，最后的数字9会根据机型/平台的不同而不同。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载TUF-AX3000的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock9 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：重要命令里的==软件中心重置命令==，来重置一次软件中心，然后应该就能看到软件中心页面了。

**Q4：华硕发了RT-AX68U固件，为什么此帖还不更新官改固件啊？**

**A4**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">不要催更！</font>我一般都会在源码放出来后第一时间更新的！

**Q5：我的xxx版本固件无线有问题，能否修复？**

**A5：** 无线问题无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q6：可不可给固件以增加xxx功能？**

**A6**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。另外，添加功能是软件中心的使命，软件中心就是为此而生的；

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

#### <font color="###00BFFF">5. RT-AX68U查询坏块命令</font>
- hnd/axhnd机型上查询坏块的方法已经不适用于axhnd.675x平台
- axhnd.675x平台查询坏块的命令如下（运行以下命令，返回数字即为坏块数量）：
```bash
cat /sys/class/mtd/mtd6/bad_blocks
```

### <font color="#f57332">九、固件下载</font>

- 以下固件下载服务器由海波云[Hypo.cn](https://www.hypo.cn/?from=ksbbs) 友情赞助！

#### <font color="#DC143C"> **386_41947**</font>

MD5: 44C46F6FD60ECFF26F771AFCFCEDD76A

SHA1: 954BA11E121E58E1906597226A32CF5EC044729B

下载链接：[RT-AX68U_386_41947_koolshare_cferom_pureubi.w](https://fw.koolcenter.com/Koolshare_ASUS_Official_Mod/RT-AX68U/RT-AX68U_386_41947_koolshare_cferom_pureubi.w)


