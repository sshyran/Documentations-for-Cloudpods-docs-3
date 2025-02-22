---
title: "创建快照"
date: 2022-01-06T16:19:00+08:00
weight: 40
description: >
    为虚拟机创建快照
---

快照是一种数据备份方式，可以在指定时间点对虚拟机的系统盘、数据盘或虚拟机整体创建一个完全可用拷贝，便于虚拟机故障后快速回退到创建快照时的虚拟机状态。

{{% alert title="注意" color="warning" %}}
- 目前UCloud、天翼云、Nutanix平台暂不支持创建快照操作；
- 私有云平台仅支持本地硬盘创建硬盘快照。
- 状态异常的硬盘不支持创建硬盘快照。
{{% /alert %}}

1. 在左侧导航栏，选择 **_"主机/主机/虚拟机"_** 菜单项，进入虚拟机页面。
2. 单击虚拟机右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"实例设置-创建快照"_** 菜单项，弹出新建快照对话框。
2. 选择快照类别，默认为“创建硬盘快照”，选择需要备份的磁盘，设置快照名称，单击 **_"确定"_** 按钮，创建硬盘快照。
