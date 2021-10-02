---
title: "GT-AX11000 官改固件"
linkTitle: "GT-AX11000"
type: docs
weight: 30
toc_hide: false
hide_summary: false
date: 2021-09-29
author: "sadog"
tags: ["华硕官改固件"]
categories: ["固件下载"]
description: >
  最新版本：384_7979，更新日期：2020年05月07日
---

<font color="#FF0066" style="font-size:1.5rem;line-height:1.8;font-weight:bold">广告：固件/软件中心维护不易，如果您支持我们的工作，可以考虑购买软件中心的[ddnsto](https://www.ddnsto.com/)和wifi boost，以支持开发者，谢谢！</font>

### <font color="#f57332">一、刷机须知</font>

注意1：请刷机的朋友认真阅读本帖！！！刷机带来的风险请自行承担！！！

注意2：欢迎转载本帖，但是请一定尊重开发组的成果，注明本帖来源！！！

### <font color="#f57332">二、固件特色</font>

1. 本固件使用官方固件源代码为基础（非merlin固件代码）修改而来；
2. 保持官方固件功能原汁原味的基础上增加一些功能，如ipset，base64，tproxy，wan-start，nat-start等功能；
3. koolshare软件中心支持（1.5代，不兼容一代），软件中心为ROG皮肤；
4. GT-AX11000U作为axhnd平台，兼容hnd平台的RT-AC86U和GT-AC5300的软件中心和所有插件
5. 尽可能的修复一些官方固件的bug;
6. wireguard原生内核支持。

### <font color="#f57332">三、支持机型</font>

- 本固件仅支持华硕`ROG Rapture GT-AX11000`机型，其它机型请勿使用本固件！
- GT-AX11000使命召唤黑色行动版本同样支持

###  <font color="#f57332">四、更新日志</font>

#### <font color="##00BFFF">384_7979_koolshare（2020年05月07日）</font>
1. 同步ASUS最新GT-AX11000代码：GPL of ASUS GT-AX11000 for firmware 3.0.0.4.384.7979；
2. 更新内置软件中心到最新1.5.5版本；
3. 华硕下载大师以及asusware环境相关的软件包不再内置，以减小固件包大小；
4. 侧边栏UI跟随华硕样式（从384_6208开始华硕改了侧边栏图标和字体样式，当时嫌太丑没有同步），刷了此版本后侧边栏图标显示不正常的，请使用CTRL + F5强制刷新浏览器缓存。

#### <font color="##00BFFF">384_6436_koolshare（2019年12月03日）</font>
1. 同步ASUS最新GT-AX11000代码：GPL of ASUS GT-AX11000 for firmware 3.0.0.4.384.6436；
2. 固件内置wireguard更新至0.0.20191127版本；

#### <font color="##00BFFF">384_6208_koolshare（2019年09月23日）</font>
1. 同步ASUS最新GT-AX11000代码：GPL of ASUS GT-AX11000 for firmware 3.0.0.4.384.6208；
2. 回滚华硕对主界面侧边栏字体和图标的更改，回滚到5252版本的外观（因为华硕改得实在太丑了）；
3. 现在登陆路由器后默认进入【网络地图】页面，而不是【Dash Board】页面；
4. 固件内置wireguard更新至0.0.20190913版本；
5. 更新内置软件中心到最新1.4.7版本；

#### <font color="##00BFFF">384_5252_koolshare（2019年04月19日）</font>
1. 同步ASUS最新GT-AX11000代码：GPL of ASUS GT-AX11000 for firmware 3.0.0.4.384.5252；
2. 添加ipset、curl、wireguard等支持；
3. 添加dnsmasq ipset支持，dnsmasq conf-dir，dnsmasq postconf支持；
4. 添加开机启动脚本支持：wan-start，nat-start，service-start，init-start，post-mount支持；
5. busybox添加base64支持（不可描述订阅会用到），netstat -p支持等；
6. 网络地图默认显示cpu、内存等状态而非5G状态；
7. 关闭华硕固件自动更新功能；
8. 添加koolshare软件中心支持。

### <font color="#f57332">五、刷机步骤（请仔细阅读）：</font>
- 约定`原厂固件`为华硕官方GT-AX11000固件。
- 约定`官改固件`为koolshare开发组在本帖发布的基于华硕官方GT-AX11000源代码修改而来，且带软件中心的固件。

#### <font color="##00BFFF">A. 原厂刷官改：</font>
1. 在`原产固件`升级页面下直接上传.w 后缀的`官改固件`文件。
2. 刷机完成后会自动重启，此时刷机完成
3. 如无特殊说明，刷机完成后可以不恢复出产设置，当然恢复一次更好。

#### <font color="##00BFFF">B. 官改刷官改</font>
1. 在本帖下载并刷过旧版本`官改固件`的，直接上传.w 后缀的新版本`官改固件`文件即可。
2. 刷机完成后会自动重启，刷机后所有已经安装的插件都会被保留，不会受到影响。
3. 如无特殊说明，刷机完成后不需要恢复出产设置。

#### <font color="##00BFFF">C. 官改刷原厂</font>
1. 在`官改固件`升级页面下直接上传.w 后缀的`原厂固件`文件；
2. 刷机完成后固件恢复为官方固件，但是jffs分区可能仍然留有一些软件中心相关文件；
3. 如果需要彻底恢复，执行一次恢复出厂设置（同时勾选恢复按钮旁边的选择框）。

### <font color="#f57332">六、注意事项：</font>
1. 刷机后如果界面显示不正常，请尝试清空浏览器缓存（cttrl + F5）后重试；
2. 强烈建议使用chrome浏览器或者chrome内核的浏览器，以保持最佳兼容性；
3. 恢复出厂设置并不能完全清除jffs分区的软件中心文件，需要在恢复出厂设置的时候同时勾选恢复按钮旁边的选择框。
4. 由于固件自官方改版而来，jffs分区是默认开启的，没有格式化软件中心的选项，如果需要重置软件中心（不影响jffs分区其它数据），请登录ssh后运行软件中心重置命令（见下文：重要命令）
5. 不同于RT-AC86U 512MB内存的机器，GT-AX11000有1GB内存，一般情况下不需要虚拟内存也能流畅运行各种第三方插件。
6. <font color="#DC143C">**请不要使用离线安装来安装AM380 merlin固件的任何插件，不然肯定会造成问题！！！给GT-AX11000离线安装插件一定要是hnd/axhnd平台的机器（目前包括：RT-AC86U，GT-AC5300，RT-AX88U，GT-AX11000）。详情见下文FAQ：Q2**</font>

### <font color="#f57332">七、FAQ</font>
- 此处列出一些经常被问到的问题（FAQ）的回答，持续更新中~
- FAQ更新日期：2020年05月07日

**Q1：华硕GT-AX11000会出梅林固件吗？**

**A1**：见[梅林固件原作者回答第一条](https://www.snbforums.com/threads/faq-read-me-first-before-posting-a-question.47153/)；因为没有梅林固件，所以就没有梅林改版固件。基于同样的原因，koolshare开发组才为该机型开发了koolshare官改固件。

**Q2：我的路由器搜不到wifi信号。**

**A2：** 首先排除网络客户端设备的问题，然后请尝试下面的方法：
1. 论坛常有人推荐将wifi区域切换到澳大利亚地区来改善信号强度，这确实管用，因为澳大利亚区域的最大发射功率要大一些。但是由于每个国家设备支持的信道不同，加上一些终端设备信道支持的限制，就可能会导致某些设备无法搜索到wifi信号。建议：1 在哪个国家就使用哪国的信道设置，2 如果一定要使用澳大利亚，请经信道固定在国内支持的信道范围。
2. 收不到wifi信号的时候，在路由器管理界面**【无线网络】**-**【一般设置】**中查看到该信号的信道变成了**0**，这首先可能是无意间或者某个未知错误导致该wifi信号被关闭（**【无线网络】**-**【专业设置】**-**【启用无线网络】**处于**否**状态），另一种可能是虽然无线是启用状态，但是当前信道仍然显示为0，遇到此情况建议设置固定信道看是否能解决。如果无论如何都无法解决，建议你走售后渠道更换机器。

**Q3：我手动安装第三方xxx插件失败怎么办？**

**A3：** 目前各个平台的软件中心也没有提供严格的插件开发规范，加上论坛的插件区管理比较混乱，没有进行良好的插件审核，所以经常有一些第三方插件无法兼容所有软件中心平台，但是却能在这些平台上进行安装。
1. 目前对于armv8机型（hnd/axhnd平台）：RT-AC86U，GT-AC5300，RT-AX88U，GT-AX11000，这几款机器在本论坛的固件，插件是可以通用的。
2. 除非你要安装的插件作者明确表示他的插件可以用于hnd/axhnd平台软件中心，或者插件来源于armsoft内本身的插件，才可以安装！！
3. 具体来说，目前koolshare开发组推出的几个版本的软件中心：[arm380软件中心](https://github.com/koolshare/koolshare.github.io)，[arm384软件中心](https://github.com/koolshare/armsoft)，[hnd/axhnd软件中心](https://github.com/koolshare/rogsoft)，[LEDE-酷软](https://github.com/koolshare/ledesoft)，他们的插件都是互不兼容的！即使他们可能都使用了1.5代软件中心！！具体各个不同平台的软件中心的区别，大家可以参考此处：[koolshare几个版本的软件中心区别](https://github.com/koolshare/armsoft/blob/master/README.md#koolshare%E5%87%A0%E4%B8%AA%E7%89%88%E6%9C%AC%E7%9A%84%E8%BD%AF%E4%BB%B6%E4%B8%AD%E5%BF%83%E5%8C%BA%E5%88%AB)。

**Q4：软件中心一直显示更新中怎么办？**

**A4：** 此问题可能由多种原因导致，请尝试下面的方法：
1. 访问[https://armsoft.ddnsto.com/](https://rogsoft.ddnsto.com/)，如果显示`Hello to everyone`字样，表示你的路由访问软件中心服务器没有问题；如果不显示上述字样，则表示是网络问题。<font color="#DC143C">1）</font>：可能是本地网络故障，通过putty、xshell等SSH软件连接路由器后，输入命令：`ping armsoft.ddnsto.com`看是否能ping通服务器，如果无法解析ip地址，可以尝试更换路由器dns设定。<font color="#DC143C">2）</font>：也可能是软件中心服务器正在维护，建议可以加本论坛相关讨论群组，可以第一时间获得相关信息。
2. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep httpdb|grep -v grep`，如果有输出内容表明软件中心web服务运行正常，如果输出内容为空表明软件中心web服务运行异常，请参考<font color="#DC143C">**重启软件中心命令**</font>（见下文：重要命令部分）。
3. 可以通过putty、xshell等SSH软件连接路由器后，输入命令：`ps|grep skipd|grep -v grep`，如果有输出内容表明软件中心数据库服务运行正常，如果输出内容为空表明软件中心数据库服务运行异常，可以尝试通过运行命令`service restart_skipd`来重启skipd服务。如果运行重启skipd的命令后，再次运行`ps|grep skipd|grep -v grep`仍然没有输出，说明储存在jffs分区的skipd数据库可能遭到了损坏，此时可以请参考<font color="#DC143C">**软件中心重置方法**</font>（见下文：重要命令部分）。
4. 如果以上步骤尝试完后不行，那么检查下【Tools】-【Sysinfo】的【JFFS】一栏，看是否是显示`unmounted`，如果显示`unmounted`，表明jffs分区未成功挂载，此时请尝试对路由器进行双清操作（恢复出厂+格式化jffs分区），并尝试多次重启，如果最后成功挂载，将会显示jffs分区的使用容量信息。
5. 最严重的情况，路由器的jffs分区遇到了很多无法屏蔽的坏块，查看路由器有多少坏块，先重启路由器，然后用putty、xshell等SSH软件连接路由器后，输入命令`dmesg|grep "bad block"`，显示几行，就表明有多少个坏块。一般来说，两三个坏块是正常品控水平，如果坏块太多，建议走售后渠道。

**Q5：华硕发了GT-AX11000新固件，为什么此贴还不更新官改固件啊？**

**A6**：官改固件是来源于对华硕放出的固件源代码的修改，并不是固件本身。华硕固件发布后一般会在2周到2个月之间放出源代码，此时才能进行修改工作，修改过程还涉及到一些测试、回炉工作，因此请大家看到华硕固件出来后<font color="#DC143C">**不要催更！**</font>我一般都会在源码放出来后第一时间更新的！

**Q6：我的GT-AX11000固件xxx版本无线有问题，能否修复？**

**A6**：无线问题无能为力，因为华硕使用的是博通商业代码，无线这部分在固件源代码里是不开源的，没法进行任何修改或者调整。

**Q7：可不可给固件以增加xxx功能？**

**A7**：基本不可以，本官改固件的开发宗旨是在尽量保持ASUS官方固件原汁原味的基础上，增加软件中心及对应插件的支持。所以一些官方固件所有的问题，在官改固件中也可能会遗传。koolshare固件开发组会尽量对一些ASUS已知的bug进行修复，不过仅限于非常重要的。

**Q8：我现在已经是xxx的版本，用着挺稳定，看见本帖更新了最新固件，我还需要跟随最新版本升级吗？升级后稳定吗？升级后需要恢复出厂设置吗？**

**A8：** 非常建议升级！最新的固件版本不仅有来自ASUS官方的一些功能更新，也会包含ASUS官方的一些安全更新、稳定性更新，一般来说会比老版本固件更加稳定。同时，koolshare软件中心和相关插件也是持续为最新版本的官改固件进行更新的，所以是强烈建议升级到最新版本的官改的。另外已经刷过koolshare官改固件的，升级到最新koolshare官改固件，如无特殊说明，是不需要做恢复出厂设置等操作的，固件升级后所有的插件都会得到保留。

**Q9：刷机后软件中心一片空白**

**A9：** 按照下面的顺序依次尝试：
1. 在【系统管理】-【系统设置】里开启SSH功能，然后通过putty、Xshell等SSH软件连接到路由器后台后，输入命令：`mount | grep /jffs`，如果看到类似`/dev/mtdblock8 on /jffs type jffs2 (rw,noatime)`这样的输出，说明/jffs成功挂载了，挂载设备为/dev/mtdblock8。如果没有任何输出，则说明/jffs分区没有成功挂载，请尝试重启路由、重置路由等操作后再次查看jffs分区是否成功挂载，如果仍然不行，尝试运行以下命令手动挂载GT-AC5300的jffs分区：`mount -t jffs2 -o rw,noatime /dev/mtdblock8 /jffs`，运行完毕后再次`mount | grep /jffs`，检查是否成功挂载。如果手动挂载还是不行，那么可能是FALSH有问题或者是系统有问题，这种建议售后渠道换机了。
2. 如果jffs分区挂载没有问题，软件中心页面还是空白，可以尝试使用下文：**重要命令**里的软件中心重置命令，来重置一次软件中心。然后基本上就能看到软件中心页面了。

### <font color="#f57332">八、重要命令</font>

#### <font color="##00BFFF">1. 软件中心重置方法</font>

- 软件中心出现问题需要重置软件中心的，可以解决大部分问题；
- 由于jffs坏块或者硬件问题导致的软件中心问题，重置是不管用的，建议及时换机。

##### 1.1 使用命令重置：
- 需要开启固件的ssh功能，然后使用putty等ssh客户端登陆进路由器，依次输入以下命令，即可重置软件中心。
```bash
# 1. 关闭软件中心相关进程，删除软件中心文件
kill -9 $(pidof skipd)
cd /koolshare/perp && sh perp.sh stop
cd / && rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db

# 2. 重置软件中心
jffsinit.sh
cd /koolshare/perp && sh perp.sh start
service restart_skipd

# 3. 重启路由器（可选）
reboot

# 4.浏览器进入软件中心，将软件中心版本更新到最新，安装插件...
```

##### 1.2 使用命令重置：
GT-AX11000官改固件，可以直接在ssh客户端内运行`koolshare-reset`命令即可，其效果应该等同上面的手动输入命令。

#### <font color="##00BFFF">2. 清空jffs空间</font>

- 注意，此操作会删除jffs分区内的所有文件，包括但不限于：软件中心、安装的证书、TrafficAnalyzer的数据库、自定义的设备图标等

```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/.sys /jffs/.wtfast /jffs/*
reboot
```

#### <font color="##00BFFF">3. 删除软件中心</font>
- 如果是刷回了官方固件，在此环境下执行以下命令，可以删除留在jffs分区内软件中心相关文件，而不删除其它文件。
- 如果是在官改固件下，在此环境下执行以下命令，那么软件中心删除后，重启路由，路由会自动重新安装软件中心。
```bash
kill -9 $(pidof skipd)
rm -rf /jffs/.asusrouter /jffs/.koolshare /jffs/db /jffs/config/* /jffs/etc/profile
reboot
```

### <font color="#f57332">九、固件下载</font>

- 以下固件下载服务器由海波云[Hypo.cn](https://www.hypo.cn/?from=ksbbs) 友情赞助！

#### <font color="#DC143C"> **384_7979**</font>

MD5: 72F1DF7DD100E17A962DC7BF66E55C4B

SHA1: 5192E9ACA50E97DCB0F9C024F1226C4A270EACA4

下载链接：[GT-AX11000_384_7979_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/GT-AX11000/ROG_Rapture_GT-AX11000_3.0.0.4.384_7979/GT-AX11000_384_7979_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_6436**</font>

MD5: 12817187F3FD306A650A765C17B6C90F

SHA1: 9DBB98E5672149BEEF170197B01C1710D4271952

下载链接：[GT-AX11000_384_6436_koolshare_cferom_ubi.w](https://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/GT-AX11000/ROG_Rapture_GT-AX11000_3.0.0.4.384_6436/GT-AX11000_384_6436_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_5252**</font>

MD5: E586481F1D10F397D17AE7DD850009D5

SHA1: 450DA3294EFB2F71C4D67253D2761B883DAEDD51

下载链接：[GT-AX11000_384_5252_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/GT-AX11000/ROG_Rapture_GT-AX11000_3.0.0.4.384_5252/GT-AX11000_384_5252_koolshare_cferom_ubi.w)

#### <font color="#DC143C"> **384_6208**</font>

MD5: C51F5BC7207BCD7A4BFD69556DE764DB

SHA1: F05110EDA167D2689909AD7BD247D3DFF78F1C87

下载链接：[GT-AX11000_384_6208_koolshare_cferom_ubi.w](http://firmware.koolshare.cn/Koolshare_ASUS_Official_Mod/GT-AX11000/ROG_Rapture_GT-AX11000_3.0.0.4.384_6208/GT-AX11000_384_6208_koolshare_cferom_ubi.w)



