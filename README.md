#### 什么是云计算：

云计算的历史最远可追溯到 1965 年，Christopher Strachey 发表了一篇论文，论文中正式提出了「虚拟化」的概念。而虚拟化正是云计算基础架构的核心，是云计算发展的基础。

在 2006 年 8 月 9 日，Google首席执行官埃里克·施密特（Eric Schmidt）在搜索引擎大会（SESSanJose2006）首次提出「云计算」（Cloud Computing）的概念。而亚马逊正是那年推出了 IaaS 服务平台 AWS。

但彼时的甲骨文掌门人 Larry Ellison 没少在社交软件上吐槽云：“这种白痴行为什么时候会停止？这不过是一时兴起的时尚潮流，是疯狂的事情。”而四年之后，这位“硅谷最老的花花公子”也不得不宣布向云战略进军了。

- 深圳IT领袖峰会
- 阿里云博士：王坚，坚持8年时间，2008年阿里云成立
- 全球三大云厂商：
  - 亚马逊AWS
  - 微软Azure
  - 阿里云，全国14地区建立200多个数据中心 

#### 云计算的类型

- 公有云：公有云是作为第三方云厂商所拥有和运营的，他们通过Internet提供计算资源，在公有云中，所		有的硬件、软件和其他一些基础性的结构均由云提供商拥有和运营。
- 私有云：私有云一般都是企业或者组织来使用的，可以位于企业数据中心之上，在私有云中，有专门的网络维护功能和基础结构。
- 混合云：即同时使用公有云和私有云。从而允许公司将敏感数据保留私有云中（安全性），同时使用公有云来运行应用程序（低成本）。

#### 云计算的服务模式

![saas-paas-iaas-01-1024x1024](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/saas-paas-iaas-01-1024x1024.png)

- IaaS（Infrastructure as a Service）：基础设施即服务
- PaaS（Platform as a Service ）：平台即服务
- SaaS（Software as a Service）：软件即服务

#### 虚拟化

- VMware虚拟机软件
- 企业级虚拟化：KVM虚拟化，在Linux系统管理虚拟机的

#### 常见服务器种类

- 塔式服务器
- 刀片服务器
- 机架式服务器

#### UNIX系统

<img src="https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/Snipaste_2023-05-01_13-29-12-20230501151203836.png" style='float:left;' />

