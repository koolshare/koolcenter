---
typora-root-url: ../../../..
typora-copy-images-to: ../../../../article/image
title: "U盘替换NAND的JFFS教程"
linkTitle: "U盘替换NAND的JFFS教程"
date: 2021-09-18
author: "lonlykids"
coverImg: "/article/image/blog/usbjffs-cover.jpg"
tags: ["USB2JFFS"]
categories: ["高级玩法"]
description: >
  AC86UASUS固件改版用，U盘替换NAND的JFFS教程。
---

_本帖最后由 lonlykids 于 2020-8-22 13:02 编辑_  
  
1.把你的U盘插入机器(要先格式化成ext3或者ext4文件系统,可以跟虚拟内存用同一个U盘,不影响)  
2.在U盘根目录建立jffs文件夹(通常挂载后在/tmp/mnt/sda1 , 具体以实际情况为主)  
3.下载附件解压 (软件中心已上架~用软件中心的吧~U盘不达标的 , 可以用我这个....)

 ![Boom.rar.pdf](https://www.koolshare.cn/forum.php?mod=attachment&aid=MzAwNzI4fGRhMWQ1YWZhfDE2MzE5NTAxMzR8MjM4MHwxNjEwMTc%3D) 

4.把解压出来的5个文件上传到/jffs/scripts/(**注意要先备份/jffs/scripts/文件夹,方便还原(不然只有格式化jffs救回)**) \_>这里的/jffs/scripts/是机器的 , 不是U盘的 , 别复制错了.  
5.SSH到路由器.然后输入以下命令  
    1)     chmod a+x /jffs/scripts/post-mount  
    2)     chmod a+x /jffs/scripts/unmount  
    3)     chmod a+x /jffs/scripts/wan-start  
    4)     chmod a+x /jffs/scripts/nat-start  
    5)     chmod a+x /jffs/scripts/services-start  
or  
  
    1)     chmod a+x /jffs/scripts/\*  
6.重启你的路由器  
  
7.Enjoy~  
  
  
  
PS : 此脚本还有改进的空间.但是..懒..而且不保证完全没有Bug.建议在玩之前备份一下jffs分区.有啥问题可以跟帖.我有空会看看.  
PS2: 在用了此脚本后重启完的2分钟内会有几次重启httpd的现象,具体表现是登陆进路由器后会被踢出来到登陆界面(这个是改进的地方.不影响使用.有空再改) \[Fixed\]  
PS3: 同样.用了此脚本后.重启完会发现内存占用情况比以前多一丢丢.其实是cache来的..用软件中心的ROG工具箱释放一下内存即可(也可以无视) \[Fixed\]  
  
PS4: 用了之后.发现以前好多奇奇怪怪的log信息没有了.比如 kernel: jffs2: warning: (851) jffs2\_sum\_write\_data: Not enough space for summary, padsize = -549 | kernel: nf\_conntrack: expectation table full  
PS5: 因为很多东西会往jffs频繁写.所以会对NAND的寿命有一定的影响..比如syslog.现在用U盘替代.可以进一步提升路由器的稳定性.我用的是SONY的记忆棒~感觉还不错.~  
PS6: 可以放心开 Traffic Analyzer 流量分析 了 . 现在jffs随便用了.不会因为之前只有那48MB的JFFS而担心撑爆JFFS了.  
  
PS7: 关于重置了路由器后处理方法 , 先不要插上U盘 , 开启路由器的JFFS后让软件中心成功初始化 , 然后插上U盘并删除U盘里的/jffs/nvram/文件夹 , 接着按照上面的步骤重新安装即可  
  
PS8: 从低于384.19的固件版本升级到384.19的朋友 , 请在升级19后 , 格式化JFFS分区 , 然后把U盘上的 /jffs/scripts/ 文件夹上的除了 dnsmasq.postconf(没有则无视) 文件外的所有文件拷贝到机器的 /jffs/scripts/ 文件夹下 , 然后执行 chmod +x /jffs/scripts/\* 后重启即可~  
  
  
还原方法 : 将/tmp/mnt/sda1/jffs/文件夹删除.还有/tmp/mnt/sda1/.jffs\_sync/文件夹删除,重启后将/jffs/scripts/post-mount还原(第4步骤提醒备份的文件),然后执行命令chmod a+x /jffs/scripts/post-mount,再删除/jffs/scripts/unmount后重启即可  
  
![下载附件](https://www.koolshare.cn/forum.php?mod=attachment&aid=MzAwMzQwfDY2NTM0M2VjfDE2MzE5NTAxMzR8MjM4MHwxNjEwMTc%3D&nothumb=yes)

更新 2019-05-20 23:56:46 -> 修复unmount相关错误并在post-mount新增释放内存动作  
  
更新 2019-05-21 17:50:42 -> 完善post-mount启动方法 , 并新增USB 与 JFFS之间的同步  
  
更新 2019-05-23 00:04:14 -> 撤销在USB的nvram文件copy回jffs方法  
  
更新 2019-05-29 16:08:01 -> 新增指定挂载点逻辑 , 指定某一设备挂载jffs分区 , 需要清楚目标设备的挂载路径 , 多USB设备的福音  
  
更新 2019-06-21 15:44:40 ->  优化skipd启动顺序 , 让其他插件可以更兼容 (建议更新)  
  
更新 2019-06-21 17:46:41 -> 关闭原本wan跟net的start脚本 , 让其的启动顺序在post-mount之后  
  
更新 2020-03-23 15:00:33 -> 兼容384.15  
  

已知问题 , 在SSH下输入reboot命令重启会导致重启失败 , 需要手动断电后重启才恢复 , 正常重启不受影响(不清楚是否是ASUS固件的问题) , SSH下要用echo b > /proc/sysrq-trigger重启  
  
更新方法: 删除U盘下的jffs文件夹和.jffs\_sync文件夹后重启 , 然后再从第一步开始即可  
