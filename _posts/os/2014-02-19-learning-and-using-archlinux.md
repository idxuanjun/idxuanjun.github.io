---
layout: post
category: 操作系统
title: ArchLinux 学习及使用
tagline: "把工作变成兴趣"
tags : [ArchLinux,操作系统]
---
{% include JB/setup %}

本文只是记录学习过程，为了以后使用备忘而已。

使用点滴
--------

* netctl
    有时候interface的名称不是eth0
    dmesg|grep -i rename

静态地址：
cp /etc/netctl/example/ethernet-static /etc/netctl/my_network
vi my_network

        Connection='ethernet'
        Description='Five different addresses on the same NIC.'
        Interface=eth0
        IP='static'
        Address=('192.168.1.10/24')
        Gateway='192.168.1.1'
        DNS=('192.168.1.1')
"/24"是子网掩码"255.255.255.0"

* 字体包
    fc-cache:fontconfig 字符终端使用这条命令即可

    mkfontscale:xorg-font-utils
    mkfontdir:xorg-font-utils
