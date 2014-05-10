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

    有时候`interface`的名称不是`eth0`

        {% highlight sh %}
        dmesg|grep -i rename
        {% endhighlight %}


* 静态地址

            {% highlight sh %}
            cp /etc/netctl/example/ethernet-static /etc/netctl/my_network
            vi my_network
            {% endhighlight %}


            {% highlight cfg %}
            Connection='ethernet'
            Description='Five different addresses on the same NIC.'
            Interface=eth0
            IP='static'
            # "/24"是子网掩码"255.255.255.0"
            Address=('192.168.1.10/24')
            Gateway='192.168.1.1'
            DNS=('192.168.1.1')
            {% endhighlight %}

* 字体包

        {% highlight sh %}
        # 字符终端使用这条命令即可
        fc-cache:fontconfig

        mkfontscale:xorg-font-utils
        mkfontdir:xorg-font-utils
        {% endhighlight %}
