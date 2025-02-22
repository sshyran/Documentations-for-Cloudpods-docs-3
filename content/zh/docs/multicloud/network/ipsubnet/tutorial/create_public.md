---
title: "创建公有云IP子网"
date: 2022-01-04T15:30:21+08:00
weight: 20
description: >
    创建公有云平台IP子网
---

请确保已添加对应公有云平台的云账号。

1. 在左侧导航栏，选择 **_"网络/基础网络/IP子网"_** 菜单项，进入IP子网页面。
2. 单击顶部“公有云”页签，单击列表上方 **_"新建"_** 按钮，进入新建公有云的IP子网页面。
2. 设置以下信息：
    - 指定项目：选择IP子网的所属项目。
    - 区域：选择IP子网所属区域。可通过城市、平台快速过滤筛选出合适区域。
    - 名称：设置IP子网的名称。
    - 备注：设置IP子网的备注信息
    - VPC：选择IP子网所属的VPC。
    - 可用区：设置IP子网所属的可用区。一个VPC下可以有多个可用区的IP子网，同一VPC下不同可用区的子网默认互通。
    - 子网网段：设置IP地址范围段，格式如192.168.0.0/24，IP子网需要在VPC的网段范围内。
    - 自动调度：启用自动调度后，用户创建虚拟机网络指定自动调度时，将从启用自动调度的IP子网中为虚拟机分配IP地址。
    - 标签：支持为新建的IP子网绑定标签。支持选择已有标签和新建标签。
        - 新建标签：单击列表上方 **_新建_** 按钮，设置标签键和标签值，单击 **_"添加"_** 按钮，新建标签并绑定到资源上。
        - 选择已有标签：单击 **_"已有标签"_** 按钮，选择标签键和值。
3. 单击 **_"确定"_** 按钮，完成创建。