- [UNIX](https://linuxhistory.hdert.com/)开源且免费理念；被收购，商业系统
- Unix 是一系列多任务、多用户计算机操作系统，源自最初的 AT&T Unix，由 **肯·汤普森 (Ken Thompson) 和丹尼斯·里奇 (Dennis Ritchie) ** 等人于1970 年代在贝尔实验室研究中心开始开发。
- 1973年由C语言之父 - 丹尼斯·里奇 (Dennis Ritchie) 用C语言重写了UNIX

#### Linux系统

<img src="https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/Snipaste_2023-05-01_13-30-51.png" style='float:left;'/>

- [Linux](https://linuxhistory.hdert.com/)开源且免费理念，免费使用，源代码可以自由传播，做二次开发，遵循GPL协议
- 1991年底，Linus Torvalds公开了linux内核源码0.02版；1993年，Linux1.0版发行
- GPL协议：GNU自由软件基金会（通用公共的许可协议，GPL），linus加入GNU组织，形成GNU/Linux（GNU的软件加上Linux的内核）

#### Linux发行版本

![2132px-Unix_history-simple.svg](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/2132px-Unix_history-simple.svg.png)

#### Linux基本概念

- 多用户的系统：允许同时有很多个用户登陆系统，使用系统资源
- 多任务的系统：允许同时执行多个任务
- 命令/选项/参数/文件名/目录名严格区分大小写
- 一切皆文件：硬件设备（内存、cpu、网卡、硬盘都是以文件形式存在的）
  - 不管是文件还是目录都是以倒挂的树形结构，存在于系统的/目录下，/（根）是Linux的起点

- 对于Linux系统而言，目录还是文件都是没有扩展名一说
  - .sh：脚本文件
  - .log：日志文件
  - .conf：配置文件
  - .rpm：软件包
  - .tar：压缩包

#### Linux系统分辨目录与文件的方法

- 蓝色表示目录
- 白色表示文件
- 浅蓝色表示链接文件
- 绿色表示可执行文件
- 红色表示压缩文件
- 黄色表示设备文件（硬盘、鼠标、cpu、网卡）
- 红色闪动文件表示链接文件不可用

#### 命令终端

- ～：表示用户的家目录，其他用户不能随便访问
- /root：root超级管理员的家目录
- /home/用户名：普通用户的家目录

#### 快捷键

- ctrl + l：清屏

- ctrl + u：清除当前命令

- ctrl + c:  取消当前命令

- tab：命令路径补全

- ctrl + a：光标移动行首

- ctrl + e：光标移动至行尾

- ctrl + w：删除一个单词

#### 命令一般格式

- 命令  [-选项...] [参数...]
  - 选项：
    - 短选项：-l -a -d -h（单个字符），可以合并使用：-la -df
    - 长选项：--help（单词），长选项通常是不能合并使用的
  - 参数：命令的执行对象，文件/目录/程序等
  - 可以同时有多个选项和参数

#### Linux系统文件类型

- -普通文件

- d 目录

- l 链接文件

- b 跨设备文件

- c 字符设备文件

- p 管道设备文件

- s 套接字

#### Linux系统归属关系

- u 所有者：文件或目录的拥有者，拥有者的权限通常最大
- g 所有组：文件或目录的属于哪一个组，所属组的权限略微比所有者小
- o 其他人：既不是文件所有者，也不属于文件或目录组内成员，其他人的权限通常最小的权限

#### ls命令

- ls命令（英文：list）：用于查看目录下内容及目录文件详细属性信息
- 命令格式：l s [-选项...] [-参数...]
- 常用选项
  - -a 显示目录下所有内容，包含隐藏的内容
  - -l 以长格式显示目录下的内容及详细属性
  - -h 以人性化显示目录下内容大小（KB、MB、GB）
  - -d 仅显示目录本身而不显示目录下的内容
  - -i 查看inode号
  - -R 递归查看目录下所有的内容

~~~shell
# 权限后面1、5、7代表文件引用次数，只针对与做了硬连接的文件才有效
[root@localhost /]# ls -l
总用量 20
lrwxrwxrwx.   1 root root    7 8月  12 2018 bin -> usr/bin			#l开头表示链接文件
dr-xr-xr-x.   5 root root 4096 4月  25 13:48 boot							#d开头表示目录
-rw-r--r--.   1 root root    0 4月  25 21:18 hello.txt					#-开头表示文件

#以人性化的显示占用空间
[root@localhost /]# ls -lh
总用量 20K
lrwxrwxrwx.   1 root root    7 8月  12 2018 bin -> usr/bin
dr-xr-xr-x.   5 root root 4.0K 4月  25 13:48 boot
drwxr-xr-x.  19 root root 3.1K 4月  25 21:06 dev
drwxr-xr-x.  79 root root 8.0K 4月  25 21:06 etc

#查看当前目录下所有文件包括隐藏文件
[root@localhost /]# ll -a
总用量 20
dr-xr-xr-x.  17 root root  241 4月  25 21:18 .
dr-xr-xr-x.  17 root root  241 4月  25 21:18 ..
lrwxrwxrwx.   1 root root    7 8月  12 2018 bin -> usr/bin
dr-xr-xr-x.   5 root root 4096 4月  25 13:48 boot
drwxr-xr-x.  19 root root 3080 4月  25 21:06 dev
drwxr-xr-x.  79 root root 8192 4月  25 21:06 etc
-rw-r--r--.   1 root root    0 4月  25 21:18 hello.txt

#查看文件inode号
[root@localhost /]# ll -i
总用量 20
     735 lrwxrwxrwx.   1 root root    7 8月  12 2018 bin -> usr/bin
     128 dr-xr-xr-x.   5 root root 4096 4月  25 13:48 boot
       3 drwxr-xr-x.  19 root root 3080 4月  25 21:06 dev
16777345 drwxr-xr-x.  79 root root 8192 4月  25 21:06 etc
  252494 -rw-r--r--.   1 root root    0 4月  25 21:18 hello.txt
     161 drwxr-xr-x.   2 root root    6 8月  12 2018 home
     739 lrwxrwxrwx.   1 root root    7 8月  12 2018 lib -> usr/lib 

#查看当前目录的详细信息
[root@localhost dev]# ll -d
drwxr-xr-x. 19 root root 3080 4月  25 21:06  
~~~

<img src="https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/list_content.webp" style="zoom:150%;" />

**r w - r-- r-- :所有者、所属组、其他人**

 **u     g   o**

~~~~shell
[root@localhost /]# ll
总用量 20
lrwxrwxrwx.   1 root root    7 8月  12 2018 bin -> usr/bin
dr-xr-xr-x.   5 root root 4096 4月  25 13:48 boot
drwxr-xr-x.  19 root root 3080 4月  25 21:06 dev
drwxr-xr-x.  79 root root 8192 4月  25 21:06 etc
-rw-r--r--.   1 root root    0 4月  25 21:18 hello.txt
drwxr-xr-x.   2 root root    6 8月  12 2018 home
lrwxrwxrwx.   1 root root    7 8月  12 2018 lib -> usr/lib
~~~~

#### stat命令

- stat [option] ... file
- 常用选项
  - -f

~~~shell
[root@localhost /]# stat hello.txt 
  文件：hello.txt
  大小：0               块：0          IO 块：4096   普通空文件
设备：fd00h/64768d      Inode：252494      硬链接：1
权限：(0644/-rw-r--r--)  Uid：(    0/    root)   Gid：(    0/    root)
环境：unconfined_u:object_r:etc_runtime_t:s0
最近访问：2023-04-25 21:18:35.894161871 +0800
最近更改：2023-04-25 21:18:35.894161871 +0800
最近改动：2023-04-25 21:18:35.894161871 +0800
创建时间：-

[root@localhost /]# stat -f hello.txt 
  文件："hello.txt"
    ID：fd0000000000 文件名长度：255     类型：xfs
块大小：4096       基本块大小：4096
    块：总计：4452864    空闲：4066561    可用：4066561
Inodes: 总计：8910848    空闲：8875802
~~~

#### mkdir命令

- mkdir (make directory) 用于创建新的目录
- 命令格式：mkdir [-选项] 目录名
- 常用选项：
  - -p递归创建多个目录
- 注意事项：
  - 目录还是名字，除了以 "/" 以外的任意名称
  - 文件或目录的名字长度不能超过255个字符

```shell
# 创建study目录
[root@localhost ~]# mkdir study
[root@localhost ~]# ls
anaconda-ks.cfg  study
# 递归创建study/test1/t1目录
[root@localhost ~]# mkdir -p study/test1/t1
[root@localhost ~]# ls
anaconda-ks.cfg  study
[root@localhost ~]# ll -R study
study:
总用量 0
drwxr-xr-x. 3 root root 16 4月  27 00:21 test1

study/test1:
总用量 0
drwxr-xr-x. 2 root root 6 4月  27 00:21 t1

study/test1/t1:
总用量 0
```

#### cd命令

- cd（change directory）切换目录
- 命令格式：cd [-选项] [目录名]
- 常用快捷操作
  - ～表示家目录
  - .表示当前目录
  - ..表示上一级目录
  - -可在两路径之间来回切换
- 绝对路径：以/为起点，到达目标目录；/etc/yum
- 相对路径：以当前目录为起点，到达目标目录；yum/test/

```shell
# 相对路径进入到study/test1
[root@localhost ~]# cd study/test1
[root@localhost test1]# pwd
/root/study/test1
# 回到上一级目录
[root@localhost test1]# cd ..
# 回到家目录
[root@localhost study]# cd
# 绝对路径进入/root/study/test1目录
[root@localhost ~]# cd /root/study/test1
[root@localhost test1]# cd /root/study/test2
# -两路径之间切换
[root@localhost test2]# cd -
/root/study/test1
```

#### pwd命令

- pwd（print work directory）打印当前所在的绝对目录
- 命令格式：pwd [-选项]

#### rmdir命令

- rmdir（remove directory）删除空目录，只能一层一层删除目录
- 命令格式：rmdir [-选项] 目录名

```shell
# 删除目录
[root@localhost test1]# rmdir t1
# 只能一层一层删除目录
[root@localhost ~]# rmdir study/
rmdir: 删除 'study/' 失败: 目录非空
```

#### touch命令

- touch命令用于创建新的空白文件，有同名文件不会覆盖
- 命令格式：touch [-选项] 文件名

```shell
# 创建hello.py文件
[root@localhost ~]# touch hello.py
[root@localhost ~]# ls
anaconda-ks.cfg  hello.py  study
```

#### cp命令

- cp（copy file）用于复制文件或目录，cp命令在复制时也可以修改文件或目录的名字
- 命令格式：cp [-选项] 原文件或目标 目标目录
- 常用选项：
  - -p 保留原文件属性不变（修改时间、归属关系、权限）
  - -r 复制目录（包含该目录下所有子目录和文件）
- cp test /tmp/oo
- cp test/tmp/oo

```shell
# 将hello.py重命名复制到study/test1/下
[root@localhost ~]# cp hello.py study/test1/hello1.py
# 将hello.py保留原文件属性重命名复制到study/test1/下
[root@localhost ~]# cp -p hello.py study/test1/hello2.py
[root@localhost ~]# ll study/test1/
总用量 0
-rw-r--r--. 1 root root 0 4月  27 00:28 hello1.py
-rw-r--r--. 1 root root 0 4月  27 00:27 hello2.py

# 将study目录在复制到/root/study2/下重命名oo
[root@localhost ~]# cp -r study /root/study2/oo
[root@localhost ~]# ls /root/study2/oo
test1
# 将study目录复制到/root/study2/oo下
[root@localhost ~]# cp -r study /root/study2/oo
[root@localhost ~]# ls /root/study2/oo
study  test1
```

#### mv命令

- mv（move file）移动文件或目录到其他位置，也可以修改文件或目录用户名
- 命令格式：mv [-选项] 源文件.... 目标路径

```shell
# 将study整个目录移动重命名到/root/study3/下
[root@localhost ~]# mv study /root/study3/study_t
[root@localhost ~]# ll study3/
总用量 0
drwxr-xr-x. 3 root root 19 4月  27 00:21 study_t
[root@localhost ~]# ls
anaconda-ks.cfg  hello.py  study3
```

#### cat命令

- cat（concatenate）用于查看文本文件内容
- 命令格式：cat [- 选项] 文件名
- 常用选项
  - -n 查看文件时以行号的形式显示文件内容

```shell
[root@localhost ~]# cat -n /etc/passwd
     1  root:x:0:0:root:/root:/bin/bash
     2  bin:x:1:1:bin:/bin:/sbin/nologin
     3  daemon:x:2:2:daemon:/sbin:/sbin/nologin
     4  adm:x:3:4:adm:/var/adm:/sbin/nologin
     5  lp:x:4:7:lp:/var/spool/lpd:/sbin/nologin
     6  sync:x:5:0:sync:/sbin:/bin/sync
     7  shutdown:x:6:0:shutdown:/sbin:/sbin/shutdown
     8  halt:x:7:0:halt:/sbin:/sbin/halt
     9  mail:x:8:12:mail:/var/spool/mail:/sbin/nologin
    10  operator:x:11:0:operator:/root:/sbin/nologin
    11  games:x:12:100:games:/usr/games:/sbin/nologin
    12  ftp:x:14:50:FTP User:/var/ftp:/sbin/nologin
    13  nobody:x:65534:65534:Kernel Overflow User:/:/sbin/nologin
    14  dbus:x:81:81:System message bus:/:/sbin/nologin
    15  systemd-coredump:x:999:997:systemd Core Dumper:/:/sbin/nologin
    16  systemd-resolve:x:193:193:systemd Resolver:/:/sbin/nologin
    17  tss:x:59:59:Account used by the trousers package to sandbox the tcsd daemon:/dev/null:/sbin/nologin
    18  polkitd:x:998:996:User for polkitd:/:/sbin/nologin
    19  unbound:x:997:995:Unbound DNS resolver:/etc/unbound:/sbin/nologin
    20  sssd:x:996:993:User for sssd:/:/sbin/nologin
    21  sshd:x:74:74:Privilege-separated SSH:/var/empty/sshd:/sbin/nologin
```

#### less命令

- less命令是对文件的输出进行分页显示的工具，常用于查看内容量较大的文件
- 命令格式：less [-选项] 文件
- 常用选项：
  - -N 以行号显示文件内容
- 使用方法：
  - 键盘上下键逐行查看
  - pgdn：向下翻一页
  - pdup：向上翻一页
  - /字符串：搜索指定字符串
    - n：从上向下搜索
    - N：从下向上搜索
  - G：直接跳转到文件最后一行
  - gg：直接跳转到文件行首
  - q：退出 

#### head与tail命令

- head：用于显示文件开头部分内容，默认显示文件开头10行内容
  - 命令格式：head [- 选项] 参数
  - 常用选项：
    - -n<行数>指定显示的行数
- tail：用来显示文件末尾部分内容，默认显示文件末尾10行内容
  - 命令格式：tail [- 选项] 参数
  - 常用选项：
    - -n<行数>指定显示的行数 
    - -f动态显示

```shell
[root@localhost ~]# head  /etc/services 
# /etc/services:
# $Id: services,v 1.49 2017/08/18 12:43:23 ovasik Exp $
#
# Network services, Internet style
# IANA services version: last updated 2016-07-08
#
# Note that it is presently the policy of IANA to assign a single well-known
# port number for both TCP and UDP; hence, most entries here have two entries
# even if the protocol doesn't support UDP operations.
# Updated from RFC 1700, ``Assigned Numbers'' (October 1994).  Not all ports
[root@localhost ~]# head -4 /etc/services 
# /etc/services:
# $Id: services,v 1.49 2017/08/18 12:43:23 ovasik Exp $
#
# Network services, Internet style
[root@localhost ~]# tail /etc/services 
aigairserver    21221/tcp               # Services for Air Server
ka-kdp          31016/udp               # Kollective Agent Kollective Delivery
ka-sddp         31016/tcp               # Kollective Agent Secure Distributed Delivery
edi_service     34567/udp               # dhanalakshmi.org EDI Service
axio-disc       35100/tcp               # Axiomatic discovery protocol
axio-disc       35100/udp               # Axiomatic discovery protocol
pmwebapi        44323/tcp               # Performance Co-Pilot client HTTP API
cloudcheck-ping 45514/udp               # ASSIA CloudCheck WiFi Management keepalive
cloudcheck      45514/tcp               # ASSIA CloudCheck WiFi Management System
spremotetablet  46998/tcp               # Capture handwritten signatures
[root@localhost ~]# tail -5 /etc/services 
axio-disc       35100/udp               # Axiomatic discovery protocol
pmwebapi        44323/tcp               # Performance Co-Pilot client HTTP API
cloudcheck-ping 45514/udp               # ASSIA CloudCheck WiFi Management keepalive
cloudcheck      45514/tcp               # ASSIA CloudCheck WiFi Management System
spremotetablet  46998/tcp               # Capture handwritten signatures
[root@localhost ~]# tail -f hello.py 
helloworldls!
你好，世界！
```

#### rm命令

- rm（remove）用于删除文件或目录
- 命令格式：rm [- 选项...] 文件或目录...
- 常用选项：
  - -f 强制删除，不提示
  - -r 删除目录
  - *特殊字符：通配符，表示任意字符

```shell
[root@localhost ~]# rm hello.py 
rm：是否删除普通文件 'hello.py'？y
[root@localhost ~]# rm -r study3/
rm：是否进入目录'study3/'? y
rm：是否进入目录'study3/study_t'? y
rm：是否进入目录'study3/study_t/test1'? y
rm：是否删除普通空文件 'study3/study_t/test1/hello1.py'？y
rm：是否删除普通空文件 'study3/study_t/test1/hello2.py'？y
rm：是否删除目录 'study3/study_t/test1'？y
rm：是否删除目录 'study3/study_t'？y
rm：是否删除目录 'study3/'？y
[root@localhost ~]# ls
anaconda-ks.cfg
[root@localhost ~]# rm -rf study
[root@localhost ~]# ls
anaconda-ks.cfg
[root@localhost ~]# ls
anaconda-ks.cfg  t1  t2  t24  t4  ttst3
[root@localhost ~]# rm -rf t*
[root@localhost ~]# ls
anaconda-ks.cfg
```

#### 软连接和硬连接

- Linux中的连接文件类似于Windows的快捷方式
- 注意：创建链接时一定要写目录或文件的绝对路径，哪怕是在当前路径下，也要写绝对路径；使用链接文件可以实现同步更新
- 软连接
  - 特点：软连接可以跨分区，可以对目录进行链接，原文件删除后，链接文件不可用；软链接文件权限取决于原文件权限
  - 软连接命令格式：ln -s 原文件路径 目标路径
- 硬连接
  - 特点：硬连接不可跨分区，不可以对目录进行连接，原文件删除后，链接依旧可用；硬链接文件属性保持不变（inode、最近修改时间）
  - 硬连接命令格式：ln 原文件路径 目标路径
- 删除链接：在删除链接目录，使用rm -rf末尾不能加“/”，否则会删除原文件
  - unlink 链接文件名
  - rm 链接文件名
  - rm -f 链接文件名
  - rm -rf 链接目录

```shell
[root@localhost ~]# ll
总用量 8
-rw-------. 1 root root 1191 4月  25 13:47 anaconda-ks.cfg
-rw-r--r--. 1 root root    6 4月  27 14:50 hello.py
drwxr-xr-x. 2 root root    6 4月  27 14:49 study
# 创建软链接
[root@localhost ~]# ln -s /root/hello.py /root/study/
[root@localhost ~]# ll /root/study/
总用量 0
# 软链接文件权限取决于原文件权限
lrwxrwxrwx. 1 root root 14 4月  27 14:50 hello.py -> /root/hello.py
[root@localhost ~]# echo 你好世界！> hello.py 
[root@localhost ~]# cat /root/study/hello.py 
你好世界！
[root@localhost ~]# cat hello.py 
你好世界！
# 创建硬链接，文件属性保持不变
[root@localhost ~]# ln /root/hello.py /root/study/
[root@localhost ~]# ll study/
总用量 4
-rw-r--r--. 2 root root 27 4月  27 14:54 hello.py
[root@localhost ~]# echo hello >> hello.py 
[root@localhost ~]# cat study/hello.py
helloworld
你好世界！
hello
# 硬链接原文件删除后，链接依旧可用
[root@localhost ~]# rm -rf hello.py 
[root@localhost ~]# cat /root/study/hello.py 
helloworld
你好世界！
hello

# 创建软链接目录
[root@localhost ~]# ln -s /root/study/ /root/test/
[root@localhost ~]# ll test
总用量 0
lrwxrwxrwx. 1 root root 12 4月  27 15:59 study -> /root/study/
# 删除软链接目录
[root@localhost ~]# rm -rf test/study
[root@localhost ~]# ll
总用量 4
-rw-------. 1 root root 1191 4月  25 13:47 anaconda-ks.cfg
drwxr-xr-x. 2 root root   22 4月  27 15:48 study
drwxr-xr-x. 2 root root    6 4月  27 15:59 test
```

#### fdisk命令

- Linux fdisk 是一个创建和维护分区表的程序，它兼容 DOS 类型的分区表、BSD 或者 SUN 类型的磁盘列表

- 命令格式：fdisk [- 必要参数] [选择参数]

  - 必要参数：
    - -l 列出素所有分区表
    - -u 与 **-l** 搭配使用，显示分区数目

  - 选择参数：

    - -s<分区编号> 指定分区

    - -v 版本信息

  - 菜单操作说明

    - m ：显示菜单和帮助信息

    - a ：活动分区标记/引导分区

    - d ：删除分区

    - l ：显示分区类型

    - n ：新建分区

    - p ：显示分区信息

    - q ：退出不保存

    - t ：设置分区号

    - v ：进行分区检查

    - w ：保存修改

    - x ：扩展应用，高级功能

```shell
[root@localhost ~]# fdisk -l
Disk /dev/nvme0n1：20 GiB，21474836480 字节，41943040 个扇区
单元：扇区 / 1 * 512 = 512 字节
扇区大小(逻辑/物理)：512 字节 / 512 字节
I/O 大小(最小/最佳)：512 字节 / 512 字节
磁盘标签类型：dos
磁盘标识符：0x5d403be6

设备           启动    起点     末尾     扇区 大小 Id 类型
/dev/nvme0n1p1 *       2048  2099199  2097152   1G 83 Linux
/dev/nvme0n1p2      2099200 41943039 39843840  19G 8e Linux LVM


Disk /dev/mapper/rhel-root：17 GiB，18249416704 字节，35643392 个扇区
单元：扇区 / 1 * 512 = 512 字节
扇区大小(逻辑/物理)：512 字节 / 512 字节
I/O 大小(最小/最佳)：512 字节 / 512 字节


Disk /dev/mapper/rhel-swap：2 GiB，2147483648 字节，4194304 个扇区
单元：扇区 / 1 * 512 = 512 字节
扇区大小(逻辑/物理)：512 字节 / 512 字节
I/O 大小(最小/最佳)：512 字节 / 512 字节

```

#### 内部命令与外部命令

- 什么是命令：用来实现某一种功能的指令和程序
- 命令的执行依赖于解释器（例如：/bin/bash）；**/etc/shells**文件存放系统可以用的shell
  - 用户 <--> 解释器（shell） <--> 内核
- Linux命令的分类
  - 内部命令：shell程序自带的基本管理命令
  - 外部命令：有独立的外部可执行程序文件命令
  - type用于区别内部命令与外部命令
  - which用于查找可执行程序文件位置

```shell
[root@localhost ~]# cat /etc/shells 
/bin/sh
/bin/bash
/usr/bin/sh
/usr/bin/bash
[root@localhost ~]# which ls
alias ls='ls --color=auto'
        /usr/bin/ls
```

#### hash命令

在Linux系统存在一个hash表，系统初始时hash表为空，当外部命令执行时，默认会从PATH路径下寻找该命令，找到后会将这条命令的路径记录到hash表中，当再次使用该命令时，shell解释器首先会查看hash表，存在将执行，如果不存在，将会去**PATH**路径下寻找，利用hash缓存表可大大提高命令的调用速率。

- hash命令是bash的内置命令，用于显示hash缓存

- 命令格式：hash [-选项]
  -  –l：显示hash缓存，加参数-l既可以看到hash表命令的路径，也可以看到它的名字或别名
  - –p：path name 将命令全路径path起别名为name
  - –t：name 显示指定命令的完整路径
  - –d：name 清除name缓存
  - –r：清除缓存

```shell
[root@localhost ~]# echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/root/bin
[root@localhost ~]# hash
命中    命令
   2    /usr/bin/cat
   3    /usr/bin/ls
[root@localhost ~]# hash -r
[root@localhost ~]# hash
hash: 哈希表为空
```

#### help命令帮助手册

- help命令用于查看**shell**内部命令的相关信息，包括使用方法、选项等...
- 命令格式：help [-选项] 命令
- 常用选项：
  - -d 输出每个主题的简短描述
  - -m 以伪man手册的格式显示使用方法
  - -s 为每一个匹配PATTERN模式的主题仅显示一个用法

```shell
[root@localhost ~]# help cd
cd: cd [-L|[-P [-e]] [-@]] [目录]
    改变 shell 工作目录。
    
    改变当前目录至 DIR 目录。默认的 DIR 目录是 shell 变量 HOME
    的值。
    
    变量 CDPATH 定义了含有 DIR 的目录的搜索路径，其中不同的目录名称由冒号 (:)分隔。
    一个空的目录名称表示当前目录。如果要切换到的 DIR 由斜杠 (/) 开头，则 CDPATH
    变量不会被使用。
    
    如果路径找不到，并且 shell 选项 `cdable_vars' 被设定，则参数词被假定为一个
    变量名。如果该变量有值，则它的值被当作 DIR 目录。
    
    选项：
        -L      强制跟随符号链接: 在处理 `..' 之后解析 DIR 中的符号链接。
        -P      使用物理目录结构而不跟随符号链接: 在处理 `..' 之前解析 DIR 中的符号链接。
        -e      如果使用了 -P 参数，但不能成功确定当前工作目录时，返回非零的返回值。
        -@      在支持拓展属性的系统上，将一个有这些属性的文件当作有文件属性的目录。
    
    默认情况下跟随符号链接，如同指定 `-L'。
    `..' 使用移除向前相邻目录名成员直到 DIR 开始或一个斜杠的方式处理。
    
    退出状态：
    如果目录改变，或在使用 -P 选项时 $PWD 修改成功时返回 0，否则非零。
[root@localhost ~]# cat --help
用法：cat [选项]... [文件]...
连接所有指定文件并将结果写到标准输出。

如果没有指定文件，或者文件为"-"，则从标准输入读取。

  -A, --show-all           equivalent to -vET
  -b, --number-nonblank    number nonempty output lines, overrides -n
  -e                       equivalent to -vE
  -E, --show-ends          display $ at end of each line
  -n, --number             number all output lines
  -s, --squeeze-blank      suppress repeated empty output lines
  -t                       与-vT 等价
  -T, --show-tabs          将跳格字符显示为^I
  -u                       (被忽略)
  -v, --show-nonprinting   使用^ 和M- 引用，除了LFD和 TAB 之外
      --help            显示此帮助信息并退出
      --version         显示版本信息并退出

示例：
  cat f - g  先输出f 的内容，然后输出标准输入的内容，最后输出g 的内容。
  cat        将标准输入的内容复制到标准输出。

GNU coreutils 在线帮助：<https://www.gnu.org/software/coreutils/>
请向 <http://translationproject.org/team/zh_CN.html> 报告 cat 的翻译错误
完整文档请见：<https://www.gnu.org/software/coreutils/cat>
或者在本地使用：info '(coreutils) cat invocation'
```

#### man获取命令帮助手册

- man命令用于查看系统命令的帮助信息，包括使用方法、选项、列子...，对比help，man的输出信息更加详细
- 命令格式：man [- 选项] 命令
- 常用快捷操作
  - 键盘下键向下移一行
  - 键盘上键向上移一行
  - PgUp 向上翻一页
  - PgDown 向下翻一页
  - /关键字 搜索关键字
    - n：向下查询
    - N：向上查询
  - q 退出

#### info获取命令的帮助信息

- 命令格式：info [- 选项] 命令
- 按键操作：
  - 空格键：向下翻一页
  - n：跳到下一个节点
  - p：跳到上一个节点
  - u：回到上一层节点
  - 回车键：光标移动到下一层节点处，以回车进入
  - b：跳到当前info page的第一个节点处
  - e：跳到当前info page的最后一个节点处
  - /：在info page种就行搜索
  - q：退出info page

#### Linux系统的运行级别

Linux系统有7种运行级别，不同的运行级别运行的程序和功能都不一样，而Linux系统默认是运行在一个标准的级别上，**系统运行级别文件/etc/inittab**文件

- 0：所有进程被终止，及其将有序的停止，关机时系统处于这个运行级别
- 1：单用户模式，（root用户进行系统维护），系统里运行的所有服务也都不会启动
- 2：多用户模式（网络文件系统NFS服务没有被启动）
- 3：完全多用户模式，（NFS网络文件系统）标准的运行级别
- 4：保留模式，系统未使用
- 5：登录后，进入带GUI的图形界面，标准的运行级别
- 6：系统正常关闭并重启

```shell
# 查看当前处于级别；N表示从那个级别切换过来的，3表示当前处于级别
[root@localhost ~]# runlevel
N 3
[root@localhost ~]# cat /etc/inittab 
# inittab is no longer used.
#
# ADDING CONFIGURATION HERE WILL HAVE NO EFFECT ON YOUR SYSTEM.
#
# Ctrl-Alt-Delete is handled by /usr/lib/systemd/system/ctrl-alt-del.target
#
# systemd uses 'targets' instead of runlevels. By default, there are two main targets:
#
# multi-user.target: analogous to runlevel 3
# graphical.target: analogous to runlevel 5
#
# To view current default target, run:
# systemctl get-default
#
# To set a default target, run:
# systemctl set-default TARGET.target
[root@localhost ~]# systemctl get-default		# 查看系统默认级别
multi-user.target
```

#### 关机与重启

- Linux下常用的关机命令有
  - init 0 立刻关机
  - halt 立刻关机
  - poweroff 立刻关机
  - shutdown -h now 立刻关机
  - shutdown -h 10  10分钟后自动关机
- 重启
  - reboot 立刻重启
  - shutdown -r now 立刻重启
  - shutdown -r 10 10分钟后重启

#### Linux系统目录介绍

<img src="https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/linux_file_structure.webp" />

- /（根）：系统所有数据都存放在根目录下
- /bin：存放用户和管理员必备的可执行的二进制程序文件
- /boot：存放Linux系统内核及引导系统程序所需要的文件目录
- /dev：存放硬件设备的目录，如键盘、鼠标、硬盘、光盘等
- /etc：存放服务的配置文件，用户信息文件
- /root：超级管理员的家目录
- /home：系统普通用户的家目录
- /lib：存放系统中的程序运行所需要的共享库及内核模块
- /opt：额外安装的可选应用程序包所放置的位置
- /srv：服务启动之后需要访问的数据目录
- /tmp：一般用户或正在执行的程序临时存放文件的目录，任何人都可以访问，重要数据不可放置在此目录下
- /var：存放系统执行过程中经常变化的文件，如随时都在变化的日志文件就存放在/var/log/下
- /mnt、/media：光盘和镜像等预设的挂载点
- /proc：Linux伪文件系统，该目录下的数据存在于内存当中，不占用磁盘空间
- /lib64:存放函式库
- /run：程序或服务启动后，存放PID的目录
- /sys：存放被建立在内存中的虚拟文件系统
- /usr：操作系统软件资源所放置的目录
  - /usr/bin：与/bin目录相同，存放用户可以使用的命令程序
  - /usr/lib：与/lib目录相同，存放系统中的程序运行所需要的共享库及内核模块
  - /usr/etc：用于存放安装软件时使用的配置文件
  - /usr/games：与游戏比较相关的数据放置处
  - /usr/include：c/c++等程序语言的档头（header）与包含档（include）放置处
  - /usr/lib64：与/lib64目录相同，存放函式库
  - /usr/libexec：不经常被使用的执行程序或脚本会放置在此目录中
  - /usr/local：额外安装的软件存放目录
  - /usr/sbin：该目录与/sbin目录相同，存放用户可执行的二进制程序文件
  - /usr/share：放置只读架构的杂项数据文件
  - /usr/src：一般软件源代码建议存放该目录下

#### 查看内核信息

- uname命令用于显示系统内核信息
- 命令格式：uname [-选项...]
- 常用选项：
  - -s：显示内核名称
  - -r：显示内核版本

#### 查看CPU信息

- /proc/cpuinfo文件用于存放系统CPU信息
- lscpu用于显示CPU架构信息
- 命令格式：lscpu [-选项]

```shell
[root@canvs ~]# cat /proc/cpuinfo
processor       : 0
vendor_id       : GenuineIntel
cpu family      : 6
model           : 165
model name      : Intel(R) Core(TM) i5-10400 CPU @ 2.90GHz
stepping        : 3
microcode       : 0xe0
cpu MHz         : 2904.000
cache size      : 12288 KB
physical id     : 0
siblings        : 1
core id         : 0
cpu cores       : 1
apicid          : 0
initial apicid  : 0
fpu             : yes
fpu_exception   : yes
cpuid level     : 22
wp              : yes
flags           : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon nopl xtopology tsc_reliable nonstop_tsc cpuid pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single ssbd ibrs ibpb stibp ibrs_enhanced fsgsbase tsc_adjust bmi1 avx2 smep bmi2 invpcid rdseed adx smap clflushopt xsaveopt xsavec xgetbv1 xsaves arat flush_l1d arch_capabilities
bugs            : spectre_v1 spectre_v2 spec_store_bypass
bogomips        : 5808.00
clflush size    : 64
cache_alignment : 64
address sizes   : 45 bits physical, 48 bits virtual
power management:
# processor　：系统中逻辑处理核心数的编号，从0开始排序。
# vendor_id　：CPU制造商
# cpu family　：CPU产品系列代号
# model　　　：CPU属于其系列中的哪一代的代号
# model name：CPU属于的名字及其编号、标称主频
# stepping　 ：CPU属于制作更新版本
# cpu MHz　 ：CPU的实际使用主频
# cache size ：CPU二级缓存大小
# physical id ：单个物理CPU的标号
# siblings ：单个物理CPU的逻辑CPU数。siblings=cpu cores [*2]。
# core id ：当前物理核在其所处CPU中的编号，这个编号不一定连续。
# cpu cores ：该逻辑核所处CPU的物理核数。比如此处cpu cores 是4个，那么对应core id 可能是 1、3、4、5。
# apicid ：用来区分不同逻辑核的编号，系统中每个逻辑核的此编号必然不同，此编号不一定连续
# fpu ：是否具有浮点运算单元（Floating Point Unit）
# fpu_exception ：是否支持浮点计算异常
# cpuid level ：执行cpuid指令前，eax寄存器中的值，根据不同的值cpuid指令会返回不同的内容
# wp ：表明当前CPU是否在内核态支持对用户空间的写保护（Write Protection）
# flags ：当前CPU支持的功能
# bogomips：在系统内核启动时粗略测算的CPU速度（Million Instructions Per Second
# clflush size ：每次刷新缓存的大小单位
# cache_alignment ：缓存地址对齐单位
# address sizes ：可访问地址空间位数
# power management ：对能源管理的支持
```

#### 查看系统内存信息

- /proc/meminfo文件用于存放系统内存信息
- free用于查看内存使用情况
- 命令格式：free [-选项]
- 常用选项：-h。以KB、MB、GB方式显示大小

```shell
/ $ cat /proc/meminfo
MemTotal:         877368 kB  ：所有可用RAM大小（即物理内存减去一些预留位和内核的二进制代码大小）（HighTotal + LowTotal）,系统从加电开始到引导完成，BIOS等要保留一些内存，内核要保留一些内存，最后剩下可供系统支配的内存就是MemTotal。这个值在系统运行期间一般是固定不变的。
MemFree:           22516 kB  ：LowFree与HighFree的总和，被系统留着未使用的内存,MemFree是说的系统层面
MemAvailable:     470244 kB  ：应用程序可用内存数。系统中有些内存虽然已被使用但是可以回收的，比如cache/buffer、slab都有一部分可以回收，所以MemFree不能代表全部可用的内存，这部分可回收的内存加上MemFree才是系统可用的内存，即：MemAvailable≈MemFree+Buffers+Cached，它是内核使用特定的算法计算出来的，是一个估计,MemAvailable是说的应用程序层面
Buffers:            1772 kB  ：用来给文件做缓冲大小
Cached:           459224 kB  ：被高速缓冲存储器（cache memory）用的内存的大小（等于 diskcache minus SwapCache ）
SwapCached:           16 kB  ：被高速缓冲存储器（cache memory）用的交换空间的大小，已经被交换出来的内存，但仍然被存放在swapfile中。用来在需要的时候很快的被替换而不需要再次打开I/O端口
Active:           333148 kB  ：在活跃使用中的缓冲或高速缓冲存储器页面文件的大小，除非非常必要否则不会被移作他用. (Active(anon) + Active(file))
Inactive:         330384 kB  ：在不经常使用中的缓冲或高速缓冲存储器页面文件的大小，可能被用于其他途径. (Inactive(anon) + Inactive(file))
Active(anon):     104368 kB  ：活跃的与文件无关的内存（比如进程的堆栈，用malloc申请的内存）(anonymous pages),anonymous pages在发生换页时，是对交换区进行读/写操作
Inactive(anon):   104508 kB  ：非活跃的与文件无关的内存（比如进程的堆栈，用malloc申请的内存）
Active(file):     228780 kB  ：活跃的与文件关联的内存（比如程序文件、数据文件所对应的内存页）(file-backed pages) File-backed pages在发生换页(page-in或page-out)时，是从它对应的文件读入或写出
Inactive(file):   225876 kB  ：非活跃的与文件关联的内存（比如程序文件、数据文件所对应的内存页）
Unevictable:        6708 kB  ：
Mlocked:            1428 kB  ：
HighTotal:        261888 kB  ：高位内存总大小（Highmem是指所有内存高于860MB的物理内存,Highmem区域供用户程序使用，或用于页面缓存。该区域不是直接映射到内核空间。内核必须使用不同的手法使用该段内存）
HighFree:           5680 kB  ：未被使用的高位内存大小
LowTotal:         615480 kB  ：低位内存总大小,低位可以达到高位内存一样的作用，而且它还能够被内核用来记录一些自己的数据结构
LowFree:           16836 kB  ：未被使用的低位大小
SwapTotal:        614396 kB  ：交换空间的总大小
SwapFree:         611044 kB  ：未被使用交换空间的大小
Dirty:                40 kB  ：等待被写回到磁盘的内存大小
Writeback:             0 kB  ：正在被写回到磁盘的内存大小
AnonPages:        209224 kB  ：未映射页的内存大小
Mapped:           280668 kB  ：设备和文件等映射的大小
Shmem:              1084 kB  ：
Slab:              59840 kB  ：内核数据结构缓存的大小，可以减少申请和释放内存带来的消耗
SReclaimable:      34196 kB  ：可收回Slab的大小
SUnreclaim:        25644 kB  ：不可收回Slab的大小（SUnreclaim+SReclaimable＝Slab）
KernelStack:        7504 kB  ：常驻内存,每一个用户线程都会分配一个kernel stack(内核栈)
PageTables:        15508 kB  ：管理内存分页页面的索引表的大小
NFS_Unstable:          0 kB  ：不稳定页表的大小
Bounce:                0 kB  ：
WritebackTmp:          0 kB  ：
CommitLimit:     1053080 kB  ：根据超额分配比率（'vm.overcommit_ratio'），这是当前在系统上分配可用的内存总量，这个限制只是在模式2('vm.overcommit_memory')时启用。CommitLimit用以下公式计算：CommitLimit =（'vm.overcommit_ratio'*物理内存）+交换例如，在具有1G物理RAM和7G swap的系统上，当`vm.overcommit_ratio` = 30时 CommitLimit =7.3G
Committed_AS:   16368536 kB  ：目前在系统上分配的内存量。是所有进程申请的内存的总和，即时所有申请的内存没有被完全使用，例如一个进程申请了1G内存，仅仅使用了300M，但是这1G内存的申请已经被 "committed"给了VM虚拟机，进程可以在任何时间使用。如果限制在模式2('vm.overcommit_memory')时启用，分配超出CommitLimit内存将不被允许
VmallocTotal:     245760 kB  ：可以vmalloc虚拟内存大小
VmallocUsed:           0 kB  ：vmalloc已使用的虚拟内存大小
VmallocChunk:          0 kB  ：最大的连续未被使用的vmalloc区域
```

```shell
[root@canvs ~]# free -h
              total        used        free      shared  buff/cache   available
Mem:          1.8Gi       239Mi       1.3Gi       8.0Mi       251Mi       1.4Gi
Swap:         2.0Gi          0B       2.0Gi
#Mem 物理内存统计信息
total：				物理内存总量
used：					已使用的内存总量
free：					空闲内存总量
shared：				共享内存总量
buff/cache：		块设备与普通文件占用的缓存数量
available：		还可以被应用程序使用的物理内存大小
#Swap 内存交换空间，当物理内存不足时，可以使用硬盘空间充当内存使用
total：				交换分区内存总量
used：					正在使用的交换分区内存
free：					空闲交换分区内存
```



#### 查看网卡信息

- 网卡配置文件：/etc/sysconfig/network-scripts/ifcfg-ens160
- ifconfig用于显示和设置网卡的参数
- 命令格式：ifconfig [网卡名]

```shell
[root@localhost ~]# cat /etc/sysconfig/network-scripts/ifcfg-ens160 
TYPE="Ethernet"							#网卡类型=以太网
PROXY_METHOD="none"					#代理方式=关闭
BROWSER_ONLY="no"						#只是浏览器=否
BOOTPROTO="none"						#获取ip地址的方式=none固定ip，DHCP自动获取ip
DEFROUTE="yes"							#是否设置默认路由=是
IPV4_FAILURE_FATAL="no"			#是否开启ipv4致命检测=否（如果ipv4配置失败禁用设备）
IPV6INIT="yes"							
IPV6_AUTOCONF="yes"					
IPV6_DEFROUTE="yes"
IPV6_FAILURE_FATAL="no"
IPV6_ADDR_GEN_MODE="stable-privacy"
NAME="ens160"								#物理网卡设备名字
UUID="aa1bed39-d2ef-43a6-bf70-560fc2fef10a" #网卡uuid
DEVICE="ens160"							#网卡名字
ONBOOT="yes"								#开机或重启时是否启动网卡
IPADDR="192.168.49.101"			#ipv4地址
PREFIX="24"									#子网掩码
GATEWAY="192.168.49.1"			#网关地址
DNS1="8.8.8.8"							#dns服务器ip
DNS2="8.8.4.4"							#备用dns服务器ip
```

```shell
[root@localhost ~]# ifconfig
ens160: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.49.135  netmask 255.255.255.0  broadcast 192.168.49.255
        inet6 fe80::a085:395a:93a0:e0ef  prefixlen 64  scopeid 0x20<link>
        ether 00:0c:29:ea:b2:d1  txqueuelen 1000  (Ethernet)
        RX packets 118  bytes 11932 (11.6 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 91  bytes 11671 (11.3 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
#解释：
ens160												#网卡名称
flags=4163								  	#标志
UP														#网卡处于活跃状态
BROADCAST											#支持广播
RUNNING												#网线已接入
MULTICAST											#支持组播
mtu 1500											#最大传输单元（字节），表示网卡一次能传输的最大数据包
inet 192.168.49.135						#ipv4地址
netmask 255.255.255.0					#子网掩码
broadcast 192.168.49.255			#广播地址
inet6 fe80::a085:395a:93a0:e0ef						#ipv6地址
prefixlen 64   scopeid 0x20<link> 				#前缀64 作用域0x20
ether 00:0c:29:ea:b2:d1					#网卡mac地址
txqueuelen 1000  (Ethernet)		#网卡设置的传输队列长度
RX packets 118  bytes 11932 (11.6 KiB)				#接收正确的数据包数，接收正确的数据包数量与字节
RX errors 0  dropped 0  overruns 0  frame 0		#接收错误的数据包数、丢弃的数据包数、由于速度过快丢失的数据包、发生frame错误而丢失的数据包数
TX packets 91  bytes 11671 (11.3 KiB)					#输出正确的数据包，输出的数据量和字节
TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0	#输出时产生错误的数据包数、丢弃的数据包数、由于速度过快而丢失的数据包数、发生carrier错误而丢弃的数据包数、冲突信息包的数
```

```shell
#查看指定网卡的信息
[root@localhost ~]# ifconfig ens160
ens160: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.49.135  netmask 255.255.255.0  broadcast 192.168.49.255
        inet6 fe80::a085:395a:93a0:e0ef  prefixlen 64  scopeid 0x20<link>
        ether 00:0c:29:ea:b2:d1  txqueuelen 1000  (Ethernet)
        RX packets 223  bytes 55530 (54.2 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 193  bytes 24774 (24.1 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
```

#### 查看主机名修改主机名

- /etc/hostname文件用于存放主机名
- hostname命令用于显示和设置主机名
- 命令格式：hostname [新主机名]
- hostnamectl set-hostname 主机名：永久设置主机名

```shell
[root@localhost ~]# cat /etc/hostname 
localhost.localdomain
[root@localhost ~]# hostname canvs
[root@localhost ~]# exit
注销
Last login: Thu Apr 27 23:17:39 2023 from 192.168.49.1
[root@canvs ~]# hostname
canvs
```

#### vi/vim文本编辑器

- vim是从vi发展出来的一个文本编辑器，vim具有程序编辑的能力，可以主动的以字体颜色辨别语法的正确性
- vi/vim共分为三种模式：命令模式、输入模式、末行模式
  - 命令模式：启动vi/vim，便进入了命令模式
  - 输入模式：在命令模式下按a/i/o进入输入模式
  - esc键退出输入模式，切换到命令模式
  - 末行模式：在命令模式下按英文冒号 **":"** 进入末行模式
- 命令格式：vim 文件名
  - 若目标文件不存在，则新建文件并编辑
  - 若目标文件存在，则打开文件并编辑
- 命令模式：
  - i 切换到输入模式，在当前光标所在字符前插入
  - a 切换到输入模式，在当前光标所在字符后插入
  - o 切换到输入模式，在当前光标所在行下插入新行
  - ：切换到末行模式，以在最底一行输入命令
  - x  在命令模式下删除当前光标所在单 位
  - dd 删除光标所在一整行，配合数字可删除指定范围内的行；也叫剪切
  - C   删除当前光标及光标后所有内容并进入输入模式
  - u   恢复上一次修改内容，一次恢复一个操作，可多次恢复，直到恢复本次操作初始状态为止
  - $   将光标移动至行尾
  - 0（零）将光标移动至行首
  - gg  跳转至文件第一行
  - G   跳转至文件最后一行
  - yy  复制当前行，配合数字可以同时复制多行
  - p    粘贴当前光标所在行下
  - /关键字  搜索文件内关键字，n从上向下快速定位关键字，N从下向上快速定位关键字

- 末行模式：
  - :w	 保存
  - :q      退出
  - :wq   保存并退出
  - :q!     强制不保存并退出
  - :wq!  强制保存并退出
  - :set nu  以行号形式显示文件内容
  - :set nonu  取消行号
  - :n       快速跳转到指定行号
  - :r       读入另一个文件的数据，文件内容添加到光标的下一行

#### 修改网卡IP地址

- 网卡配置文件：/etc/sysconfig/network-scripts/网卡名
- systemctl restart network  #重启网络
- ifup 网卡名     #启动该网卡设备
- ifdown 网卡名   #禁用网卡名
- 使用**nmcli**命令修改网卡IP地址
  - nmcli connection modify ens160 ipv4.method manual ipv4.addresses 192.168.49.200/24 connection.autoconnect yes
    - nmcli connection modify： 修改
    - ens160 ipv4.method： 配置ipv4的地址方法
    - manual：自动配置
    - ipv4.addresses 192.168.49.200/24 ：ipv4地址/子网掩码
    - connection.autoconnect yes ：开机自动连接
  - nmcli connection up ens160：激活网卡
  - nmcli connection down ens160：关闭网卡
  - nmcli connection reload ens160：重载网卡

#### host命令

- host用于将一个域名解析到一个IP地址

```shell
[root@Canvs ~]# host www.baidu.com
www.baidu.com has address 39.156.66.18
www.baidu.com has address 39.156.66.14
www.baidu.com is an alias for www.a.shifen.com.
www.baidu.com is an alias for www.a.shifen.com.
```

#### nslookup命令

- nslookup用于查询域名解析是否正常，在网络故障时用来诊断网络问题

```shell
[root@Canvs ~]# nslookup www.baidu.com
Server:         192.168.49.2
Address:        192.168.49.2#53

Non-authoritative answer:
Name:   www.baidu.com
Address: 39.156.66.14
Name:   www.baidu.com
Address: 39.156.66.18
www.baidu.com   canonical name = www.a.shifen.com.
```

#### alias别名管理

- alias命令用于设置命令别名，用户可以使用alias自定义命令别名来简化命令的复杂度，不能与系统命令重名
- 命令格式：alias  [别名]=[命令]     
  - 注意事项：等号前后不能有空格，前后命令中有空格需要用**" "或' '** 区分

- unalias 别名    取消别名

```shell
[root@Canvs ~]# alias
alias cp='cp -i'
alias egrep='egrep --color=auto'
alias fgrep='fgrep --color=auto'
alias grep='grep --color=auto'
alias l.='ls -d .* --color=auto'
alias ll='ls -l --color=auto'
alias ls='ls --color=auto'
alias mv='mv -i'
alias rm='rm -i'
alias which='(alias; declare -f) | /usr/bin/which --tty-only --read-alias --read-functions --show-tilde --show-dot'
alias xzegrep='xzegrep --color=auto'
alias xzfgrep='xzfgrep --color=auto'
alias xzgrep='xzgrep --color=auto'
alias zegrep='zegrep --color=auto'
alias zfgrep='zfgrep --color=auto'
alias zgrep='zgrep --color=auto'
```

#### history管理历史命令

- history命令用于显示历史记录和执行过的命令，登录shell时会读取 **~./bash_history** 历史文件中记录下的命令，当退出或登出shell时，会自动保存到历史命令文件，该命令单独使用时，仅显示历史命令

- 命令格式：history [-选项] [参数]
- 常用选项：
  - -a 追加本次新执行的命令至历史命令文件中
  - -d 删除历史命令中指定的命令
  - -c 清空历史命令列表
- 快捷操作：
  - !#  调用历史命令中第N条命令
  - !string  调用历史命令中以string开头的命令
  - !!  重复执行上一条命令

#### date和clock命令

- date用于显示或设置系统日期与时间
- 命令格式：date [-选项] [+格式符]    查看系统日期时间
- 常用选项：
  - -s 设置日期时间
  - 格式符：
    - +%Y 年份
    - +%B 月份
    - +%d  日
    - +%H 时
    - +%M 分
    - +%S  秒
    - +%F 年-月-日
    - +%X 时：分：秒
- clock用于显示硬件时间
  - hwclock -w ：将硬件时间设置成与系统时间相同
  - hwclock -s ：将系统时间设置成与硬件时间相同

```shell
[root@Canvs ~]# date
2023年 04月 29日 星期六 13:10:14 CST
[root@Canvs ~]# hwclock -s
[root@Canvs ~]# clock
2023-04-29 13:10:43.024903+08:00
# 查看日历
[root@Canvs ~]# cal
      四月 2023     
日 一 二 三 四 五 六
                   1
 2  3  4  5  6  7  8
 9 10 11 12 13 14 15
16 17 18 19 20 21 22
23 24 25 26 27 28 29
30                  
```

#### 管道符

- 管道符 **'|'** :将命令的输出结果交给另外一条命令作为参数继续处理 

```shell
# 以行号显示文件前10行后5行的内容
[root@Canvs ~]# cat -n anaconda-ks.cfg | head -10 | tail -5
     6  # Use graphical install
     7  graphical
     8  repo --name="AppStream" --baseurl=file:///run/install/repo/AppStream
     9  # Use CDROM installation media
    10  cdrom
```

#### wc命令

- wc用于统计文件的字节数、行数，并将统计结果输出到屏幕
- 命令格式：wc [-选项] 文件名
- 常用选项：
  - -c 统计字节数
  - -l 统计行数

```shell
[root@Canvs ~]# wc anaconda-ks.cfg 
  44  116 1191 anaconda-ks.cfg
  行数 单词 字节
```

#### 重定向操作

- 将前面命令的输出结果，写入到其他的文本文件中
- 表示符号:
  - \>:重定向输出覆盖，只收集正确的输出结果
  - \>>: 重定向输出追加
  - \<: 输入重定向覆盖
  - \<<: 输入重定向追加
  - 2>:  只收集错误的输出结果
  - &> : 正确错误都收集

#### echo命令

- echo是一种最常用的与广泛使用的内置于Linux的bash和C shell的命令，通常用在脚本语言和批处理文件中来在标准输出或者文件中显示一行文本或者字符串。
- 命令格式：echo [-选项] [参数]

```shell
[root@localhost ~]# echo helloworld > hello.py 
[root@localhost ~]# cat study/hello.py 
helloworld
[root@localhost ~]# echo 你好世界！>> hello.py 
[root@localhost ~]# cat study/hello.py 
helloworld
你好世界！
# 输出系统环境变量
[root@Canvs ~]# echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/root/bin
```

#### sleep命令

- sleep命令用于将目前动作延迟一段时间
- 命令格式：sleep 时间
- 常用选项：
  - s 秒
  - m 分钟
  - h 小时
  - d 日

```shell
[root@Canvs ~]# sleep 3s
```

#### 用户账号管理

- 用户账号可用于登录系统，可以实现访问控制
- 用户模版目录：/etc/skel/

#### useradd创建用户

- useradd 命令用于创建新的用户
- 命令格式：useradd [-选项] 用户名
- 常用选项：
  - -u 指定用户UID
  - -d 指定用户家目录
  - -c 用户描述信息
  - -g 指定用户基本组
  - -G 指定用户附加组
  - -s 指定用户的shell

```shell
[root@Canvs ~]# useradd user1
#/sbin/nologin：禁止用户登录系统
[root@Canvs ~]# useradd -s /sbin/nologin user2
```

#### id命令

- id命令用于查看系统用户和用户所在组的信息
- 命令格式：id [-选项] [用户名]

```shell
[root@Canvs ~]# id user1
uid=1000(user1) gid=1000(user1) 组=1000(user1)
```

#### /etc/passwd用户信息文件

用于存放用户的基本信息文件

- **用户名：密码占位符：UID：基本组GID：用户描述信息：用户家目录：解释器程序**

- UID：0 					超级用户

- UID：1-499			系统伪用户，不能登录系统并且没有家目录

- UID：500-65535	普通用户

```shell
[root@Canvs ~]# cat /etc/passwd
root:x:0:0:root:/root:/bin/bash
bin:x:1:1:bin:/bin:/sbin/nologin
user1:x:1000:1000::/home/user1:/bin/bash
```

#### /etc/default/useradd文件

- 用于存放用户默认值信息

```shell
[root@Canvs ~]# cat /etc/default/useradd 
# useradd defaults file
GROUP=100				#用户默认组
HOME=/home			#用户家目录
INACTIVE=-1			#密码过期宽限天数（/etc/shadow文件第7个字段）
EXPIRE=					#密码失效日期（/etc/shadow文件第8个字段）
SHELL=/bin/bash	#默认使用的shell
SKEL=/etc/skel	#模版目录
CREATE_MAIL_SPOOL=yes	#是否建立邮箱
```

#### /var/spool/mail/ 用户邮件目录

```shell
[root@Canvs ~]# ll /var/spool/mail/
总用量 0
-rw-rw----. 1 user1 mail 0 4月  29 14:44 user1
```

#### passwd设置用户密码

- passwd命令用于设置用户密码
- 命令格式：passwd [-选项]  [用户名]
- 密码规范：长度不能少于8个字符，复杂度（数字、字母区分大小写、特殊字符）
- 常用选项：
  - -S 查看密码信息
  - -l 锁定用户密码
  - -u 解锁用户密码
  - -d 删除密码
  - --stdin 通过管道方式设置用户密码
    - 非交互设置用户密码
    - 命令格式：echo "密码" ｜ passwd --stdin 用户名

#### /etc/shadow用户密码文件

- 用户的密码信息存放在/etc/shadow文件中，该文件默认任何人都没有任何权限（不包括root）

```shell
[root@Canvs ~]# cat /etc/shadow
root:$6$9xY0y.9t47/FUzTu$MBHC3Dwq/7J3Rip19b7mtfEwGRb3JT.reJwIYMeBQZlqUM.6x4D5RmQnBMaphU81Z47eFvGioCoN8Sw.6TYYF.::0:99999:7:::
bin:*:17784:0:99999:7:::
user1:$6$gztIjp4aFADpp9jg$X9KrRa0oMlbaAi/3V03fveX2iu7gsYo52saXuK.H7kq5HUkDNRG/jwHEc1ETj49bWyoofLVX.LgRoXoSQNN7i.:19476:0:99999:7:::
user2:!!:19476:0:99999:7:::

#第一字段：用户名
#第二字段：密码加密字符串，加密算法SHA52散列加密算法，如果密码位是 "*" 或 "!!" 表示密码已过期
#第三字段：密码最后一次修改时间，日期从1970年1月1日起，每过一天时间戳加1
#第四字段：密码修改期限，如果改字段为0表示随时可以修改密码，如果为10，表示10天内不可修改密码
#第五字段：密码有效期
#第六字段：密码到期前警告时间
#第七字段：密码过期后的宽限天数
#第八字段：账号失效时间，日期从1970年1月1日起
#第九字段：保留
```

#### su命令

- su命令用于切换当前用户身份到其他身份
- 命令格式：su [-选项] [用户名]

```shell
[user3@Canvs ~]$ su root
Password: 
[root@Canvs user3]# 
[root@Canvs ~]# su user3
[user3@Canvs root]$ 
```

#### usermod修改用户属性

- usermod命令用于修改已存在用户的基本信息
- 命令格式：usermod [-选项] 用户名
- 常用选项：
  - -u 修改用户UID
  - -d 修改用户家目录
  - -g 修改用户进本组
  - -G 添加用户附加组
  - -s 修改用户shell

```shell
[root@Canvs ~]# usermod -g 1000 user3
[root@Canvs ~]# usermod -u 1580 user3
[root@Canvs ~]# id user3
uid=1580(user3) gid=1000(user1) 组=1000(user1),1001(user2)
```

#### userdel删除用户

- userdel用于删除给定的用户以及与用户相关的文件，该命令不加选项仅删除用户账号，不删除用户相关文件
- 命令格式：userdel [-选项] 用户名
- 常用选项：
  - -r 删除用户同时，删除与用户相关的所有文件

```shell
[root@Canvs ~]# userdel -r user1
```

#### groupadd添加新组

- groupadd用于创建一个新的工作组，新组的信息将被添加到/etc/group文件中
- 命令格式：groupadd [- 选项] 组名
- 常用选项：
  - -g GID	      #指定组的id

```shell
[root@Canvs ~]# groupadd study
```

#### /etc/group组信息文件

- 组信息存放在/etc/group文件中

```shell
[root@Canvs ~]# cat /etc/group
root:x:0:
bin:x:1:
user1:x:1000:
user2:x:1001:
# 组名：组密码占位符：GID：组内附加用户
```

#### /etc/gshadow组密码文件

- 组密码信息存放在/etc/gshadow文件中

```shell
[root@Canvs ~]# cat /etc/gshadow
root:::
bin:::
user1:!::
user2:!::
# 组名：组密码：组内管理员：组内附加用户
```

#### groupmod修改组属性

- groupmod用于修改指定工作组属性
- 命令格式：groupmod [-选项] 组名
- 常用选项：
  - -g GID     #修改组的GID
  - -n 新组名   #修改组名

#### gpasswd组内管理员命令

- gpasswd是Linux工作组文件/etc/group和/etc/gshadow管理工具，用于将用户添加到组或从组内删除
- 命令格式：gpasswd [-选项] 用户名 组名
- 常用选项：
  - -a #将用户添加到工作组
  - -d #将用户工作组中删除

```shell
[root@Canvs ~]# gpasswd -a tom study
正在将用户“tom”加入到“study”组中
[root@Canvs ~]# gpasswd -a jack study
正在将用户“jack”加入到“study”组中
[root@Canvs ~]# gpasswd -a lisa study
正在将用户“lisa”加入到“study”组中
[root@Canvs ~]# cat /etc/group
study:x:1003:tom,jack,lisa
[root@Canvs ~]# gpasswd -d tom study
正在将用户“tom”从“study”组中删除
```

#### groupdel删除组

- groupdel 用于删除指定工作组
- 命令格式：groupdel 组名

```shell
[root@Canvs ~]# groupdel study
```

#### chmod权限管理

- chmod（change mode）设置用户对文件的权限
- 常用命令：chmod [-选项] 归属关系+-=权限类别文件...
- 常用选项：
  - -R   递归修改，包含目录下所有字文件与字目录
- 归属关系：u 所有者、g 所属组、o 其他人
- 权限操作：
  - \+ 添加权限
  - \- 去除权限
  - = 重新定义权限
- 数字权限表示：
  - 4 - r	可读
  - 2 - w   可写
  - 1 - x    可执行
  - 0         没有权限

```shell
[root@Canvs ~]# ll
总用量 4
----------. 1 root root    0 4月  29 20:15 hello.py
[root@Canvs ~]# chmod u+rwx,g+rx,o+rx hello.py 
[root@Canvs ~]# ll -d
dr-xr-x---. 2 root root 167 4月  29 20:15 .
[root@Canvs ~]# chmod u-x,g-x,o-x hello.py 
[root@Canvs ~]# ll
总用量 4
-rw-r--r--. 1 root root    0 4月  29 20:15 hello.py
[root@Canvs ~]# chmod u=rwx,g=rx,o=rx hello.py 
[root@Canvs ~]# ll
总用量 4
-rwxr-xr-x. 1 root root    0 4月  29 20:15 hello.py
[root@Canvs ~]# chmod 777 hello.py 
[root@Canvs ~]# chmod 000 hello.py 
[root@Canvs ~]# ll
总用量 4
----------. 1 root root    0 4月  29 20:15 hello.py
```

#### umask预设权限

- umask用于显示或设置创建文件的权限掩码
- 命令格式：umask [-p] [-S] [模式]
- 常用选项：
  - -p         如果省略 MODE 模式，以可重用为输入的格式输入
  - -S         以符号形式输出，否则以八进制数格式输出


#### chown归属关系管理

- chown（change owner）用于设置文件的所有者和所属组关系
- 命令格式：
  - chown [-选项] 所有者:所属组 文件  #同时修改所有者和所属组身份
  - chown [-选项] 所有者 文件   #只修改所有者身份
  - chown [-选项] :所属组 文件 #只修改所属组身份
- 常用选项：
  - -R 递归修改

```shell
[root@Canvs ~]# touch /test/hello.txt
[root@Canvs ~]# chmod -R 770 /test/
[root@Canvs ~]# ll /test/
总用量 0
-rwx-rwx-----. 1 root endless 0 4月  29 21:17 hello.txt
[root@Canvs ~]# chown -R :endless /test/
[endless@Canvs test]$ ll
total 4
-rwxrwx---. 1 root endless 16 Apr 29 21:21 hello.txt
[endless@Canvs test]$ echo 你好世界！>> hello.txt 
[root@Canvs ~]# cat /test/hello.txt 
你好世界！
```

#### SetUID特殊权限

- SetUID（SUID）：对于一个可执行的文件用了SUID权限后，普通用户在执行该文件后，临时拥有了所有者的身份，该权限只在程序执行过程中有效，程序执行完毕后用户恢复原油身份
- SetUID权限会附加在所有者的x权限位上，所有者的x权限标识会变成s，如果该文件没有x权限那么权限位会变成S
- 设置SetUID命令格式：chmod u+s 文件名

```shell
[endless@Canvs test]$ which passwd
/usr/bin/passwd
[endless@Canvs test]$ ll -d /usr/bin/passwd 
-rwsr-xr-x. 1 root root 34512 Aug 13  2018 /usr/bin/passwd
# 给cat添加SUID权限
[root@Canvs ~]# chmod u+s /usr/bin/cat
[root@Canvs ~]# ll -d /usr/bin/cat
-rwsr-xr-x. 1 root root 51856 1月  11 2019 /usr/bin/cat
# 给cat删除SUID权限
[root@Canvs ~]# chmod u-s /usr/bin/cat
[root@Canvs ~]# ll -d /usr/bin/cat
-rwxr-xr-x. 1 root root 51856 1月  11 2019 /usr/bin/cat
```

#### SetGID特殊权限

- SetGID（SGID）：当对一个可执行的二进制文件设置了SGID后，普通用户在执行该文件时临时拥有其所属组的权限，该权限只在程序执行过程中有效，程序执行完毕后用户恢复原有组身份
- 当对一个目录设置了SGID权限后，普通用户在该目录下创建的文件的所属组，均与该目录所属组相同
- SetGID权限会附加在所属组的x权限位上，所属组的x权限标识会变成s
- 设置SetGID命令格式：chmod g+s 文件名

```shell
[root@Canvs ~]# which locate
/usr/bin/locate
[root@Canvs ~]# ll -d /usr/bin/locate
-rwx--s--x. 1 root slocate 48552 5月  11 2019 /usr/bin/locate

[endless@Canvs test]$ ll -d /usr/bin/locate
-rwx--s--x. 1 root slocate 48552 May 11  2019 /usr/bin/locate
```

#### Sticky BIT特殊权限

- Sticky BIT（SBIT）：该权限只针对于目录有效，当普通用户对一个目录拥有w和x权限时，普通用户可以在此目录下拥有增删改的权限，因为普通用户对目录拥有w权限时，是可以删除此目录下的所有文件
- 如果对一个目录设置了SBIT权限，除root可以删除所有文件以外，普通用户就算对该目录拥有w权限，也只能删除自己建立的文件，不能删除其他用户建立的文件
- SBIT权限会附加在其他人的x权限位上，其他人的x权限标识会变成t
- 设置SBIT命令格式：chmod o+t 目录名

**root**

```shell
[root@Canvs /]# chmod 777 test/
[root@Canvs /]# 
[root@Canvs /]# ll -d /test/
drwxrwxrwx. 2 root root 6 4月  29 21:49 /test/
[root@Canvs /]# chmod o+t test/
[root@Canvs /]# ll -d /test/
drwxrwxrwt. 2 root root 25 4月  29 21:50 /test/
[root@Canvs /]# ll /test/
总用量 0
-rw-rw-r--. 1 endless endless 0 4月  29 21:50 endless.txt
-rw-rw-r--. 1 jack    jack    0 4月  29 21:51 jack.txt
```

**endless**

```shell
[endless@Canvs test]$ touch endless.txt
[endless@Canvs test]$ ls
endless.txt  jack.txt
[endless@Canvs test]$ rm -rf jack.txt 
rm: cannot remove 'jack.txt': Operation not permitted
```

**jack**

```shell
[jack@Canvs test]$ touch jack.txt
[jack@Canvs test]$ ls
endless.txt  jack.txt
[jack@Canvs test]$ rm -rf endless.txt 
rm: cannot remove 'endless.txt': Operation not permitted
```

#### FACL访问控制列表

- FACL（Filesystemctl Access Control List）文件访问控制列表：利用文件扩展属性保存额外的访问控制权限，单独为每一个用户量身定制一个权限
- 命令格式：setfacl 选项 u:用户名:权限 文件
- 常用选项：
  - -m 设置权限
  - -x 删除指定用户权限
  - -b 删除所有用户权限

**root**

```shell
[root@Canvs /]# groupadd dev
[root@Canvs /]# gpasswd -a endless dev
正在将用户“endless”加入到“dev”组中
[root@Canvs /]# mkdir /dev_test
[root@Canvs /]# chown :dev /dev_test/
[root@Canvs /]# ll dev_test/
总用量 0
[root@Canvs /]# ll -d dev_test/
drwxrwx---. 2 root dev 6 4月  29 22:27 dev_test/
[root@Canvs /]# getfacl /dev_test/
getfacl: Removing leading '/' from absolute path names
# file: dev_test/
# owner: root
# group: dev
user::rwx
group::rwx
other::---
# 为jack用户设置FACL权限rx
[root@Canvs /]# setfacl -m u:jack:rx /dev_test/
[root@Canvs /]# getfacl /dev_test/
getfacl: Removing leading '/' from absolute path names
# file: dev_test/
# owner: root
# group: dev
user::rwx
user:jack:r-x
group::rwx
mask::rwx
other::---
# 删除FACL权限
[root@Canvs /]# setfacl -x u:jack /dev_test
[root@Canvs /]# getfacl
Usage: getfacl [-aceEsRLPtpndvh] file ...
Try `getfacl --help' for more information.
[root@Canvs /]# getfacl /dev_test/
getfacl: Removing leading '/' from absolute path names
# file: dev_test/
# owner: root
# group: dev
user::rwx
group::rwx
mask::rwx
other::---
```

**endless**

```shell
[endless@Canvs dev_test]$ id endless
uid=1003(endless) gid=1003(endless) groups=1003(endless),1004(dev)
[endless@Canvs dev_test]$ touch endless.sh
[endless@Canvs dev_test]$ ls
endless.sh
```

**jack**

```shell
[jack@Canvs ~]$ cd /dev_test/
-bash: cd: /dev_test/: 权限不够
# root用户设置了FACL权限后
[jack@Canvs ~]$ ll -d /dev_test/
drwxrwx---+ 2 root dev 24 Apr 29 22:29 /dev_test/
[jack@Canvs dev_test]$ touch jack.txt
touch: cannot touch 'jack.txt': Permission denied
# root用户删除了FACL权限
[jack@Canvs ~]$ cd /dev_test/
-bash: cd: /dev_test/: 权限不够
```

#### 常用特殊符号的使用

- Linux系统下通配符起了很大的作用，对于不正确的文件名称可以使用一下特殊字符表示
- \* 通常的特殊符号，在文件名上，用来代表任意多个字符
- ? 常用的特殊字符，在文件名上，用来代表任意单个字符
- [0-9] 在文件名上，用来代表多个字符或连续范围中的一个，若无则忽略
- {a,b,cd,abcd} 在文件名上，用来代表多组不同的字符串，全匹配

```shell
[root@Canvs /]# ls /etc/*.conf
/etc/dracut.conf  /etc/libaudit.conf   /etc/resolv.conf     /etc/updatedb.conf
/etc/fuse.conf    /etc/libuser.conf    /etc/rsyslog.conf    /etc/vconsole.conf
/etc/host.conf    /etc/locale.conf     /etc/sestatus.conf   /etc/xattr.conf
/etc/idmapd.conf  /etc/logrotate.conf  /etc/sudo.conf       /etc/yum.conf
/etc/kdump.conf   /etc/man_db.conf     /etc/sudo-ldap.conf
/etc/krb5.conf    /etc/mke2fs.conf     /etc/sysctl.conf
/etc/ld.so.conf   /etc/nsswitch.conf   /etc/tcsd.conf
[root@Canvs /]# ls /dev/tty?
/dev/tty0  /dev/tty2  /dev/tty4  /dev/tty6  /dev/tty8
/dev/tty1  /dev/tty3  /dev/tty5  /dev/tty7  /dev/tty9
[root@Canvs /]# ls /dev/tty[0-9]
/dev/tty0  /dev/tty2  /dev/tty4  /dev/tty6  /dev/tty8
/dev/tty1  /dev/tty3  /dev/tty5  /dev/tty7  /dev/tty9
[root@Canvs /]# ls /dev/tty{1..20}
/dev/tty1   /dev/tty12  /dev/tty15  /dev/tty18  /dev/tty20  /dev/tty5  /dev/tty8
/dev/tty10  /dev/tty13  /dev/tty16  /dev/tty19  /dev/tty3   /dev/tty6  /dev/tty9
/dev/tty11  /dev/tty14  /dev/tty17  /dev/tty2   /dev/tty4   /dev/tty7
[root@Canvs /]# ls /dev/tty{1,15,2,20,8}
/dev/tty1  /dev/tty15  /dev/tty2  /dev/tty20  /dev/tty8
```

#### grep文件内容过滤

- grep 用于查找文件中符合条件的字符串，它能利用正则表达式搜索文件中的字符串，并把匹配到的字符串的行打印出来
- 命令格式：grep [-选项]  "查找条件" 目标文件
- 常用选项：
  - -n  以行号形式输出
  - -i   忽略字符串大小写
  - -v  显示不包含匹配的行
- 常用正则表达式符号
  - ^字符串    显示以该字符串开头的行
  - $字符串    显示以该字符串结尾的行
  - ^$             显示空行

```shell
# 显示行号包含root的内容
[root@Canvs /]# grep -n root /etc/passw?
1:root:x:0:0:root:/root:/bin/bash
10:operator:x:11:0:operator:/root:/sbin/nologin
# 显示行号查找以root开头的内容
[root@Canvs /]# grep -n ^root /etc/passwd
1:root:x:0:0:root:/root:/bin/bash
# 显示行号查找以bash结尾的内容
[root@Canvs /]# grep -n bash$ /etc/passwd
1:root:x:0:0:root:/root:/bin/bash
22:jack:x:1001:1001::/home/jack:/bin/bash
23:lisa:x:1002:1002::/home/lisa:/bin/bash
24:endless:x:1003:1003::/home/endless:/bin/bash
# 显示行号过滤注释、空行的内容
[root@Canvs /]# grep -v '^#' /etc/login.defs | grep -v '^$' -n
2:MAIL_DIR      /var/spool/mail
4:PASS_MAX_DAYS 99999
5:PASS_MIN_DAYS 0
6:PASS_MIN_LEN  5
7:PASS_WARN_AGE 7
9:UID_MIN                  1000
10:UID_MAX                 60000
11:SYS_UID_MIN               201
12:SYS_UID_MAX               999
14:GID_MIN                  1000
15:GID_MAX                 60000
16:SYS_GID_MIN               201
17:SYS_GID_MAX               999
20:CREATE_HOME  yes
22:UMASK           077
24:USERGROUPS_ENAB yes
26:ENCRYPT_METHOD SHA512
```

#### find文件/目录查找命令

- find命令根据预设的条件递归查找文件或目录所在位置
- 命令格式：find 查找路径 查找条件1 查找条件2 .. [-exec处理命令{}\;]
  - -exec 可接额外的命令来处理查询结果
  - {}代表find查找到的内容被放置{}中
  - \;代表额外处理命令结束
- 常用查询条件
  -  -type类型 （f文件 d目录 l链接文件）
  - -name "文件名"
  - -iname 按文件名查找忽略大小写
  -  -size文件大小（k、M、G + 大于 -小于）
     -  -a 并且两个条件同时满足
     -  -o 两个条件满足任意一个即可
  -  -user 用户名
  -  -mtime 按日期查找（+代表多少天之前 -代表多少天之内 0代表24小时之内）

```shell
# 查询/etc/下所有文件
[root@Canvs ~]# find /etc/ -type f
# 查询/etc/下以tab结尾的所有文件
[root@Canvs ~]# find /etc/ -name "*tab" -type f
/etc/fstab
/etc/crypttab
/etc/inittab
/etc/anacrontab
/etc/crontab
# 查询/etc/下忽略大小的FsTaB文件
[root@Canvs ~]# find /etc/ -iname "FsTaB" -type f
/etc/fstab
[root@Canvs ~]# find /etc/ -size +5M -type f
/etc/selinux/targeted/policy/policy.31
/etc/udev/hwdb.bin
[root@Canvs ~]# ll -h /etc/udev/hwdb.bin  /etc/selinux/targeted/policy/policy.31
-rw-r--r--. 1 root root 8.1M 2月  22 2019 /etc/selinux/targeted/policy/policy.31
-r--r--r--. 1 root root 8.8M 4月  25 13:48 /etc/udev/hwdb.bin
# 查询/etc/下大于1M小于10M的文件
[root@Canvs ~]# find /etc/ -size +1M -a -size -10M -type f
/etc/selinux/targeted/policy/policy.31
/etc/udev/hwdb.bin
# 查询/下用户为endless的所有文件；proc/下存放内存中的文件，时有时无，所以报错
[root@Canvs ~]# find / -user endless -type f
find: ‘/proc/1764/task/1764/fdinfo/7’: 没有那个文件或目录
find: ‘/proc/1764/fdinfo/6’: 没有那个文件或目录
/var/spool/mail/endless
/home/endless/.bash_logout
/home/endless/.bash_profile
/home/endless/.bashrc
/home/endless/.bash_history
# 查找/var/log/下
[root@Canvs ~]# find /var/log/ -mtime +30 -type f
/var/log/README
[root@Canvs ~]# ll -h /var/log/README 
-rw-r--r--. 1 root root 1.1K 2月  26 2019 /var/log/README
# 查找/var/log/下3天前修改的文件拷贝到/tmp/test
[root@Canvs ~]# find /var/log/ -mtime +3 -type f -exec cp {} /tmp/test/ \;
```

#### 压缩与解压缩

- Linux独有压缩格式及命令工具：
  - gzip  .gz
  - bzip2   .bz2
  - xz   .xz
- 命令格式：
  - gzip [-选项..] 文件名
    - 常用选项：-d 解压缩
  - bzip2 [-选项..] 文件名
    - 常用选项：-d 解压缩
  - xz  [-选项..] 文件名
    - 常用选项：-d 解压缩
- 查看压缩文件内容
  - zcat [-选项..] 文件名
  - bzcat [-选项..] 文件名
  - xzcat [-选项..] 文件名

```shell
[root@Canvs ~]# ll -h services 
-rw-r--r--. 1 root root 677K 4月  30 15:26 services
# gzip压缩文件
[root@Canvs ~]# gzip services 
[root@Canvs ~]# ll -h services.gz 
-rw-r--r--. 1 root root 140K 4月  30 15:26 services.gz
# 查看压缩文件内容
[root@Canvs ~]# zcat services.gz 
# gzip解压缩
[root@Canvs ~]# gzip -d services.gz 
[root@Canvs ~]# bzip2 services 
[root@Canvs ~]# ll -h services.bz2 
-rw-r--r--. 1 root root 127K 4月  30 15:26 services.bz2
[root@Canvs ~]# bzcat services.bz2 
[root@Canvs ~]# bzip2 -d services.bz2 
[root@Canvs ~]# xz services 
[root@Canvs ~]# ll -h services.xz 
-rw-r--r--. 1 root root 104K 4月  30 15:26 services.xz
[root@Canvs ~]# xzcat services.xz 
```

#### tar打包工具

- tar命令用于在Linux下对文件/目录打包，使用tar程序打出来的包称为tar包，tar包文件通常都以.tar结尾
- tar命令格式：tar 选项 压缩包名 被压缩文件
- 常用选项：
  - -c 创建打包文件
  - -f 指定打包后的文件名称，放在所有选项最后
  - -z 调用gzip压缩工具 -J调用xz压缩工具 -j调用bzip2压缩工具
  - -t 列出打包文件内容
  - -x 释放打包文件
  - -C 指定解压路径
  - -v 显示详细信息

```shell
# tar打包/etc/crontab /etc/passwd /home/
[root@Canvs ~]# tar -zvcf /root/xxoo.tar.gz /etc/crontab /etc/passwd /home/
tar: 从成员名中删除开头的“/”
/etc/crontab
tar: 从硬连接目标中删除开头的“/”
/etc/passwd
/home/
home/
home/jack/
home/jack/.bash_logout
home/jack/.bash_profile
home/jack/.bashrc
home/jack/.bash_history
[root@Canvs ~]# ll -h xxoo.tar.gz 
-rw-r--r--. 1 root root 1.8K 4月  30 15:38 xxoo.tar.gz
# 查看打包文件内容
[root@Canvs ~]# tar -tf xxoo.tar.gz 
etc/crontab
etc/passwd
home/
home/jack/
home/jack/.bash_logout
home/jack/.bash_profile
home/jack/.bashrc
home/jack/.bash_history
# 解压缩文件
[root@Canvs ~]# tar -xvf xxoo.tar.gz -C /root/test/
etc/crontab
etc/passwd
home/
home/jack/
home/jack/.bash_logout
home/jack/.bash_profile
home/jack/.bashrc
home/jack/.bash_history
```

#### 磁盘类型介绍

- IDE接口类型：主要用于个人家用计算机
- SCSI接口类型： 主要用于服务器，数据传输速度快，支持热插拔
- STAT接口类型：主要用于个人计算机
- NVME接口类型：固态硬盘接口

#### Linux常用分区格式

- MBR分区格式：比较古老的分区格式，分为主分区与扩展分区，最大支持2.2T以内磁盘容量
- GPT分区格式：可划分128个主分区，最大支持18EB磁盘容量（1EB=1024PB，1PB=1024TB）

| 分区方式 | 位数 | 分区表大小 | 支持分区个数                      | 单个分区支持大小 |
| -------- | ---- | ---------- | --------------------------------- | ---------------- |
| MBR      | 32   | 64         | 主分区4个（3个主分区+1个扩展分区) | 2.2TB            |
| GPT      | 64   | 128        | 128个主分区                       | 18EB             |

#### 文件系统类型详解

- 文件管理系统，赋予分区文件系统分区才可以正常使用

- CentOS6：分区默认使用文件系统类型ext3
- CentOS6：分区默认使用文件系统类型ext4
  - ext4日志记录功能，意外宕机，通过日志记录吧没有保存的数据，在系统在此重启时快速恢复
  - 单个文件系统最大支持1EB的分区容量，单个文件最大可以存储16TB数据
- CentOS7：分区默认使用文件系统类型xfs
  - xfs开启了日志记录的功能，数据 恢复的时候比ext4文件系统快
  - 单个文件系统最大支持8EB分区容量，单个文件最大可以存储500TB的数据
  - 单个文件每秒读写数据的速度可以达到4G
- swap文件系统：交换分区，硬盘空间充当内存使用

#### 挂载

- 在Linux系统中用户无法直接使用硬件设备，硬件设备在系统中都是以只读的方式存在的，必须挂载
- 挂载就是给我门用户提供一个可以使用设备的一个接口
- 挂载注意事项：
  - 挂载点必须是一个目录，理论上还得是一个空目录

#### lsblk命令

- 用于列出所有可用块设备的信息，而且还能显示他们之间的依赖关系，但是它不会列出RAM盘的信息
- 命令格式：lsblk [-选项...] [设备名]
- 常用选项：
  - \-d     仅显示磁盘本身，不会列出磁盘的分区数据
  - \-f      列出磁盘分区使用的文件类型

```shell
# 列出当前系统所有磁盘与磁盘内的分区信息
[root@localhost ~]# lsblk
NAME          MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sr0            11:0    1  6.6G  0 rom  
nvme0n1       259:0    0   20G  0 disk 
├─nvme0n1p1   259:1    0    1G  0 part /boot
└─nvme0n1p2   259:2    0   19G  0 part 
  ├─rhel-root 253:0    0   17G  0 lvm  /
  └─rhel-swap 253:1    0    2G  0 lvm  [SWAP]
# NAME ：设备名称
# MAJ:MIN ：主设备号:次设备号，内核通过主次设备号识别磁盘
# RM ：是否为可卸载设备，1可卸载，0不可卸载
# SIZE ：设备的容量大小
# RO ：表示设备是否为只读，0非只读设备，1只读设备
# TYPE ：表示设备类型（disk为磁盘，part为分区，lvm逻辑卷，rom只读）
# MOUNTPOINT ：设备挂在点（SWAP没有挂载点）

[root@Canvs ~]# lsblk -f
NAME          FSTYPE    LABEL                    UUID                                   MOUNTPOINT
sr0           iso9660   RHEL-8-0-0-BaseOS-x86_64 2019-04-04-08-40-23-00                 
nvme0n1                                                                                 
├─nvme0n1p1   xfs                                06438da3-eaa0-459b-9091-6fee1e244aca   /boot
└─nvme0n1p2   LVM2_memb                          wX3tOu-WDtb-B4e9-BnqU-hwbB-7Aj9-Q3UF11 
  ├─rhel-root xfs                                366b9f06-3974-4bb9-b8b1-bce6b9789df7   /
  └─rhel-swap swap                               85c063b0-cedb-413e-a2fd-5c066c8075ed   [SWAP]
```

#### df查看分区使用情况

- df命令用于查看文件系统使用情况
- 命令格式：df [选项...] [参数...]
- 常用选项：
  - -h 以人类易读方式显示文件系统容量
  - T 显示文件系统类型

```shell
[root@Canvs ~]# df -Th
文件系统              类型      容量  已用  可用 已用% 挂载点
devtmpfs              devtmpfs  889M     0  889M    0% /dev
tmpfs                 tmpfs     904M     0  904M    0% /dev/shm
tmpfs                 tmpfs     904M  8.6M  895M    1% /run
tmpfs                 tmpfs     904M     0  904M    0% /sys/fs/cgroup
/dev/mapper/rhel-root xfs        17G  1.5G   16G    9% /
/dev/nvme0n1p1        xfs      1014M  163M  852M   17% /boot
tmpfs                 tmpfs     181M     0  181M    0% /run/user/0
```

#### du统计文件/目录大小

- du命令用于统计磁盘下目录或文件大小
- 命令格式：du [选项...] [参数...]
- 常用选项：
  - -h 以kb、MB、GB显示文件大小
  - -s 只统计每个参数的总数

```shell
[root@Canvs ~]# du -h /root/
8.0K    /root/test/etc
16K     /root/test/home/jack
12K     /root/test/home/lisa
16K     /root/test/home/endless
44K     /root/test/home
52K     /root/test
792K    /root/
[root@Canvs ~]# du -sh /root
792K    /root
```

#### /dev/目录下文件

```shell
[root@Canvs ~]# ls /dev/
hd[a-t]:IDE设备
sd[a-z]:SCSI设备
fd[0-7]:软盘驱动设备
md[0-32]:软raid设备
loop[0-7]:本地回环设备
lp[0-3]:打印机设备
mem:内存设备
null:空设备，称为黑洞，任何写入数据都将被丢弃
zero:零资源设备，任何写入的数据都将被丢弃
full:满设备，任何写入的数据都将失败
tty[0-63]:虚拟终端设备
random:随机数设备
urandom:随机数设备
port:存取I/O端口
```

#### blkid查看设备属性

- blkid命令显示块设备属性信息（设备名称、设备UUID、文件系统类型）
- 命令格式：blkid [选项...] [参数...]

```shell
[root@Canvs ~]# blkid
/dev/nvme0n1: PTUUID="5d403be6" PTTYPE="dos"
/dev/nvme0n1p1: UUID="06438da3-eaa0-459b-9091-6fee1e244aca" TYPE="xfs" PARTUUID="5d403be6-01"
/dev/nvme0n1p2: UUID="wX3tOu-WDtb-B4e9-BnqU-hwbB-7Aj9-Q3UF11" TYPE="LVM2_member" PARTUUID="5d403be6-02"
/dev/sr0: UUID="2019-04-04-08-40-23-00" LABEL="RHEL-8-0-0-BaseOS-x86_64" TYPE="iso9660" PTUUID="0da1aba4" PTTYPE="dos"
/dev/mapper/rhel-root: UUID="366b9f06-3974-4bb9-b8b1-bce6b9789df7" TYPE="xfs"
/dev/mapper/rhel-swap: UUID="85c063b0-cedb-413e-a2fd-5c066c8075ed" TYPE="swap"
```

#### 分区过程

添加新硬盘-分区-格式化文件系统-挂载使用

扇区是磁盘存储数据的最小单元，默认一个扇区可以存储512字节的数据

#### MBR分区格式

- fdisk命令用于查看磁盘使用情况和磁盘分区（MBR分区格式）
- 命令格式：fdisk [选项...] [设备路径]
- 常用选项：-l 列出磁盘分区表类型与分区信息

```shell
[root@Canvs ~]# fdisk -l /dev/nvme0n1
m		#获取命令帮助
p		#显示磁盘分区表
n		#新增加一个分区
q		#不保存分区退出
d		#删除一个分区
w		#保存一个分区
a		#设置克引导标记
b		#编辑bsd磁盘标签
c		#设置DOS操作系统兼容标记
l		#显示已知的文件系统类型，82为swap交换分区，83为linux分区
o		#建立空白DOS分区表
s		#新建空白SUN磁盘标签
t		#改变分区的系统ID
u		#改变显示记录单位
v		#验证分区表
x		#附加功能
```

```shell
# 开始分区
[root@Canvs ~]# fdisk /dev/nvme0n2 

欢迎使用 fdisk (util-linux 2.32.1)。
更改将停留在内存中，直到您决定将更改写入磁盘。
使用写入命令前请三思。

设备不包含可识别的分区表。
创建了一个磁盘标识符为 0xc02acda3 的新 DOS 磁盘标签。
# 新建分区
命令(输入 m 获取帮助)：n  
分区类型
   p   主分区 (0个主分区，0个扩展分区，4空闲)
   e   扩展分区 (逻辑分区容器)
选择 (默认 p)：p
分区号 (1-4, 默认  1): 
第一个扇区 (2048-52428799, 默认 2048): 
上个扇区，+sectors 或 +size{K,M,G,T,P} (2048-52428799, 默认 52428799): +10G  

创建了一个新分区 1，类型为“Linux”，大小为 10 GiB。

命令(输入 m 获取帮助)：p
Disk /dev/nvme0n2：25 GiB，26843545600 字节，52428800 个扇区
单元：扇区 / 1 * 512 = 512 字节
扇区大小(逻辑/物理)：512 字节 / 512 字节
I/O 大小(最小/最佳)：512 字节 / 512 字节
磁盘标签类型：dos
磁盘标识符：0xc02acda3

设备           启动  起点     末尾     扇区 大小 Id 类型
/dev/nvme0n2p1       2048 20973567 20971520  10G 83 Linux
命令(输入 m 获取帮助)：w
分区表已调整。
将调用 ioctl() 来重新读分区表。
正在同步磁盘。

[root@Canvs ~]# lsblk
NAME          MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sr0            11:0    1  6.6G  0 rom  
nvme0n1       259:0    0   20G  0 disk 
├─nvme0n1p1   259:1    0    1G  0 part /boot
└─nvme0n1p2   259:2    0   19G  0 part 
  ├─rhel-root 253:0    0   17G  0 lvm  /
  └─rhel-swap 253:1    0    2G  0 lvm  [SWAP]
nvme0n2       259:3    0   25G  0 disk 
└─nvme0n2p1   259:5    0   10G  0 part 
```

#### mkfs格式化文件系统

- mkfs命令用于在分区上建立文件系统
- 常用文件系统类型
  - ext4
  - xfs
- 命令格式：
  - mkfs.xfs 分区设备路径   #格式化为xfs类型文件系统
  - mkfs.ext4 分区设备路径  #格式化ext4类型文件系统

```shell
[root@Canvs ~]# mkfs.xfs /dev/nvme0n2p1 
meta-data=/dev/nvme0n2p1         isize=512    agcount=4, agsize=655360 blks
         =                       sectsz=512   attr=2, projid32bit=1
         =                       crc=1        finobt=1, sparse=1, rmapbt=0
         =                       reflink=1
data     =                       bsize=4096   blocks=2621440, imaxpct=25
         =                       sunit=0      swidth=0 blks
naming   =version 2              bsize=4096   ascii-ci=0, ftype=1
log      =internal log           bsize=4096   blocks=2560, version=2
         =                       sectsz=512   sunit=0 blks, lazy-count=1
realtime =none                   extsz=4096   blocks=0, rtextents=0
```

#### mount挂载

- mount文件系统挂载命令
- 命令格式：mount 设备路径   挂载点目录
- 常用选项：
  - -a： 依照配置文件/etc/fstab的数据将所有未挂载的磁盘都挂载起来
  - -o： 该选项后变可跟挂载时额外参数

- remount命令：重新挂载文件系统，在文件系统出错时重新挂载文件系统时非常重要

```shell
[root@Canvs ~]# mount /dev/nvme0n2p1 /test
[root@Canvs ~]# df -Th
文件系统              类型      容量  已用  可用 已用% 挂载点
devtmpfs              devtmpfs  889M     0  889M    0% /dev
tmpfs                 tmpfs     904M     0  904M    0% /dev/shm
tmpfs                 tmpfs     904M  8.6M  895M    1% /run
tmpfs                 tmpfs     904M     0  904M    0% /sys/fs/cgroup
/dev/mapper/rhel-root xfs        17G  1.5G   16G    9% /
/dev/nvme0n1p1        xfs      1014M  163M  852M   17% /boot
tmpfs                 tmpfs     181M     0  181M    0% /run/user/0
/dev/nvme0n2p1        xfs        10G  104M  9.9G    2% /test
```

#### umount卸载

- umonut命令用于卸载文件系统
- 命令格式：umount 挂载点目录

```shell
[root@Canvs ~]# umount /test
[root@Canvs ~]# df -Th
文件系统              类型      容量  已用  可用 已用% 挂载点
devtmpfs              devtmpfs  889M     0  889M    0% /dev
tmpfs                 tmpfs     904M     0  904M    0% /dev/shm
tmpfs                 tmpfs     904M  8.6M  895M    1% /run
tmpfs                 tmpfs     904M     0  904M    0% /sys/fs/cgroup
/dev/mapper/rhel-root xfs        17G  1.5G   16G    9% /
/dev/nvme0n1p1        xfs      1014M  163M  852M   17% /boot
tmpfs                 tmpfs     181M     0  181M    0% /run/user/0
```

#### /etc/fstab开机自动挂载

- /etc/fstab用于存放文件系统信息，当系统启动时，系统会自动读取文件内容将指定的文件系统挂载到指定的目录
- 文件内容详解

```shell
/dev/mapper/rhel-root   /                       xfs     defaults        0 0
UUID=06438da3-eaa0-459b-9091-6fee1e244aca /boot                   xfs     defaults        0 0
/dev/mapper/rhel-swap   swap                    swap    defaults        0 0

# 解释：该文件内容为6个字段
第一个字段：要挂载的设备路径
第二个字段：挂载点目录
第三个字段：设备文件系统类型
第四个字段：挂载参数
第五个字段：是否对文件系统进行备份，0不备份，1为备份
第六个字段：是否检查文件系统顺序，允许的数字是0，1，2；0表示不检查1的优先权限最高
# 挂载参数：
sync，async：此文件系统是否使用同步写入（sync）或异步（async）的内存机制，默认为异步（async）
atime，noatime：更新访问时间/不更新访问时间，访问分区时，是否更新文件的访问时间，默认为更新
ro，rw：挂载文件只为读取（ro）或读写（rw），默认rw
auto，noauto：自动挂载/手动挂载，执行mount -a时，是否自动挂载/etc/fstab文件内容，默认为自动（auto）
dev，nodev：是否允许此文件系统上，可建立装置文件，默认为允许（dev）
suid，nosuid：是否允许文件系统上含有SUID与SGID特殊权限，默认为允许（SUID）
exec，noexec：是否允许文件系统上拥有可执行文件，默认为允许（exec）
user，nouser：是否允许普通用户执行挂载操作，默认为不允许（nouser），只有root用户可以挂载分区
defaults默认值：代表async，rw，auto，dev，suid，exec，nouser七个选项
```

```shell
[root@Canvs ~]# vim /etc/fstab 
/dev/mapper/rhel-root   /                       xfs     defaults        0 0
UUID=06438da3-eaa0-459b-9091-6fee1e244aca /boot                   xfs     defaults        0 0
/dev/mapper/rhel-swap   swap                    swap    defaults        0 0
/dev/nvme0n2p1 /test xfs defaults 0 0
[root@Canvs ~]# mount -a
[root@Canvs ~]# df -hT
文件系统              类型      容量  已用  可用 已用% 挂载点
devtmpfs              devtmpfs  889M     0  889M    0% /dev
tmpfs                 tmpfs     904M     0  904M    0% /dev/shm
tmpfs                 tmpfs     904M  8.6M  895M    1% /run
tmpfs                 tmpfs     904M     0  904M    0% /sys/fs/cgroup
/dev/mapper/rhel-root xfs        17G  1.5G   16G    9% /
/dev/nvme0n2p1        xfs        10G  104M  9.9G    2% /test
/dev/nvme0n1p1        xfs      1014M  163M  852M   17% /boot
tmpfs                 tmpfs     181M     0  181M    0% /run/user/0
```

#### GPT分区格式

- gdisk命令用于查看磁盘使用情况和磁盘分区（GPT分区格式）
- 命令格式：gdisk [选项...] [设备路径]
- 常用选项：-l 列出磁盘分区表类型与分区信息

```shell

p		# 显示磁盘分区表
n		# 新增加一个分区
q		# 不保存分区退出
d		# 删除一个分区
w		# 保存分区退出
```

```shell
[root@Canvs ~]# lsblk /dev/nvme0n3
NAME          MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
nvme0n3       259:5    0   20G  0 disk 
[root@Canvs ~]# gdisk /dev/nvme0n3
GPT fdisk (gdisk) version 1.0.3

Partition table scan:
  MBR: not present
  BSD: not present
  APM: not present
  GPT: not present

Creating new GPT entries.

Command (? for help): p
Disk /dev/nvme0n3: 41943040 sectors, 20.0 GiB
Model: VMware Virtual NVMe Disk
Sector size (logical/physical): 512/512 bytes
Disk identifier (GUID): 911BC8C0-9816-4815-A212-4AAFC8B3323A
Partition table holds up to 128 entries
Main partition table begins at sector 2 and ends at sector 33
First usable sector is 34, last usable sector is 41943006
Partitions will be aligned on 2048-sector boundaries
Total free space is 41942973 sectors (20.0 GiB)

Number  Start (sector)    End (sector)  Size       Code  Name

Command (? for help): n
Partition number (1-128, default 1): 
First sector (34-41943006, default = 2048) or {+-}size{KMGTP}: 
Last sector (2048-41943006, default = 41943006) or {+-}size{KMGTP}: +10G
Current type is 'Linux filesystem'
Hex code or GUID (L to show codes, Enter = 8300): 
Changed type of partition to 'Linux filesystem'

Command (? for help): p
Disk /dev/nvme0n3: 41943040 sectors, 20.0 GiB
Model: VMware Virtual NVMe Disk
Sector size (logical/physical): 512/512 bytes
Disk identifier (GUID): 911BC8C0-9816-4815-A212-4AAFC8B3323A
Partition table holds up to 128 entries
Main partition table begins at sector 2 and ends at sector 33
First usable sector is 34, last usable sector is 41943006
Partitions will be aligned on 2048-sector boundaries
Total free space is 20971453 sectors (10.0 GiB)

Number  Start (sector)    End (sector)  Size       Code  Name
   1            2048        20973567   10.0 GiB    8300  Linux filesystem

Command (? for help): n
Partition number (2-128, default 2): 
First sector (34-41943006, default = 20973568) or {+-}size{KMGTP}: 
Last sector (20973568-41943006, default = 41943006) or {+-}size{KMGTP}: 
Current type is 'Linux filesystem'
Hex code or GUID (L to show codes, Enter = 8300): 
Changed type of partition to 'Linux filesystem'

Command (? for help): p
Disk /dev/nvme0n3: 41943040 sectors, 20.0 GiB
Model: VMware Virtual NVMe Disk
Sector size (logical/physical): 512/512 bytes
Disk identifier (GUID): 911BC8C0-9816-4815-A212-4AAFC8B3323A
Partition table holds up to 128 entries
Main partition table begins at sector 2 and ends at sector 33
First usable sector is 34, last usable sector is 41943006
Partitions will be aligned on 2048-sector boundaries
Total free space is 2014 sectors (1007.0 KiB)

Number  Start (sector)    End (sector)  Size       Code  Name
   1            2048        20973567   10.0 GiB    8300  Linux filesystem
   2        20973568        41943006   10.0 GiB    8300  Linux filesystem

Command (? for help): w

Final checks complete. About to write GPT data. THIS WILL OVERWRITE EXISTING
PARTITIONS!!

Do you want to proceed? (Y/N): y
OK; writing new GUID partition table (GPT) to /dev/nvme0n3.
The operation has completed successfully.			# 创建GPT分区成功

[root@Canvs ~]# lsblk -l /dev/nvme0n3
NAME      MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
nvme0n3   259:5    0  20G  0 disk 
nvme0n3p1 259:7    0  10G  0 part 
nvme0n3p2 259:8    0  10G  0 part 
```

#### LVM逻辑卷

- 逻辑卷：LVM（Logical Volume Manager）逻辑卷管理系统
- LVM是建立在硬盘和分区之上的一个逻辑层，来提高磁盘分区管理的灵活性
- 逻辑卷可以实现将底层的物理分区整合成一个大的虚拟硬盘
- 逻辑卷技术是通过Linux系统内核dm（device mapper）设备映射组件

![lvm](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/lvm.png)

#### LVM逻辑卷相关概念

- 物理卷 Physical Volume(PV) 将实际的磁盘分区（partition）系统识别码（system ID）修改为8e后，再通过pvcreate指令转化为LVM最底层的物理卷，作为后续空间管理的基础
- 卷组 Volume Group(VG）将数个PV进行整合，即变成VG，在32位的操作系统中，LV的大小与PE的大小有关；在64位操作系统中，LV几乎没有容量限制
- 物理区块 Physical Extent(PE) ，他是LVM中的最小单元。PE类似于文件系统中的block
- 逻辑卷 Logical Volume(LV) ，由VG划分而来，LV的大小与PE的大小及PE的数量有关，size（LV） = count（PE）* size（PE）

| 功能         | 物理卷管理**Physical Volume(PV)** | 卷组管理**Volume Group(VG）** | 逻辑卷管理**Logical Volume(LV)** |
| ------------ | :-------------------------------: | :---------------------------: | :------------------------------: |
| scan 扫描    |              pvscan               |            vgscan             |              lvscan              |
| create 创建  |             pvcreate              |           vgcreate            |             lvcreate             |
| display 显示 |             pvdisplay             |           vgdisplay           |            lvdisplay             |
| remove 删除  |             pvremove              |           vgremove            |             lvremove             |
| extend 扩展  |                                   |           vgextend            |             lvextend             |

#### LVM的优缺点

- 优点：
  - 可以在系统运行的状态下动态扩展文件系统的大小
  - 文件系统可以跨越多个磁盘，文件系统大小不受磁盘大小的限制
  - LVM的存储空间可以通过新增磁盘的方式扩容
- 缺点：
  - 从卷组中移除一个磁盘的时候必须要使用reducevg命令
  - 当卷组中有一个磁盘损坏了，整个卷组都会受到影响（由于一份数据看你会同时存储在不同的磁盘中）
  - 在磁盘创建过程中增加了额外的步骤，所以数据存贮性能会受到影响

#### vgcreate创建卷组

- 创建卷组思路：将创建好的物理卷组成卷组（或者直接创建卷组）
- 命令格式：vgcreate 卷组名 设备路径1 设备路径2....

```shell
# 创建dataVG卷组
[root@Canvs ~]# vgcreate dataVG /dev/nvme0n2p2 /dev/nvme0n3p1
  Physical volume "/dev/nvme0n2p2" successfully created.
  Physical volume "/dev/nvme0n3p1" successfully created.
  Volume group "dataVG" successfully created
# 详细显示卷组信息
[root@Canvs ~]# vgdisplay /dev/dataVG
  --- Volume group ---
  VG Name               dataVG			# 卷组名
  System ID             
  Format                lvm2				# 卷组格式
  Metadata Areas        2
  Metadata Sequence No  1
  VG Access             read/write
  VG Status             resizable
  MAX LV                0
  Cur LV                0
  Open LV               0
  Max PV                0
  Cur PV                2
  Act PV                2
  VG Size               19.99 GiB		#卷组大小
  PE Size               4.00 MiB
  Total PE              5118
  Alloc PE / Size       0 / 0   
  Free  PE / Size       5118 / 19.99 GiB
  VG UUID               oRmiXk-WGtF-q2EK-WrMY-GK0s-KTle-P9GjVU  #卷组uuid
# 显示卷组简洁信息
[root@Canvs ~]# vgs dataVG
  VG     #PV #LV #SN Attr   VSize  VFree 
  dataVG   2   0   0 wz--n- 19.99g 19.99g
```

#### lvcreate创建逻辑卷

- 命令格式：lvcreate [-选项...] 卷组
- 常用选项：
  - -L 指定逻辑卷的大小
  - -n 指定逻辑卷名

```shell
# 创建逻辑卷并添加卷组
[root@Canvs ~]# lvcreate -L 19G -n dataLV dataVG
  Logical volume "dataLV" created.
# 显示逻辑卷信息
[root@Canvs ~]# lvs /dev/dataVG/dataLV 
  LV     VG     Attr       LSize  Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  dataLV dataVG -wi-a----- 19.00g      
# 查看卷组信息
[root@Canvs ~]# vgs dataVG
  VG     #PV #LV #SN Attr   VSize  VFree   
  dataVG   2   1   0 wz--n- 19.99g 1016.00m
[root@Canvs ~]# lsblk -l /dev/dataVG/dataLV 
NAME          MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
dataVG-dataLV 253:2    0  19G  0 lvm  
```

#### LVM格式化文件系统

- mkfs.xfs 设备路径
- mkfs.ext4 设备路径

```shell
[root@Canvs ~]# mkfs.xfs /dev/dataVG/dataLV 
meta-data=/dev/dataVG/dataLV     isize=512    agcount=4, agsize=1245184 blks
         =                       sectsz=512   attr=2, projid32bit=1
         =                       crc=1        finobt=1, sparse=1, rmapbt=0
         =                       reflink=1
data     =                       bsize=4096   blocks=4980736, imaxpct=25
         =                       sunit=0      swidth=0 blks
naming   =version 2              bsize=4096   ascii-ci=0, ftype=1
log      =internal log           bsize=4096   blocks=2560, version=2
         =                       sectsz=512   sunit=0 blks, lazy-count=1
realtime =none                   extsz=4096   blocks=0, rtextents=0
[root@Canvs ~]# blkid /dev/dataVG/dataLV 
/dev/dataVG/dataLV: UUID="d40cc212-2ebe-4e72-a544-0b0f1e9b4949" TYPE="xfs"
```

#### LVM挂载

- mount 设备路径
- /etc/fstab 添加设备

```shell
[root@Canvs /]# mount /dev/dataVG/dataLV /data
[root@Canvs /]# df -Th /data
文件系统                  类型  容量  已用  可用 已用% 挂载点
/dev/mapper/dataVG-dataLV xfs    19G  168M   19G    1% /data
```

#### vgextend扩展卷组

- 命令格式：vgextend  卷组名 设备名...

```shell
# 将磁盘添加到卷组
[root@Canvs /]# vgextend dataVG /dev/nvme0n3p2
  Physical volume "/dev/nvme0n3p2" successfully created.
  Volume group "dataVG" successfully extended
[root@Canvs /]# vgs
  VG     #PV #LV #SN Attr   VSize   VFree  
  dataVG   3   1   0 wz--n- <29.99g <10.99g
  rhel     1   2   0 wz--n- <19.00g      0 
```

#### lvextend扩展逻辑卷

- 命令格式：lvextend  [-选项...] 逻辑卷路径
- 常用参数：
  - -L 指定逻辑卷的大小
    - +10G   #表示添加10G大小

```shell
[root@Canvs /]# lvextend -L +10G /dev/dataVG/dataLV 
  Size of logical volume dataVG/dataLV changed from 19.00 GiB (4864 extents) to 29.00 GiB (7424 extents).
  Logical volume dataVG/dataLV successfully resized.
[root@Canvs /]# lvs
  LV     VG     Attr       LSize   Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  dataLV dataVG -wi-ao----  29.00g                                                    
  root   rhel   -wi-ao---- <17.00g                                                    
  swap   rhel   -wi-ao----   2.00g        
```

#### xfs_growfs扩展文件系统

- 当逻辑卷扩大以后，也需要多逻辑卷的文件系统进行扩展，刷新文件系统容量

- 命令格式：xfs_growfs 挂载点
  - xfs_growfs   # 用于刷新XFS设备
  - resize2fs      # 用于刷新EXT3/EXT4设备

```shell
[root@Canvs /]# xfs_growfs /data/
meta-data=/dev/mapper/dataVG-dataLV isize=512    agcount=4, agsize=1245184 blks
         =                       sectsz=512   attr=2, projid32bit=1
         =                       crc=1        finobt=1, sparse=1, rmapbt=0
         =                       reflink=1
data     =                       bsize=4096   blocks=4980736, imaxpct=25
         =                       sunit=0      swidth=0 blks
naming   =version 2              bsize=4096   ascii-ci=0, ftype=1
log      =internal log           bsize=4096   blocks=2560, version=2
         =                       sectsz=512   sunit=0 blks, lazy-count=1
realtime =none                   extsz=4096   blocks=0, rtextents=0
data blocks changed from 4980736 to 7602176
[root@Canvs /]# df -Th
文件系统                  类型      容量  已用  可用 已用% 挂载点
devtmpfs                  devtmpfs  889M     0  889M    0% /dev
tmpfs                     tmpfs     904M     0  904M    0% /dev/shm
tmpfs                     tmpfs     904M  8.6M  895M    1% /run
tmpfs                     tmpfs     904M     0  904M    0% /sys/fs/cgroup
/dev/mapper/rhel-root     xfs        17G  1.5G   16G    9% /
/dev/nvme0n2p1            xfs        10G  104M  9.9G    2% /test
/dev/nvme0n1p1            xfs      1014M  163M  852M   17% /boot
tmpfs                     tmpfs     181M     0  181M    0% /run/user/0
/dev/mapper/dataVG-dataLV xfs        29G  240M   29G    1% /data
```

#### lvremove删除逻辑卷组

- 逻辑卷的删除不允许联机操作，需要先卸载，在执行删除
- 在执行删除操作时，首先删除LV逻辑卷，在删除VG卷组，最后删除PV物理卷
- 删除命令：lvremove 

```shell
# 查看逻辑卷的信息
[root@Canvs ~]# lsblk -l /dev/dataVG/dataLV 
NAME          MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
dataVG-dataLV 253:2    0  29G  0 lvm  /data
[root@Canvs ~]# df -Th /data
文件系统                  类型  容量  已用  可用 已用% 挂载点
/dev/mapper/dataVG-dataLV xfs    29G  240M   29G    1% /data
# 卸载逻辑卷挂载
[root@Canvs ~]# umount /data
[root@Canvs ~]# lsblk -l /dev/dataVG/dataLV 
NAME          MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
dataVG-dataLV 253:2    0  29G  0 lvm  
# 删除逻辑卷
[root@Canvs ~]# lvremove /dev/dataVG/dataLV 
Do you really want to remove active logical volume dataVG/dataLV? [y/n]: y
  Logical volume "dataLV" successfully removed
[root@Canvs ~]# lvs
  LV   VG   Attr       LSize   Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  root rhel -wi-ao---- <17.00g                                                    
  swap rhel -wi-ao----   2.00g                                                    
[root@Canvs ~]# vgs
  VG     #PV #LV #SN Attr   VSize   VFree  
  dataVG   3   0   0 wz--n- <29.99g <29.99g
  rhel     1   2   0 wz--n- <19.00g      0 
# 删除卷组
[root@Canvs ~]# vgremove /dev/dataVG
  Volume group "dataVG" successfully removed
  
[root@Canvs ~]# vgs
  VG     #PV #LV #SN Attr   VSize   VFree  
  dataVG   3   0   0 wz--n- <29.99g <29.99g
  rhel     1   2   0 wz--n- <19.00g      0 
[root@Canvs ~]# vgremove /dev/dataVG
  Volume group "dataVG" successfully removed
[root@Canvs ~]# vgs
  VG   #PV #LV #SN Attr   VSize   VFree
  rhel   1   2   0 wz--n- <19.00g    0 
[root@Canvs ~]# lsblk -l
NAME      MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sr0        11:0    1  6.6G  0 rom  
rhel-root 253:0    0   17G  0 lvm  /
rhel-swap 253:1    0    2G  0 lvm  [SWAP]
nvme0n1   259:0    0   20G  0 disk 
nvme0n1p1 259:1    0    1G  0 part /boot
nvme0n1p2 259:2    0   19G  0 part 
nvme0n2   259:3    0   25G  0 disk 
nvme0n2p1 259:4    0   10G  0 part /test
nvme0n2p2 259:5    0   10G  0 part 
nvme0n3   259:6    0   20G  0 disk 
nvme0n3p1 259:7    0   10G  0 part 
nvme0n3p2 259:8    0   10G  0 part 
```

#### 根分区扩容

- 1、查看/分区卷组和逻辑卷信息

```shell
[root@Canvs ~]# df -Th /
文件系统              类型  容量  已用  可用 已用% 挂载点
/dev/mapper/rhel-root xfs    17G  1.5G   16G    9% /
[root@Canvs ~]# lvs
  LV   VG   Attr       LSize   Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  root rhel -wi-ao---- <17.00g                                                    
  swap rhel -wi-ao----   2.00g              
[root@Canvs ~]# vgs
  VG   #PV #LV #SN Attr   VSize   VFree
  rhel   1   2   0 wz--n- <19.00g    0 
```

- 2、扩容/分区卷组

```shell
[root@Canvs ~]# vgextend rhel /dev/nvme0n2p2 
  Volume group "rhel" successfully extended
[root@Canvs ~]# vgs
  VG   #PV #LV #SN Attr   VSize  VFree  
  rhel   2   2   0 wz--n- 28.99g <10.00g
```

- 3、扩容/分区逻辑卷

```shell
[root@Canvs ~]# lvextend -L +9G /dev/rhel/root 
  Size of logical volume rhel/root changed from <17.00 GiB (4351 extents) to <26.00 GiB (6655 extents).
  Logical volume rhel/root successfully resized.
[root@Canvs ~]# lvs
  LV   VG   Attr       LSize   Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  root rhel -wi-ao---- <26.00g                                                    
  swap rhel -wi-ao----   2.00g              
```

- 4、扩容文件系统

```shell
[root@Canvs ~]# xfs_growfs /
meta-data=/dev/mapper/rhel-root  isize=512    agcount=4, agsize=1113856 blks
         =                       sectsz=512   attr=2, projid32bit=1
         =                       crc=1        finobt=1, sparse=1, rmapbt=0
         =                       reflink=1
data     =                       bsize=4096   blocks=4455424, imaxpct=25
         =                       sunit=0      swidth=0 blks
naming   =version 2              bsize=4096   ascii-ci=0, ftype=1
log      =internal log           bsize=4096   blocks=2560, version=2
         =                       sectsz=512   sunit=0 blks, lazy-count=1
realtime =none                   extsz=4096   blocks=0, rtextents=0
data blocks changed from 4455424 to 6814720
[root@Canvs ~]# df -Th /
文件系统              类型  容量  已用  可用 已用% 挂载点
/dev/mapper/rhel-root xfs    26G  1.6G   25G    7% /
```

#### lvreduce逻辑卷的缩减

- 命令lvreduce
- 不允许连接缩减
- 先缩减文件系统空间，在缩减逻辑卷的空间

#### RAID磁盘阵列

- RAID独立磁盘冗余阵列，简称为【磁盘阵列】
- RAID可通过技术（软件/硬件）将多个独立的磁盘整合成一个巨大容量大逻辑磁盘使用
- RAID可以提高数据I/O（读写）速度，和冗余数据的功能







**RAID磁盘阵列**

RAID即独立磁盘冗余阵列，简称为【磁盘阵列】，其实就是用多个独立的磁盘组成在一起形成一个大的磁盘系统，从而实现比单块磁盘更好的存储性能和跟高的可靠性。

#### RAID常见方案：

- RAID0
  - RAID0是一种非常简单的方式，它将多块磁盘组合在一起形成一个大容量的存储。当我们要写数据的时候，会将数据分为N份，以独立的方式实现N块磁盘的读写，那么这N份数据会同时并发的写到磁盘中，因此执行性能非常的高。RAID0 的读写性能理论上是单块磁盘的N倍（仅限理论，因为实际中磁盘的寻址时间也是性能占用的大头）

![](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/raid0.webp)



- RAID1
  - RAID1 是磁盘阵列中单位成本最高的一种方式。因为它的原理是在往磁盘写数据的时候，将同一份数据无差别的写两份到磁盘，分别写到工作磁盘和镜像磁盘，那么它的实际空间使用率只有50%了，两块磁盘当做一块用，这是一种比较昂贵的方案。

![](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/raid1.jpeg)

- RAID3

  - RAID3的方式是：将数据按照RAID0的形式，分成多份同时写入多块磁盘，但是还会另外再留出一块磁盘用于写「奇偶校验码」。例如总共有N块磁盘，那么就会让其中额度N-1块用来并发的写数据，第N块磁盘用记录校验码数据。一旦某一块磁盘坏掉了，就可以利用其它的N-1块磁盘去恢复数据。
  - 由于第N块磁盘是校验码磁盘，因此有任何数据的写入都会要去更新这块磁盘，导致这块磁盘的读写是最频繁的，也就非常的容易损坏。

- RAID5

  - RAID5是目前用的最多的一种方式。因为 RAID5 是一种将 存储性能、数据安全、存储成本 兼顾的一种方案。RAID5的方式可以说是对RAID3进行了改进。

  - RAID5模式中，不再需要用单独的磁盘写校验码了。它把校验码信息分布到各个磁盘上。例如，总共有N块磁盘，那么会将要写入的数据分成N份，并发的写入到N块磁盘中，同时还将数据的校验码信息也写入到这N块磁盘中（数据与对应的校验码信息必须得分开存储在不同的磁盘上）。一旦某一块磁盘损坏了，就可以用剩下的数据和对应的奇偶校验码信息去恢复损坏的数据。
  - RAID5校验位算法原理：P = D1 xor D2 xor D3 … xor Dn （D1,D2,D3 … Dn为数据块，P为校验，xor为异或运算）
  - RAID5的方式，最少需要三块磁盘来组建磁盘阵列，允许最多同时坏一块磁盘。如果有两块磁盘同时损坏了，那数据就无法恢复了。

![](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/raid5.png)



- RAID6
  - RAID6除了每块磁盘上都有同级数据XOR校验区以外，还有针对每个数据块的XOR校验区，这样的话，相当于每个数据块有两个校验保护措施，因此数据的冗余性更高了。可以在有两块磁盘同时损坏的情况下，也能保障数据可恢复。

- RAID10
  - RAID10其实就是RAID1与RAID0的一个合体。
  - RAID10兼备了RAID1和RAID0的有优点。首先基于RAID1模式将磁盘分为2份，当要写入数据的时候，将所有的数据在两份磁盘上同时写入，相当于写了双份数据，起到了数据保障的作用。且在每一份磁盘上又会基于RAID0技术讲数据分为N份并发的读写，这样也保障了数据的效率。

![](https://canvs.oss-cn-chengdu.aliyuncs.com/canvs_typora/raid10.webp)



- **RAID0、RAID1、RAID5、RAID6、RAID10 的几个特征：**

|     特性     |   RAID0    |        RAID1         |         RAID5          |                        RAID6                         |               RAID10               |
| :----------: | :--------: | :------------------: | :--------------------: | :--------------------------------------------------: | :--------------------------------: |
| 最小驱动器数 |     2      |          2           |           3            |                          4                           |                 4                  |
|    容错率    |            |       单驱动器       |        单驱动器        |                      两个驱动器                      |    每个子阵列最多有1块硬盘故障     |
|    读性能    |     高     |         媒介         |           低           |                          底                          |                 底                 |
|    写性能    |     高     |         媒介         |           低           |                          底                          |                媒介                |
|    利用率    |    100%    |         50%          |       67% - 94%        |                      50% - 88%                       |                50%                 |
|   典型应用   | 高端工作站 | 操作系统，事务数据库 | 数据仓库，网络服务归档 | 数据归档、备份到磁盘、高可用性解决方案、大容量服务器 | 快速数据库，文件服务器，应用服务器 |

