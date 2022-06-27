# Linux_Learn
Linux学习
# 一、计算机硬件体系
## 1.1冯诺依曼体系结构
1. 计算机处理的数据和指令一律用二进制表示
2. 顺序执行程序
3. 计算机硬件由运算器，控制器，存储器，输入设备，输出设备
## 1.2计算机硬件储存
- 硬盘==》内存==》CUP
### （1）输入设备
### （2）输出设备
### （3）存储器
- 用来存放数据和程序
1. RAM (random access memory)随机存储器---内存
> 速度快，容量小
> 数据掉电易失
> 逻辑IO
1. ROM (read-Onbody memory)只读存储器--硬盘
> 容量大，速度较慢
> 数据长久保存
> 物理IO
### （3）CPU(中央处理器)
1. 控制器
> 主要用来控制和指挥程序和数据的输入运行以及处理运算结果
2. 运算器
> 主要进行算术运算和逻辑运算，并将中间结果暂存在运算器中。

## 1.3 硬盘的分类
### 1.3.1 按照存储介质不同分为两类：
1. 机械硬盘
> 1. 采用磁性碟片来存储数据,采用随机读取的方式
> 2. 用显微镜把硬盘表面放大，会看见硬盘表面凹凸不同，凸起的地方法被磁化，凹进去的地方未被磁化
> 3. 凸起的地代表数字1（磁化为1），凹进去的地方代表0
> 4. 硬盘可以以二进制来存储文字，图片等信息
> 5. 硬盘可以通过其转数来判断其好坏 7200转/分 100~200M/s
> 一个扇区4kb
1. 固态硬盘
> 1. 固态硬盘通过闪存颗粒（固态电子存储芯片阵列）来存储数据
> 2. 固态硬盘的读取速度普遍可以达到400M/s 写入速度可以达到130M/s以上
> 读写速度是机械硬盘的3~5倍
## 1.3 网络连接
### 1. IP地址IPADDR
> 1. IP地址是一个逻辑地址，用来标识网络中的一个主机
> 2. IP地址 = 网络地址+主机地址
> 3. IP地址是一个4*8bit(1字节)由o|1组成的数字串（IP4协议）
#### 2. 子网掩码NETMASK
> 1. 功能：将IP地址划分为网络地址和主机地址两部分
> 2. 子网掩码用来判断任意两台计算机的IP地址是否在同一个子网中A:192.168.7.111 B:192.168.8.222 C:255.255.0.0
> 3. 子网掩码与IP地址相与可以得到IP地址的网络地址 A&C===>192.168.0.0(网络地址)
### 3. 默认网关GATEWAY
> 1. 连接两个不同的网络设备都可以叫做网关设备；网关的作用就是实现两个网络之间的通信和控制
> 2. 网关地址就是网关设备的IP地址
### 4. 域名服务器DNS
> 1. DNS是域名服务器，是用来解析域名的（域名和IP之间的解析）
> 2. window电脑配置域名---c:\windows\System32\dirivers\etc\hosts
### 域名劫持（病毒）--通过修改hosts文件ip地址与域名映射做破坏（被浏览器拦截淘汰了）
## 1.4 网络连接模式
### （1）（bri'ged）桥接模式
> 1. VMWare虚拟出来的操作系统就像局域网中的一台独立的主机，它可以访问任何一台机器
> 2. 使用桥接模式的虚拟机和宿主机的关系，就连接在同一个Hub上的两台电脑
> 3. 当前主机地址：192.168.8.100 虚拟机：192.168.8.xxx
### （2）(NAT)网络地址转换模式
> 1. 使用NAT模式就是虚拟机系统姐借助NAT功能，通过宿主机所在的网络来访问公网
> 2. NAT模式下的虚拟系统的TCP/IP配置信息是由

